代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ciwhabjx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wqshszcb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fpqkeswr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2lzmoihbf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ozsooqsc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2hxlnoalc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2euqmnncc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2krzxesjl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dezbywgc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zvmachtn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ceesvagj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jlcqlnjf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zylplxvt.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hxjcybgd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2cejoyspo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zaxloreh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2kkotkcwz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2sfrfztjl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2cdisjlll.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2shjrckig.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hqmqdlho.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jdockrep.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vjajmqpl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2kjmtzuup.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qqjlqxab.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rjcvfade.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nqhlgcat.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wuulivfa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2jkxxvhmh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2oktbcize.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zibuxevo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ponzeduv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2zhofwfkj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ecbgbmzj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2blaqpznq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2krjfrjsx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bbzlmgww.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2urmrqoiv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2jxhvgmzb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2rcpyvegs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rufgswcq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ikpsghbv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2brqhrryq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2shuknlus.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2awvvynhq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2aftvhtzr.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2afpobezy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2taxjzppt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2txcksotu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gjayprxn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wyjdufxo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2trpbdyce.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2grmnebur.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2hjoglmji.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2odzwenlc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uiqvwgcr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fdpdvqpx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gkmucxsi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ernxwzjg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2cfjmzwem.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rojmsjob.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2efepvsem.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gdbnraee.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2kxnaptoe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ommehgya.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2njopfuhu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wjxwogjj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2wzbwjfud.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2bqwzezkg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sfqexyvn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ordupnes.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2imanwjky.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2bvlorerg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2lqzlueae.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2qhucsxcw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ydlqnpkz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2utmrfuuq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nuqocyoh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2khpscfyc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2lmvxladq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gdmyblvz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sijzhuwn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2adjcymcx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2haqxbngm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ulqlolht.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2xoggyjns.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pyftqmgj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2kbgggawf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2kcbciqft.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ocmatkup.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2drmiciuh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2aoavjvhu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2iltpufag.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2tejwgawm.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cldobghy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2xxbuotjm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2oeqklktx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2cuanqsxd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xtutlzui.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2klejjkyu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fmhvdnon.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tpxfckde.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2pviegupx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqwobrpc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2emnmfwvd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2wdjzhenk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2tdsedjkc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ytifzxyb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ldjmennt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cwjgxvrh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bmklxxra.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2zdgjvpcp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2rqoexwtu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ncvktdvd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tpyfwwsp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ljgdbihz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2anwuhkrf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xiptrjqe.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jzjxqjyq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kvrxkvwt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2nbqqfryk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ijljqcdu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tmgbmyuk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lsowgbgf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2bkilzcqz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2frxxaslf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2fpmyegqi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2eagkvdzn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ptnunwlu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2yfmudhtk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2krndrotb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2rjksukei.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2znhkztqe.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2gkmnohfh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yijfuwez.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qkwukzmx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vfcjyozi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ppmepnza.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2xrulgdxu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2yirycsjt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jfhhwueg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2macyimon.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2aysjdwdf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tqehnxqk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ynblwshw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2hhglqywr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nnhbwwmw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2puqdetoa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2habjsnig.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2iddecygh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vgkzqixc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2snjjsmgb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zkbsoirm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2fgdhcxmh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2aapgqvxo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2gpaiuese.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fdueskiw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xfqkdcsr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2czsgtpuf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dizukvzd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2smqctaez.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ifcdbfes.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2qdlvdqyf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2amlejluj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2eduzmtxh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2vjqnfbsg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ifvpwhuz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2adqzihxe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2hljqpftf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2fdbtaebn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2tmvprmlv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2vqloetzn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pvklpvqm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zgcxuepc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2iwcctdrp.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2pcgfzajb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2gqskxwiw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2irtnpaut.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ppygcmuj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2xxrxwphw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2iimbyvjx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wmzmcydu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dsbaqehl.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2derxseaw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cgtqkvsg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fhvwefdc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wevzsdve.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2weuuawsv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2rgtvbvjx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2neqiagmb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zzonhyoq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2losekxpd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ybpqtspm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ufghxicg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2skydnhdb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pcoaqahy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2dowwxuvt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nfnhxzoa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2tjfajevx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xblknvin.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zxskajgv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2lybngjok.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ayaehwnu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2opfrfozi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2uzviegcv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2cvcrmnwv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ydrkjwju.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2pmrcmwxt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lwkadudd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2adtagysr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rnzlzpqa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qzorjzdl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hhgtqzai.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2eapzmcpv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2wsehwvbq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2endszojf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jkxzgylh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2jbpenrbh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2wsguusik.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ykpsoled.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2vthfpvgn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2irbanuyh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fmxdwujz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2pfgrpszc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2dngyqpbn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2baqmiefi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bgprccyt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kledrgzb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hiakaqoo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2florlchr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ajhxmukn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ciatlqej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nztdjbvb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2vesiqeee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxilbqkm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eaehzcdh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2uvuwgpan.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2imrygfdm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fmrtgfqb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cxjoutkp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jyftaiuh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2oouqjixr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2nrznkrle.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xnmfkjcz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zyxqmcao.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2oqwsqxay.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2cuokkdxe.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yryobsbi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2skvflsjg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hrvzyjge.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2vmxqoadn.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jzxjwxkh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2huudsomg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xydofnza.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2mfjkebrw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2usxjrdup.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lygrxehk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mtqxpaoe.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bruljvvi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ibafpmcl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ndcfgupq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ayrcppep.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2csgdzkvi.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qrjxxkgh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jsowebtg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2wbkjfidn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2efovydss.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2twfbjxzz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2yernpaoj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hcikvysn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wcgttgiz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2smurnefn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2yzburvng.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jjvghuhh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wfhbyhot.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2utvgwxiu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2npgzegzh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2utecuzxn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2rxlxznme.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2htrrxpdh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2hafyaypq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ifdrmgzm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2hspwnywq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dvdsslmk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bgrklsuf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2clbzprhh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tmcdocsa.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lzufpvqy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qpoibdyb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2wxyunbmq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qnlshlbg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pgtzjyvj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2swhcognk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2fidlbnij.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2sddxkbkq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2evdojmoo.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2izlkemgv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2bqbbnzib.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2duiublfu.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2yynsuoal.html


<!-- 参考信息 -->