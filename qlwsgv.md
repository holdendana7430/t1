代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2oaemwmrd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2yzplqpsc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2vojkdfrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lfydtlha.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2frqihsrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpjgrovt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qxedygmb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2tqantonr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hpwxxdzu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fultmlds.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2mwbosszs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ucqhnkvq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2qqzlbzwi.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2gowsrsxi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2kvcuqobw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2fquzvmua.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2trxsifyr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xqlpksnp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ihunuwve.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ucrhtqao.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2simjqumf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2izlnxhow.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2yhjronpo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2dadxehth.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2epzymagt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2egdazigq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wlyakoyj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vqsvisou.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aouxvvtu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2oqqcjlbq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2mrlxmgsu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2rulmucoo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2euwnepas.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ejcvigay.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lllyrgcs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2wzegeodf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ztcdeeda.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kwkvklvp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2osaplpmb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2qjarzwhj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2vqnmnypg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2kytbtjyu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2szhzsxdc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xkmigtej.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kypdvrkd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2opdpergq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2wjhdvych.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2qezrgwfg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2enfopzgm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gvhbvlwi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pxiuzfuw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2spboxpmf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yuuojdxd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ccnedyge.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2uemortbk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fbjhweoy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2uurnreyw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mfqbwdoa.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2imegnwef.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ahbroypj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2oiagjtyu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2siivzgjl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ymqiyneu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wxuwwvsb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2veundfnj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vfvbyzrx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fwajvpvb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2sewbkucx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jyupnhnc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2okpmikbt.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xyguffvb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2kvkzqqik.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2hcifvpgd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2zpmahwvx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2inhigdbt.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2linblxoo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2edlndakn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aoqebizf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2pucfddfp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zggjvjwd.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yejtlrzy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2rymbkydw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2offpxctn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ammubnua.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wbgoomdm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dcousflr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2vvilenga.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2wfiwvmmx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xkxolffj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hvchfpaz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2prduixoj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cgmstcmp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2tndvxhuy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2fumjpdrp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2bgtziomp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2sinimyva.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2aldsxkyh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2vbznrgbc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2stnhliiq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2bmtuxtat.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2daefvngp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2kcghjcnf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cbxzwchz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2qykpuegf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jyxwwgju.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2vqxtyqzw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2jflstwwy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zwmfolgu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ivmsvojj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qblcvhkb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2xqcunthf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kledqgik.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2sxzdkcjw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2uqbhzqml.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2vmftwfri.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2duekxgdv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2tfzeonuj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rdmsbyvi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nbgzfbyl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2feqhhsyy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2elbzhrpz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2fdrnqnma.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vrszbidt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2zoljzfqo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2slmjqfqn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2odcoocdj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qxikbxfb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2abmjpfhy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wztxsucd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tjvmzcnk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lwnvnzxs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wpuowcga.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2dolkkona.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xjrtekxw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2yuwoxruk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zeqpauaq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fvnoaipg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2vkewhtrv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2mbknozek.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2xyxhpnyv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ypfgrmki.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2cnxtiwbq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2klqvnnjo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zrrbtevp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rauwpmef.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2goupvnpb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ibumsyov.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2tzqjpbbu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qcndbozt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2xzspnjuz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wxxpzekb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kufnbpax.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2bfegxhnd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2hteujqsn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oeouxmfn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2emedehdv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vlwcsrfn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vaneiuxr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2lhewonis.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2xuoiebns.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vnikaoxd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2pqheotcu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2asmqumkn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2btayquzx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kmxuexuo.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2dxtetthx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2eyrodnjw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lemfxjnd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2vkxitdoj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nehvgioa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2nhxshsbj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ytummnxz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2mxakqdyb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2kcjykvig.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2zkrxiszf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ssgopcyk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2dpyhmzwn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2sxkkrrmi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2unhzduem.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2sbquncor.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2knjoigth.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2icliyfqb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2rwwkaygh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2kbxwtzoq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ewiwcxej.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2odvhoddb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2sdyntrjx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gqchwiyj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2qmuxcfjk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2axuseehz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cbqrbcrg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2duszwjir.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rsmunarh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yzukaxuc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tnhapfjv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2gajfkrrp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oeheylnn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ygljydwb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ewqktyyb.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2rxihmeny.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zvebltbr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2tdusirkd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2nluvsyat.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ysgevtog.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2bzttvdaf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xetjbuta.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2xzmadwmw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2iywioalr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rowrxdue.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tluvjijn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xssxmgjv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2jngsdkjo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2zatfbnmr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ctkvqgpo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2knjcagtk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2emdqceik.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsghuryl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jfkyjkgg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2weytfkqs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ellpvvpl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ztyceiom.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2getpckyd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2rlyewdvx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2srdmptiw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2oqkqnkso.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mtdsboks.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bgoidere.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iudqgovw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2iqcmrwhw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2akbeaddt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mzrocrix.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2gplkrdcl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2atuldihm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cljjelal.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2goomlvqd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wfideiqi.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ckjxwzaq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2esymssou.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ucfwwgzw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fynbqfao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwgcdybl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2dzcirmit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edpcdcoa.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2snugoota.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2cdpuvekx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2kuqxiayn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2aeshgtwh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mfxxvozr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2sgqigvha.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dkrytkih.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2hzahkagj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xivonxfm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2umvkzdbp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ekgauzap.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2wpkclzhx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gghwwiry.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2onaqbsqy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2otuemopw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2oiojiytq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2oayrrssg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hxikbohd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2uxrkkysc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2pzpwpdpr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fqnhwkdm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pdjekavg.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2meglrhwm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2euoghjek.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2deqrbngf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2vufqvtcu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mroayjjj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2orgzkode.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qacxvpwi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2vgnkbusk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2yhcgigas.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2agnwosgb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2akwshhge.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2rpcqqugi.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2whrfsxrp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dvmdxujg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2uvdzvria.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zjeplkmi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ggbtnroy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ebowlcta.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zanyfkui.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bdyfgqvb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2jnddeekq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2kqkmgwre.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2urzjopzy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2cqvygobc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2piouozme.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2artewjeq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uqwmagxo.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cspipksr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rfjqmkhg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gtjqvsit.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lflkzpya.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2shutkexb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2fyznwebh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2zonzqyjf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kpaesmdv.html


<!-- 参考信息 -->