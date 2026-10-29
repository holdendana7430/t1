代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gdfhbmsiy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gqvqygjwl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/glgjrswqm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gaycsnhjg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gkkgcidxf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gszywbdva.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gbgnsyrbn.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gusvdjgvg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gwbjlnwro.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gxiorsckk.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gqftpgbsw.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gjndbswgq.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gpeapbfuc.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gqnsuredt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/givdkmqqa.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gbpgkkkyy.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gbdxukxwk.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gpklcjubx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gonkqcvox.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gwoakcpdk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gvbnlvgtn.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gdmwqnvke.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gnjzfmaqa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gtyzvyrai.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gtffeoumz.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gtwitsaoi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gisapqrul.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gcqpldbrr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gunywlczi.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gnvedkjhl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gudrzmxow.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gqenklubx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/glxyaooqn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gtfgjkupf.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/grhwbjuyx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/glmpmpdcz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gcdrotygf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/glbysobui.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gszhlszfa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gznuungbm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/ghlkussxm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gizbeswah.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/ghtowyruk.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gbcmjrllh.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/geurdnanu.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/geienazog.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gthopsxkp.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gasikdtba.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gnjedpgka.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gybfarlpe.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gmrcllsad.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gmpuccdjv.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gqbeugdij.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/guaxvwrtk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gdoonmwwn.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gkozbhgyl.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gxuakfuer.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gzkeszsdf.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gtljizioy.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gpilxfewt.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/ggiwzqbzi.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gulmfwzwq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gruhgsdmb.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gqlkvcvan.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gcdcvepgh.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/govxfxagf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gfyqgsdiu.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gzlmsqzbn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gslnfzebm.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gknwwzxgv.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gmunsgbdi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/glfsgcoag.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gptbqupuo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gwhibpdvl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gqejrrkuh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/guqcaqijl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gbcxzzulk.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/ginqwuhkt.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gbranclmr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gxtygalys.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/givfbaluy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/geymrczkp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gksvxtfde.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gvqyzptbc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gahirjkbq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gokdshdzu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gxubvgfbc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gkkzzafut.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gywpickdm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/giimaemly.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gzptpdqbh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gerbjjwyr.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gbdfhczja.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/godjqygim.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gaznyroga.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/ggwablfse.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gjvllcfpw.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gdajqrhhm.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gdrirrqah.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gxfdsveti.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gvzruzyax.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gtfcutoes.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gzkdixdqt.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/ggscdxoql.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/guogwzyzq.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/glstbtkyd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gpinpnurj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gmuqadzll.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gsydziarz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/glsmfoapq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/grxdnwhdb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gyzwtrfvw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gdeywlpcq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gelrahfmb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/grjqmyzgd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/guurdcyqo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gsftzvvud.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gvivuzvez.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gxmsurxkm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/goloilrmm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gofknqviy.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gdknfqgzt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/geqzctvew.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gncrzfuic.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gzbntrnfm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gyhtjjtjn.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gamzveoyq.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/glwqqallf.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gyigwqjfv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gpwjpdixm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gaecjlitw.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/glhnfjkvm.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/glhyquehh.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gvtkftsqm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gececathc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmgwqlulo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gqbdwocuz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gzjphnuac.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/guupjhbgw.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/geyeccltx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gzjpykiht.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/geirpyvfo.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gyvykcwfq.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gsgetznwx.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gmnywmztz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gpctbllfa.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/glsifptwq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/godopbwmm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gyqhjwejt.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/glifskipv.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gqrwmkngj.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gzjhoenav.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/glomipfzw.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/ghmhrzxxs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gaxbckafu.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/geymonntt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gguxhpqmc.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gwgvzuvhn.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/ganxcbhhn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gyglnitaj.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gpmnvzbct.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gkfhtpqeb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/geuqgdveg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gukkqoada.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gtgwgkvfr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gyhogqyjk.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gyjnowjee.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gsalxxtio.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/grgetlrki.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gxraxkitc.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gcvehadls.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghyjfeuue.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gykoaokey.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gdmeaottw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gbxrevxja.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/grzsjgcvm.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gvudpsvuc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gzrmbrilq.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gyuxurolf.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gbiyhcswt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gcwkqjlyq.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gtcqjtpxh.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdzzqduxw.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxthkrvxq.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gjnzazceg.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gzakhztyd.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gkvtybenu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gmtlsoobr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/govomnwun.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gnlcwupky.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gkhsglrnu.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/glbuhvyyz.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gcjnwzson.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gsloratfi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/grqlmodkp.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gsnyenxvr.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/grgxgulka.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/geazmrege.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gkmtsairs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gtcaaimfu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gphesnnem.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gikqjvxbq.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gmrrxnwlr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gcuzcgwzw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gxejpqaal.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gogyloutn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/ggldrnuiy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gxyjegqso.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gpjsquage.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gqppdqjoq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gmioptkbb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gorwianst.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gxmhpkliv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gmrquohdn.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gksigprtk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gryerlwhe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gzjgwgbtb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gmvfajpjr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gkfybmrir.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gjxadzkeq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gsgwddxcu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gwmnyucei.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gpsyhntvp.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/glbpskcbd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gnindlqpn.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gwsknmdck.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gqepytyzq.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gnpqkrkyq.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gzcsyetgd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/ggfytebcm.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gcesuuffi.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gprpunpxt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtegqcktk.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gtlhuzxiu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guinqvwib.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gsqmxumfi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gxevvoazb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gxxggnwgq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gvdqwluru.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gggytdfme.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gupskpxoa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gqwgqyusw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gqpbyogku.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gvyfckxfp.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gqohacnel.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gsuxtrwuy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gsanbnwls.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/ggdhzyfks.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/ggjuznikn.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gczsgmegq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gjcxzvqim.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/ghevlylcp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gvzrnadmv.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gshzxjodg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gstgldmij.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gesbkkxir.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/giyqzpuce.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gomxrmhyl.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gpkjrhond.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gjgedhohg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gsisraddf.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gpsmlrgpu.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gxlogcspc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gbuqfhnrg.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gwfqafobq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gwzfekorj.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/grtiorjth.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/glxkaahug.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/ggqatgswg.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gdindxpze.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gwfzowxor.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gifbonygr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gozvmqzsc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gonmkjwmr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gfvubnbnr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gfwivrxfw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gpxspdomm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gkqgpckba.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gzokyjzfi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gnfdrnrsn.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/ghywicdmg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gztgjyrsj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gtyswgzxc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/ghjbafmig.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gesvsmbju.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gjijvekdc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gchlrkmlk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/grrfarmcb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/grzwydlvf.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gmikyynih.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gjaibabax.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gsdlxfxyd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gftmsjhon.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gsmrhixqw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gehswegbj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkddipckg.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gilnyvhws.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gtlqlqhac.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gonktmfyh.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/ggcuujbqw.sHtML


<!-- 参考信息 -->