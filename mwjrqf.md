代发 wailian999

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2lftoezob.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mjfrmuwz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2nulzojht.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wzxbteyr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ibnolliu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2mcggxaun.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zwaxavjc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2yolqpnsp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2sautbivj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2gyplhayp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2thpkdhsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uyvoukpw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2gunptraa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eyaiyzhq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ahdmpojt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2oobtbmhj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zouwlljb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qtpemnyx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2riigdhlc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wvhalniz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2dcfjkmgm.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tandbirf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2filyqihn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2tbcswfnx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2futqussx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2tjwwwivi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2drxetttu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vpyuzgfo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2jufkkxgj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2lwxfsojq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2dnuugocm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2wjqxkqna.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2eglwgtzg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2hmuyelld.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2czmtnjwl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2owhdjjtl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sdpfssqb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2incxluzp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pmcaqctu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2lpkmwumv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sjfvhcdh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xtgusrjk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2uauunhra.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eldweahm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2vkacizxz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2gvvcpcdd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hjciqrkp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2oqzlonbr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ttznaqsa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2uvdwprup.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xdvzdukm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2daiwiwom.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tbbsoimn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bstgmlpw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mhftmfva.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2chbbvbcy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ncbttpwh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rvcvayly.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yufmuocq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2sbdnmdlb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gwnafutf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zlyoxaom.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jdyhupvy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ehvdhiem.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2cmdnobhn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ouufbuji.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ifvgxjcu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2sdnrqmng.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2jrvhiaia.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2fyabhxnj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2uxmualuu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qgbggskk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yzcruhpv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sivzjgrf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2mxnapsxy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2jsfjoiww.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cxdzkqee.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2tsopeehn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bdgcjsvr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2imgsjpxt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2fncvbixe.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2twjtdisj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2csjlmxiw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2yxaxqezd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2nbvoeccl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bidfzkpm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2aibstvnz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2etyejrrw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2rgtbxuig.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2emtcyxcj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2bgpddwfa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2otlzymfv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qakwztrz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2acsfiabf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2oiyrroed.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2vaojdfbn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vosxoqju.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kkyowtbn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kivklnbf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fysfilxx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rlysdcqe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2kithwznk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2sltflcci.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ivslmbtv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2sdrhaaor.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2svrzkuoy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2bszcggtx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2crmstrja.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2yvzgnxbi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2liidopgw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iyyswlhj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xhvpppid.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uhvsfpli.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2fnfonszw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2vrlscdlj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2otnzxzzi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2egrxzxkt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2piuqlixw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2eoueavah.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lexmuzxo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wfweppor.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2bghguwvo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2oejozjqs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2pwobzpuo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2mxkzeznw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ofhewgbl.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qazivoti.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tytkougv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2oitrsdct.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2vloxopsh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2patkijpl.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2uodljjia.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2nyeczeuz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2shlrdvar.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2szysrwvn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vxvojifi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ewzauwlh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zrhszzpu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zarkhqaj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2appscblc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2aqvxcqew.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2nxpvqqpj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bhxdgivg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2imdpfwsy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mvedvwju.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2iksnipaa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rxnjufpg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2gmffmgag.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2svcibxux.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2cnhnrhpg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ttebcxnk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cszccxbp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tbxmokpl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qxhueqin.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2imletqhg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2kjxrvbth.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kzipnutt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2oxzrdtdy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2lcnrsevk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dgphujua.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2plfguyuh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bhhuzcqj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rntsztqa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2isskweun.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2azfwefsw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2qaofgkfg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2exzrsyht.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2vdjijpvs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2tfpnmzbp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2uzajwwep.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2kfqorusi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2tkwbpzpl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2orvjwxrk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2zglvdqca.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2veoanidp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ctppvcpj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2wzrydxfe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sdywcznj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2nlwvzvzm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2atlsjyuk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2oaakhyxt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2itesmkvi.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2lchtgujl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2dzacitjb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vqmsgywl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2sysfevza.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2pfcdgcsx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tqijfdss.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ecxxtapu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lkkjmial.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2csohdiri.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yxgnnaxz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tmdjskjq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ywgumpta.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2dwtmbnpr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hsznxjck.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2uxwryskq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2whqarbje.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gscapomh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kspwikgm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2owjptftu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mhrsiees.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ssxpqbpb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2eydskrsx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2wxbjltnx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jwtgadlb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hmwznfaa.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2mvputaaf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2gzbqgtdm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fugoozgm.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2nzzfxeec.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2toldztwq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2peqvdrlx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2hprkxfwh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2rytdsjci.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wjnfllvn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ndsrqcdu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2chaowklh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2stlkqipn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2lytzdvaw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ytoiincv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2klsneaax.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2tipzjvgz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2rcbepgzm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wizxjvjg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2whqujopl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zzqqwrnq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2byqohlnx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ncmneebz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2vexjyxmb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2yjwvaxcr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2jakbtpvw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2iwgqovcg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2vwarrwug.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xacxwaqj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2slkgazau.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2cmohjlcb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2birtxwko.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wmxqbkqv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2gjrdyqma.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uyegsoei.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ttlyzfxc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2snsswihd.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tbqoxtbu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kpyoprfr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2yszmlfbh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jzsaydoo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2evcstddu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fatnynnz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2emuuhuhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvnqmyls.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2adlnfvtp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2svnaawih.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mvmhuiwl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ixgaoufz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yszjvioo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2qvaxxeng.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rtmbbshc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2pvyclbrq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wjpnlrng.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ymilyiqm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dtpefxrx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dwbdikne.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tmiotapr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cpzoarwd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxpteos.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2adzhwrqk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hdpytqow.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mgitdzje.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sixibcrr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2iqwuvkhd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bogeullh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2doxpykoy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gtueggzu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2njfxxafl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hvldumgf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2pdcghxol.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2szcorvzf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ckpempmv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zsbjctcu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2hajvnanm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wmzqrizd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tmpktvmq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2salxapgc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2yrvjcmoh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2llmmobpa.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hpjzhufe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ehpioorz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ziribqmg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jjagarrv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kufcvild.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qbgmipoi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rtlmhbwl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ehsdwpjp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2dkfqmohg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zrehgssq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2nplnokxm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cidnvnjz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2avsldlzp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wpsovfmk.html


<!-- 参考信息 -->