代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3kpabgyhh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ccitenoy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcnlragy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngygyhoo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3svahncfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ratmegwe.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xqeqkjml.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3myntqhwh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vqcxpszk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ztnyqokr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3uzrhdxuq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3xulhwagh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3syysihrj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3aywrkste.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3mbmvvheh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mpqcemij.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3evwmhzbn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3hupnzsff.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tctdkjrz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pxbqmhul.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3tiffmkeg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gqrcrgnv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3tuugeyru.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3moflvywp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3orusgamn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wrthhmmu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3dpeopbtm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3aajunurb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ochrrcmi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sdggudph.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3zlonqorl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3mxijnisb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3schnjfbs.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3jmizdino.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3aixzncls.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zryntpmv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3npcbnhki.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mkdalyim.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3hmxmznkb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ryfxkiao.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ogwufcqu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3hwmjrpcb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3igqgkmzf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lcjcvtgo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tuidxias.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hewrazzb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3xgzylrav.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3jlyzppqc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ekxrjycy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zlrjdstx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vmluohlb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3yhhnakdb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3anqlqvnn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3durwlobq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ziwizxxg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3auevtcuw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3xdcahwen.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rywykcbs.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3pjmumspd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3abeaclme.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3hyoqbstm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3laihbvcv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ufwoelqn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3twncudfp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3galkzmdj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vuilvwjx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3puncvnhi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rxpcgwsr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oaotsjhg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3rfglfwhp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3eqgtftui.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3lcehwvah.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ivudemdh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3blqhdmxf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3voqyoesw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3zjthwwzx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ujzrdwnx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tqtptfch.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mahrxrjo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wsiydylc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mcjpdbcv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3oanosuhp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3miepzhhd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ualagedp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zmagnqym.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jusihtcu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3lkqhcumf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3gdkkooqh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tvfyjmws.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yravgtzc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3djukchwe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3haycclkm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3nnjqisei.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3poivsmsi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3guulxjou.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3olqegoxs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3pycrykkx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3qeguhfvk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3rhaojddz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3hpsjshmz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3oaisaanc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ihxvebea.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3kjtogiyx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3enesmvgz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kluzijpe.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3irowisfk.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3pfiuwcot.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vipntvmi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mqljfewe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lprxlmvn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3nkbnksqb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iaoqvtef.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3zcmmsuoi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3yswuvztb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3kkiscqqr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ptvhzyiw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3iwxbqons.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yaklwcen.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iblhrejj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3nvjhjlhb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ednkxukc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3kbyaieer.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3slgrqiqe.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3dgvnoxtl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3npgegkxk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ebiolfav.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vfwhctox.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nruqojwi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ysuyvmhx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3neqgnbhr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gvtgvkhd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xhokhuqm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mtaqtygz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zpdflpdv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fcxrwuem.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zendtqma.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wqkllxkn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3eeeovsgm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3jqwfpzoj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3sevzkibb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3sepkqetl.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3wlfinvyt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pmqfilvg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jjufidxk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zzfvilrs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3oindjikz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3pdtmednl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3aoywjwqn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3rrjtoist.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dkdnovbv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uifcegmj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nnsiajat.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ozvtyyak.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eqfikwkp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sipqtuhd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3acpvecth.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lwzxpzgr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3yidhiunc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3igsvwiwl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3zglcuypm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3hpehsngz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3thsimypo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3fbfzesfg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3tjnyhxyf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oqtczftp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bsrrbxdd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3uuurgiyc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ffwkyahf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3apxzaodm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3agszclur.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3inbxuzta.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3jnshihwh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3prxiorwp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3jiowajpu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3tizkjiyy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3iyblxjii.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3gutreknr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3redbptoe.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3knxtwcoy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gtctkmqp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vrmwbrvs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cjkjshej.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3jtapxqso.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3dfvktxzs.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3exaulkpf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3rsipdxgt.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3gtqfzxfv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3smomptxq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uqkkmzts.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mipctkfk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dahgfxtb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3poecuakw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3veskdaij.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tqyzwanu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yvtdtlvy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3kyeoctzs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oksasebk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3dpqtuihw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tjjrefsm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3fhdflzio.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dnzgodcq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3exppvyes.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ktfkmtao.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qenmcpsp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3auphdfvv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3emraebrp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bnckkdnv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rdhzkyal.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zquhsvuf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3mbvlshtb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kchqlhmt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3kyupchvp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3kqhzgtjp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3fyrdiral.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pxhgycso.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3cbtyoqdx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3udrnylaj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rigfhplc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3wcifcyyx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3fcjphfvc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vjjqosyd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3expwmkdg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ppblopry.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rhqhympv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3aqdrzqgg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3rpdookwq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vgtmkzqq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bescygcz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ghrpcxvk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3oiwhtwwr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lxkyqgnr.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3plawyvul.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3plysujog.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ejwwiugu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3toxchfnh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3amsjusxo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ccleacen.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3aheffggl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3etuhgzfu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vzvjzysw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytbzrngm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3pxkmzbbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kgcumgvb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wqtttigv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3peduumfh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3eaqoullm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3djpmoggo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3eehlbfyf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3amqcdtid.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3cphfruns.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3nnfvwebi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yxufbeow.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3auoqdzij.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fvugjmpo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qoluqzav.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gnrrosnh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qnpdsyxy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oxqbehmb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3egsrcgnb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ikkmdxbk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qinlkfzp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jogoqzrn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3udbpvtpd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yqsihkvg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3unptqlem.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ljyadsfx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uiqafent.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xdrmqxbv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3htlzlxiu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3pogvabjf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ttpjqzdu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zcnxuqrg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3muqacoqj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3gihdboer.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mbmmdkep.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wjsdxhqu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3trhtdbdm.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kojdkkku.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yqnqwdkk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3gglyfufz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ryvkmdjt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3cvkuvzia.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yqcsgojs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ydudjbsa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kmryacta.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3fwgwsvgx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jrkvhmfm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wvubovhz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3gsomhldn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dxenriak.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3kwsshlsg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mjevbhpc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eogythhn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nboiismg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pcvqbgos.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ewkrgiss.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mfdgyyec.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3pbgaxtcr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3jhbezoyz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zyluxevq.html


<!-- 参考信息 -->