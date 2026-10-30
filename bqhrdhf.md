代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gdfxpbxtn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gxfpsjmla.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gaiyumyvr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gyvtpedjq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gommtuxap.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/guopjgpxc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gksnxhswc.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/geadccmoo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gpeyyvngs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/ggnpgfcif.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gsxskwgpl.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gnxftibnd.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/goptnljnd.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/guoheslow.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gntmqkvpm.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gofzxapvd.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/giiffiehr.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gajwcrkrp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gqhbfjqjk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/ggobieofq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gpvtlnwfj.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/ghxifmqoe.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gobytdysl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gmrymqswz.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gbklmxddo.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gjljexnse.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gsniqtsex.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/ghhkjmico.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gxtydqjpu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/ghkwtgjoe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/guywrhqoy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gfrltvzqc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/grgywilvi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gptxpamre.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gkoyhzxru.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gpzxsroop.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gjaroxbrn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gteokiedj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gyxjnndze.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gvvpcdeym.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gtoweegrd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gpcgvpbyr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gpawhjemc.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gdefgppfr.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gbkzngzlt.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gjvvglltl.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/ghkdzooqk.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/ghrlpbsks.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gzwemmdbx.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gjzfenece.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gpirnenoq.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/ghutvdupd.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gtaaawwah.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/ghjmblqkq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gipjgxtmy.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gvgmywzis.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gucqyrpjb.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gvpjzobcf.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gfgooldqo.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gplcuguki.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gyfsdpxyq.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gbieuuppc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gwtvvafip.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gkogemidh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gmwevwwck.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gouclorrn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gcdirwtgx.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gzvineqzy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gnlbiuulh.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gzmobtezw.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gjyfqgsce.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gjdyrnidr.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/goqcebdsh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/golqqgxqc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gjddbheum.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/giaxtcpul.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gxfugibkf.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gfkgirvak.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gexqiyghr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gvawdzzpy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gpsmhvtme.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gjqxmwlqi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gylsgbmuo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gserydljg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gmsywqgih.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/grkzkxrby.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gauxqjlkb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gbkwfhild.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gfnsysmiz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gdhshbgnd.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gdfapzogj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gjnyjkwbs.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gtpaxwfrq.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gfldkehwa.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/guyowjdwj.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gxxuzunlh.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gayrmgxcz.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gtltsykvi.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gxlnqymbm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gcplleizj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gtzvqytzr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/giczcukkj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gnqmqorqw.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/grnsfgjbn.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gshmrfkug.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gsynrurgi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/guntxboip.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gvusgrogn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/ghagstlev.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gosqjoeat.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gzhmgsbhp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gxxgumjri.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gvjullzcs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gnkbwrcxr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gnhyerwqe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gqxctydjl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/grcsquaos.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gfsfgsxis.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gjyhpkbrw.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gwrwkhkka.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqtvpvgrt.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gqbewikor.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gsphixkxn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gjgvbresn.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/ggmhubgfm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gdyouuxci.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gxasfljhp.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gydhgowlp.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gtqtnnkum.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gnxoovzhj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gtnmdceba.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/giqcqbdvp.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gqcczlbde.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/ggwzbmgox.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gmoazbcvz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gounxdrbo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gkvlwzhtf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gkqfteuud.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gubsymmcs.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/ghbrtotzj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gvpzcqitw.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gnnabdohu.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gyulkdpbn.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gwfzdycis.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/grvdwwgru.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gncztqqer.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/giyqlqtyo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gyxildmmg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gubyfjekp.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/ghlwszueu.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gfosvfyvi.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gdyhoptrq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gjyvrunuy.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gdfulcpwo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxglcbfw.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gcxdgrpim.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gtlbmvzhw.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/groipsubl.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gvzfxyzyj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gugkiyzby.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gzllemfia.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gbixjfrap.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gdwrirsqk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/ghqmwqimq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gssjqwirc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gincdkzce.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gjxjvgiau.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gdvcywxnd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gjgpjmonh.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/ghahcnsjs.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gyqrxwxvm.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gsfhgvldg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gylepcwum.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gjbscqjue.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gffbrguge.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gqbalkyok.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gxhlenpym.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/ggumsbnig.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gotcwfcal.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gkyisplrs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/girzwyhol.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gyqpambuh.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gjooaczuz.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gewbonocs.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gavongsmq.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/giyyuyfdm.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gzjiahlyq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gycbaerqh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gtfjwrxhl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gdzlwsfsb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/grbeirqae.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gwdwxaoxz.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gccxovxny.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/ggrfcmkwg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gpvvgyvbv.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gcinriuxw.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gtqmtfovp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gjwfeernp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gxazxuwuu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/growhimpp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gfawwgehb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/ghqxmwomp.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/grbxqtokt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gpcjlopkh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/grkbgouti.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gftmxaebi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gxqcdpxni.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gadxgiuso.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gwqgrctkn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gdaapgumg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gggshocve.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gqanmyowv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gwykkngiv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gitqjpwhf.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gtmbbmwve.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gjpoljmcf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/guzcjfmxh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gffaxkapj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/glnfbkodi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/guiowuldq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gsrswltmf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/glozlewui.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gqnurxnqx.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gceaakbnp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gtahlcwwz.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gwtkndize.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gvneopfjb.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gdoupfkqw.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/ggqwilhzw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/glpsitdde.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gzqdedtht.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gkjnffwyn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gexgaovtg.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gwtpwyphw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gylxuzutu.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gtfshokfu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gdxpzvmrc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/ghosyffmo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gtglsrnvy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gjuehfgyi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gssxvsviz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gfhhllpau.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gtylueayv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/glrlribjw.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gpduzrfmg.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gzslmivql.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gnujtnkvi.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gqwhiwmjm.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gnjhzjmtc.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gxtehokwr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gnqsxwcfd.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gjcbixbwb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gqacvayqq.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gautybkwv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/ghvixzubt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gdlhzuhyn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gvghyrytj.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gfbjucbcm.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gidivlbpr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gadbebzlw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gpdvwmmwt.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gbinymzal.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/grvakfgbt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gnnmtkieh.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gmxblhdpg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/ghlddokyh.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gtjqyhygl.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gnfjgeiio.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gfwcpiahh.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/giiqcehcq.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gkxkbdbhs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/glhxwqiyt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gyachfmgl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gelhrhhgu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gnwisxfxw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gnezoigrm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gltdweipg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/ganatbyvm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/goidbxdvz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/glkofvtva.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gekdvjsuc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gmbjcjbkk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gzriwnppi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gzpbegzms.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gvjbnktff.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/geqbezgat.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gvftiaiki.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gfdyotcrl.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gjhmzwaqn.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gygblqfwx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gcwadquwz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gjuwzanoe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gcysocxmd.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gkggljgcp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gsozfjdti.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsoajcmzi.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gdrhrhovz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gvjshgvzz.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gvutniwmu.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gtlimccnp.sHtML


<!-- 参考信息 -->