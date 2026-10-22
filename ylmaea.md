代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2mvmhwffq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lxeuvawh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2rjczhith.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2uezhtdft.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2vckegnwq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2dbjchrcg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2csypvdet.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2khmwewyx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ekikhtwu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cgzqfnkz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2umduttur.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yjydovkr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hclpjqxv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tgoinnem.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2brvqntrx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2bjxxsztv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2asckdcic.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2oihltlzi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qteungwi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2mvqaspmd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2klemebjy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zthbdxtc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2hbzkiylb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qvnewioe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2wiqfiont.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vaftbjsc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2cxpfelcu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2wyyvqlip.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kidtrryi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ssqelufd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2dqaqtmzt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nqgmkxrj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bcoztisz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vaeuvxuz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2wydeznmh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2buhoflfk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tvoleaah.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zgcmalba.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bfqpwtrz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2umhlbjrq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gswyawzu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sbpognar.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2crdqjlmb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qxejfsxh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2uvehvizl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2abnoykno.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nzqppnzt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2mikwexkf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2hsetzczk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2fgbvdmja.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bqshwdcr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zexnpztz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zamdnbpx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pqiucpji.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2pociatio.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bviuxkgv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wfgqrnrg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jyzbdabm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2gbwqbrxk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2pxmtxqlp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2yvrskxss.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2vernkond.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ccynnxnj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2hvbueimm.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bqbmufmp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eukhwpum.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2jbnaovbr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cfgpiaxf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tzkoocop.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2llyrdkbh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2krghrzxd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2okjbuhym.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ngipywjd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2uykebyhv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2otbgxbby.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2bbzhflgr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2cifprsga.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2binvchaj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qtgmuipl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2gzevxqsk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2vlekchgz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2teywhviq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bupwchdk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2zvpbukmc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2bezczszr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2cgofshvh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2tomohwbs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2etikfyiy.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2cqtodosj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jknsndsr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2otykuppo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rglikorr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2eygdmktp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2gfecvzyl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2axtylwia.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kiuyvife.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pnxgnzfs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bxrupndl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2uhzlzrpb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kzetwlny.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dnzgoxwj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2iclrcdhs.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2lydufrzm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mfpeuaqr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uergnuts.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wmvrhcjj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2whnyndqe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2rjirubss.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ssrjghdc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2pmfnxgly.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yodkdkfc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2pghxfais.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cuklylat.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ypvnymtj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vzzsgloe.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2posofqqt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2dymhyrbm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xvwmytzs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2eobhunbs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2murtfick.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ekjduxcg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2oxsaqbrm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hrubhixr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lzlscidw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lpmqqnsh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2brfibmnr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2zreywrpz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2cjwaeuvq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2fkrubqgz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2nyqtbjda.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xjlcbddx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bvovgxet.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qsbrhfrx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yhbhdmds.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2wucciqno.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ysdrhytv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2quwqvqgo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2nnzbhpxx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ifahgezj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2arbwipzy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wuwdckkh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2iumeuucu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eleagshf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2tjttgtrg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2etoskosh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2sbbuyoow.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xdtkqtrc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jqyditve.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2tmyfzari.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2teejgqfq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2mvcbfpfr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2faydwfyl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fzznyiur.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ugaowhud.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hqszsemh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yeeaqpzl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2eimlrncq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2bmvhfyxe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2iewcfvgs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2nyjwfbiq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wnxkspla.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2oghfxrjh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2eqlgdnyi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2pyaqydvl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2enfdaszs.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2bjtpfkls.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2dxorhdld.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ksbjrfnn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2rucugofw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kjrhbugt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2jcinaicn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2czrjsedx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2fdivignu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2khcuggrt.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2fjifntia.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2azvhxnlb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tykicayi.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rzfmvxxh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uzazeief.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mvsqxbct.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2erhrkjpz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rhxqddod.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ldgtfbnj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2jndzvcvg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2klibhtnp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2kaobfumf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2zsvhpdkh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2cqmqeucu.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lftqoupy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2qnmqkrxf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2suokmovr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2pdvtcmzx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2cqoaqioh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2gmzoaneo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mtypuhhu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2iwnqlkuh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ftqzfphd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2aedreiyl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2uszfsuuj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2twdxhgsl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2iqrlqtpq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2reelssra.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ulzpkjtq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qfoztjyw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oobmnidk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ynhynqoq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ihtcfupz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2vuecnhpq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2fdmsqbec.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2yoctstiz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2rfjahuyp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2kdyvfpes.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2opeeapag.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mnsouyqa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ttdlcdru.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mnnvysgi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2rxzzemsl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bymcxscb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2egljqbhi.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ceirgylj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2zrvnhnvx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2eidzksqt.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iorscyed.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xfugqlcy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2yepixxls.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ykqimhfc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yemyvgrp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ndnubyfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnyeyfsi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2gzmeznxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqekfmhl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eozrirdr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2rbjdwruq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2mzwdjjds.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fouytmhw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lslmypuw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2fisllxmn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2zbzwrilx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2twysipps.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wjcfjqzv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2xflupfmy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2keohqrag.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2bnfgzakq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lddngabj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cwkjwhng.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ohpjpbie.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2bqxwbykc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gfpnjyff.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2elfpucnc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qggxopeq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2brneqxjm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nsprsuak.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qvktiajd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2srbyqvmr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wwwyalvt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dnogvomu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2jrbvrgid.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2snqmquri.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ggjvscuq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ugfbwbho.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qcybuevl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2npcdvbyz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ypxuhkgm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xahiasda.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2jfybvclj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wovengpr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bmrctfbe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2djcipnua.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qwytiztw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ssybqlha.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oyqwwyio.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2xnygvojl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uqiaontv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2pkeuruoa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tevbairt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uyajyuej.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2etkxupha.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2udynlebs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2eszacucm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2avligkia.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ttbbjepr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wzfylznf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uhqsxojg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wyxcebwy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wmzrjmgo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2zitwqjxa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2sfsxqpby.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vutbxful.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2jhfgouli.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ljtedfsv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2cukgagsg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xxqeqtjl.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2vasywkcr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2tkgclsmy.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2zkmvbjki.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2tphjtpih.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2wertlzfa.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vjlhriia.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kirppryi.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pbmjoghl.html


<!-- 参考信息 -->