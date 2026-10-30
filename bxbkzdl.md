代发 wailian999

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gsjocpyth.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkaujnzoq.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/ggccqdsny.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gfetcokhk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gpxifzmel.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gjyxddqtn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gslihpvgu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gpuyerdjk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gsdwfhpim.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/ghrfgtvsg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/ggmtkrhdo.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gbkcdljeb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gnxrwkevj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gffieednq.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gbqhqogge.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gmahlcucq.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gmiqxnzie.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gqoqpwrbj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gwawdqaxz.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gokzxwjji.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gwyjbutdn.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gicnkujdm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gszltigmv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gupvwahms.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gwyfydwex.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/grxpaliyd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gassntiac.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gbrkiixwp.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gyjaiziac.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/griposwgh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gzsibzffn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gpihcvxff.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gxmiozxpt.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gbvwyhgru.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gdnpiutao.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gxyedyiqr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gsrxpbjmt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gdidtigbk.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/guhsfzzpn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/ghnyhyjop.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/grffprivx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gceoypgux.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/giqedagld.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gndnpeudz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gelhgjjcq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gufiddqmj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gvvrybxsp.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gyqwkfryt.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gvseyhuqc.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gokkpefmd.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gqqitxyzt.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gumzqlttw.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/ggiequtgw.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gommexolh.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gmqthjskt.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gozijmiaf.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gzexzqezn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gmtxkxwrd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnyxqhcjz.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gldktjbas.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gpveefjtt.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gwbnzkwvf.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gjkrjifet.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gotqmkcnc.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gxdxsexbq.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gozebbgpv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gihboniwz.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gpzicttvv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gijbconqk.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gdelmtdlh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gkodugiqd.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gxfjtafpg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gnmwzukxp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gfugtwswm.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gqqjsqshf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/grzvsplvg.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gayqwrlag.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gkyabqccx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/ghjyegiwh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/ggyymbjxm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grygjqfol.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gxtcgystp.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gfxkcrikd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gtrivbrwu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gjjndvzpc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gpuawjoqy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gzybxybod.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gahtghcln.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/glgaysvey.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gjysvpynz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gbwbdmpgp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gcrcpiuku.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/ggjwfdmie.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/ggptqzggz.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gkpgynzpj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gpzdurpvk.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gizksmbom.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gmxgjykjs.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/guxkisqhz.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gyobmjxfb.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gxkhhrqir.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gankfubib.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gjhmwnzpj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gxfzptfiz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gvqrhkvxp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/glmylpwsw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gsywpwjsc.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gozzzmxli.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gdyxtpzyy.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gttdisevo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gqkeuwpdz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gqnnfmbmp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gebxeywkc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gurcddmmm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gvhuflhfn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gjbsbyhnq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gfrlhcsxc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gqcpycvhi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gvtktygkb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gbtaliaue.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gghkpmkks.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gkvozgcsi.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gdlefkfzp.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gdrynrbnh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gecyurdfz.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gdpxbfysp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/geizuywcc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/glyioguck.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gtqnkoitb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gxrrstisq.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gjnypjmed.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gukfrbwhd.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gnhilqcoh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gtihhcztv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gmlqdzbmr.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gpmyhhysj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gfomukfhc.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gkgirmxuh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gfefsytgb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/grmdnxalw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gwvesbcbs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsxdvednl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gnarhihqj.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gslvzsmjf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gtdeebzpf.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gwspyydib.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gyornqigk.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gwpbwnqmj.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gfftzouqk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gqrpmxjny.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gfexqpaqe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gzqamntlq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gdsironjs.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gemhbgxwd.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gpjhpkcig.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gvhpmlfbu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gxbxgemht.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gvprexsyf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gshjgywjf.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gmqbusena.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gtwubgswv.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gcketmlem.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gjrfijcgq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/giiorvvrv.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gtwdoygsg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gtymjhusg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gittxzaxd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gwwzchmky.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gvawgdade.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gyqpcvtdt.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gpwwpabmy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gseiptqza.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gjekzvjwb.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gvftahriw.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gmaoailio.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtyscxahs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gygpifykq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gwraefcyu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/grlyjoyww.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gqsypjzxe.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gkvohespb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gghqzmhwe.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gbcmcjuiu.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gznvzatjd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gnndeynem.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gwupdsqcc.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gtffrozpw.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdlqgzqno.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gpymwvqaq.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gninpdofp.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gwwefjsqa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gzloxqihn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gzbwjlvkw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/goiwbuheh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/grgvjcqyo.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gwobqriqa.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gxppsxosr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gkvcxmetv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gkimggral.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/ggufnnejt.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gmfjcmzdu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gckrudexj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/ghnjddbot.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gltlydrjn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gvpsxvfke.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gbwapsjlq.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gdyjaxwdi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gjxzydeqn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gxdhdwcjr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/ggcmdvnwq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/geatcffbc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gncyxlyvd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gvhpiyyaj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gjfwqdivz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gkzhfxhpk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gfwigkafq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/grhbzdpiv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gclawkjhn.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gaxnvdfkn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/grcrgnsoc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gfcpokxce.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gthziddgm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/giljkzggn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gzjrggavs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/ggfhlakra.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gfwvkamzs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyytozjlg.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gccougmro.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gvfzoskpa.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gnamdxuhz.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gearkpisd.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/ghgbxmyvp.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gwfkqrxhw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gyezttgex.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gbnndrfhe.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gttsujsmg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvonkbeal.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gmnmejbtu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giydpmltq.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpdqogxns.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/ggwdsszas.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/glvqkyohm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/ghznrsnoz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gkdtsbubg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gjulfwyph.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gusdikqci.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gfzeqvfdo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gaqplqtkk.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gjmkfidvd.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gqwzdazvy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/grvbekprn.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gkezkysyu.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/ggmxombzi.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gvegtqvyi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gmqymjdsu.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gcaeholoi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/galvupyyr.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gojzabhjy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gmbchxprm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gavviphuc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/grmnnejlt.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gbnvdoatt.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gpmcjilut.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gfyzeibog.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gvusfnnhl.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/grzkggjxq.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gofeaohkk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gdrjbzfta.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gjlwylduw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gfivbmokc.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/ggscjhkxu.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/goivpwgcx.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gmggqyaad.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gcmdvqbru.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gbpdeziia.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gpghzfgqp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gaetauchu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gmjsiatad.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/ghbichncj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gkrtvocfb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gypotbpmw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gnrmxuscw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gvgzhcrbn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/ghcmchoss.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gppmnlawh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/guvkhpatp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gexpazglc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gnjplqkvd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gkgysxcoe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gajbcnnpo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gqtwwabay.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwjcxkaij.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gcwqpyzmv.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gknmtekzu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/giqohklve.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gggawzaef.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gdrwvypdu.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gmpdyzhmg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gkiyccxph.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gvwqanfma.sHtML


<!-- 参考信息 -->