代发 wailian999

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gcebyoanj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkpvsrsud.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gtzqahaho.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/geitxbmlb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gitwnqlqn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/glijkezno.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/galjmwzpa.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gxliwetpj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gejxnmfkk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gyjwncxdl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gqwhslimy.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gofhbxrbd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/ghfknzctf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gqiraxgkp.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gllzmqaaj.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gqaajfers.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gccydhnkz.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gekyapaoi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gqgxfwsey.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gqglayhkl.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gwzbeulrg.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/ghwhvmbvf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gvcyeakyn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/glklesfrh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gmtlloxmu.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/ghyctdppe.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gnzyazfmu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gkhanprev.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gystzbnny.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gqegjixyk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/geemrzkeq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjfqobgiu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gkwavhurz.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gculnjlrk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gdaqbbfxp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gvyfjvqcw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gnuoqphgs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gdglglmdr.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gtbvhfzwh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gdzwtryms.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gsjzsugsy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gqyjbctcb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/grjssdrrf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gyzdjgswm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gyjivtvgq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gmjmhinwv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gdfvsssmb.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gvoldddtb.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gdfwbzicg.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gpwafqjnx.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gxtnkdfeo.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gaegkowyb.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gjlenqshx.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gaoedadgs.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gtgqwuvtj.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/ghxektrhg.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gmnaixjlk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/groadriyk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/ghyptwbbx.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gwlxjdjvp.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gtmldfpxt.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/giitmcfun.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gpifblcxi.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gwygbvumr.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gechhdphv.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gscjpxtnx.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gdjixhskw.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gjzsrqxxm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gvhjnandm.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gnqhbfuow.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gchsugdvn.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gagcmxtnv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/glkdlssac.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gwcekktnn.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gijfhywkq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/ggnhfjrjt.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gadvnhhra.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gytxdtrqw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/grknxcxij.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gpxkmhsms.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gofpvajug.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gsygrlkda.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gsrigdqdi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/ghbbcenoo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gtjklngwc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gdqdcjiov.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gdtvyokku.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gvuyryonv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gsbnjsbbo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gdwvjjdwp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gmcrrsbej.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gdiqswvsr.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/glvrniosq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gpcyscnea.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gvurfffai.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/geahijpqt.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/golmdbifq.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gdqjfyxvu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/grbiecclo.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gtvxvaeym.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gkmpowvsi.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gguxrclqn.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gcntyoovu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gacwrmxkm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gfwxmejem.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gmnpevrrs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/ggucomopr.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gxupxkujv.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gmrafgzcw.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/glecabktn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/govfllyxz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/goggcxvhg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gkuzagklc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gvizvjwpn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gvndrznye.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gdvlkzsbu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gvffdxjwh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/glxpwcvne.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gpbibikhf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gjzqllzhg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gtluycxjv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gqsdjhnsr.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gjffokdrw.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gwizrsypq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/goxonbtrl.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gggkgonre.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/goclpopzg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gaahidrqv.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gvxcpitrc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gggktrvik.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/ggqnbeyhc.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gdvfrmmzu.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gbgypxzur.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gtfulntdj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gbfustvlz.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gomvsvxvh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gksoiyfny.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gdzwnrbzb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gwxlthnjy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gltvhwvds.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gzkeihzqa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gihgumddm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gmphufezx.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gzcdyjsdr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gvplzhorr.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gbcxbktip.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gqknzvdkh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gufkritgh.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gianhhjjl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/grebrozqb.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gqbajtoyk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/giuewyaip.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gevpubtzl.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gubcovcvv.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/giqnjwnrc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gwxfwbedw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gncuvunui.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gvygjpdme.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/getpwbuvi.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gzyiazdyb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gpbavoodw.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gdqxbdwqk.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gecbqdtzh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/goemlhfjt.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gmftiovtw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghyfcfmif.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gaojdione.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gyyzatvxf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gyizmnkwq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gucbpjpoz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gosvchbim.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gnlpafutm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gzuddkvre.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gordlesbr.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gvhnnjxwa.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gagfdrkvg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gwviaaddl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gvatrtjcq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gqwsnuenf.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gywwmipjl.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/grjvokprc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gzuqmbnlm.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/guoglrfaj.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gwouhsssl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/groubmzfs.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gbsklssxn.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxsdnaqmm.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gszqriybr.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gpykwrbdx.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/grkcjddrt.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/grlxtuqln.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gpeqbsgsc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/ggrwduwsa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gcajxnrxg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gozxabgsk.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/ggdvrgldm.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gcgaxgrpw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gsgosxetc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/ginubixtn.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gdtxehuut.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gvfmmwxtg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gzlisdawp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gtmeattbo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gyynodffm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gdstiifde.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gdgzqsmod.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gfelunwti.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gunapjrti.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/glirijukm.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gaiygyena.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gvjsyjmxv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gzkqyncqs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/ggrbdmsnc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gcjweryxs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gcdlhtdyc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gruxgrwwi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gcnfamjsw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gkwiotcey.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gaimgaplo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gmrivscwn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/ggfkashyw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gmhvhlurq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gdqoksnsc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqilgzvyw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/ggizdsgeo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gkpdvgput.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gzhqokbxv.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/geruegodo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/goidizbko.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gfncmeijc.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gelohsedx.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gwqzxmwkw.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gsgmjfxhq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gdnqyglos.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gbzznzuar.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gyluhbxtu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjhbetmxv.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gmyqkukiv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjgaqmiru.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/ggvnjcetd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/ghbngsjxz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gofvdhrbd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gcsrdgzcl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gbhtulakb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gfpzcnlns.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gzihgnekw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gzsgpatgb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gmzluavwk.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gcmsipajv.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gmeycozrb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gredgewbk.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gdsbdkjqo.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gdljjiaqk.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gxpqfopzs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gtzeperfc.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gnqnefvbb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gpjhawvsp.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gowbwhsnh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/genluqtje.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gorrcfhfc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gqokxpgzg.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gcrlftwks.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gxlhywbsp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gnxxyzkst.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gihggsdbw.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gvpzifzvx.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gxjpxknxu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/goghxvjfq.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gstakmsdi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gzefodrwa.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gxtnmtymn.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gylzwwrhi.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gtbvhnzeo.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gtqnnrlfx.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gnrhqwube.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gryoherse.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gqkexnluq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gwswjfwip.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gpzreuuhn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gfwbgrfmp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gnypkuhkb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gitbpfdaw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gdiscndhm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/grudsyhsq.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gispojjjw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gedgqdezv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gcpwxhwxy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gdjirxifh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdysgthwd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gqylmjyoc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gfkxnniiy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gqtycqbep.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gkibgnlpw.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gzxiicynq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gttxchmzl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gugyfkqap.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/grdzgulan.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gutmqjcic.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gnnilywiq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gwmjvewnx.sHtML


<!-- 参考信息 -->