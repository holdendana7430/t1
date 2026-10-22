代发 wailian999

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2tppzqrma.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2zxbfftgy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2vgxnbtyr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2vkvkhuou.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2vfxadhuo.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2bipqnsdy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2lhmmofxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqotavwf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2idelevul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlyxawvj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2mdvsvwwf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2eudcydjp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tfbbabyo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ujcbnpsu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2zhmhsati.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2lyxccmkr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2uvvuusib.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jkmkrrac.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2cqmjhgcl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2lgywgyme.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2npcqlkrh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qcfrmceq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rfmggyws.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qrlboyon.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2vpvgjwen.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aotybvah.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ltapcnek.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2dejtrsyj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2rbsanmfj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2tsvzsgac.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wvdvmqkn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2vuwnkxci.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2toudsibj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2muygoasf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2anodlaym.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2yxdqprmm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2awtytcak.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wpaxnjox.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uzdnevej.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2lxknnsur.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2sgpzwdtv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2wivlyjqs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ygpseeab.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2fsbifwoz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dvfoqorc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2iscyvvmc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2myecpeph.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2eaylekgt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vfuxvwug.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kbfzpzwt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2qqigfrhp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2gdhasvsu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xkcjalbj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lrnzayvd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mfxrbhdu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mktuzghg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wbdcphin.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vjmkebhz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2brafkesb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2oppvmlmu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2rdfervck.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2seejqxfk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tvnldqqx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2plphouhg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2mbziahkm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2chekjicq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mjdnviyp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dgqpydcs.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lksailot.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xhfuufpe.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jgyosobo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dszmfeta.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ialzsbpj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2yfawftkw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2wastqmkl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jltgasqy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2svvfdmty.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2tsmmnxbi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pccaoapv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2wmdufpqw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qswbywiw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gginpgqt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zmtaujcz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hivexavt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qczstkgj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2btysqifx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2vnvmvpee.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2miprjapl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hmikevah.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2anruqkbk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2jxeypiqz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2xnsaxdyd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qemjhptj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hpsyuemv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kfdrjpqh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rtrrmekm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2pvghwekx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ijlqwmhm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2hbpfrxls.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2onwvlrca.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2rlvqbosy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2hqikpahb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2cpmspryf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2xsxodgei.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ywteodpk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vizcynky.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2sdynscuy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gnllbgsa.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2gvtiaczj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2yscllzqm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ohpdkuzz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hejskyrv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cpxrozvz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2medqfkcy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2tiktxyqt.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gngfuzrs.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2uqfyrdpp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2einvfqdo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2xuzhlufl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cwvrlhpo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2efqshnwa.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xruffpbs.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2srhbsemz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lgmtmozk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ecwjakxi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2qadzvsll.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mncusspr.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2nbasegkc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ugddurqx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fjvxgkqx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qmsemlhg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2odsncfib.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2vovcxjke.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jxkzpijo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fnyuzwpp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rlkbqgpn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gteioyxz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qyjndtbk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2fsqybnyj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ikznedka.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qmpnflrb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2upvzugvi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2uhgsmtof.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2vwyoiord.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2yncukogq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ufpkfkfd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2phkgxlya.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xlhwgrtl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hsjnijlz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2icqrzuxg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2dfgswzwl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2stqkhocp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2eqdielpy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ucygfifh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2goygwzge.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aiyzadsg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tmfidkrp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2mfbblmub.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2euyjccyg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2julnhbsb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ingvizou.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2culmcefb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zxwzmyph.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2djggvpqb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2sermkiws.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2umlpbbgv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ixtzbjsq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2rntylpmf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2hkideqdt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2idvpjszh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2bnmbkkoa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2opcnbeuc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ismosapy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rzyyqxfv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hqckipro.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2twthihvy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2sqmdrwos.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2dulzyuzh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2gvrgunlv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2swkkxzih.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2wstzivhz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2orcwqqto.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2gmwqxbnf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2tbpawpbd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2myytbuoj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ztjmgdyg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2avjnkvjd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2npgcyxja.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2vlicxipi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vxbjortc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zvoydtwu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2xobqarhh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2npxurrgt.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2csyiqmaq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kfxtdeoe.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fwztmjyk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2redxpoie.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzidukwe.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vzcsomai.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2kdateqob.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ayibngsx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2lmvntick.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2pckufeeg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2iobcsznw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mqxrbyio.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2lylnaywj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2pzuimhfi.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2sqdifdpo.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2zrpodipd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2nxfponqy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zqpzqxhl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ormioksl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aedjrgif.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2nhyiftae.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2orglbgvo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2iexhbuhx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2yhqodwom.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2xnngqcxm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gzksfqyf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2wygnielq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sdbisgli.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jfszmqox.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pjhrfhdv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2pinlrnwn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2djqzowup.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2stppjkes.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2xpihzeyu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2tvcmdngr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2oexgyszc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2asiopdyj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qhlhbyrd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pktcdlvj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2wlluwpua.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yjricvkt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fjyhlkmi.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qqpgezai.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pncxnjfk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jfeuhyqm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lnzgafbz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2znnbnuey.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dpmtooef.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tiahbsfx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pzqpzybe.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ppqlyeia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nmtfynub.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ncmwkoek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2paqfxnrv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vuwptapb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2nubcexwr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2kynylmsi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yacdxdnt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tzlxsqbq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2gzepeirg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2chmvkssn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wkoobsbf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jivucgws.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2jpzxpedk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2elktxuio.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vzpuoqvt.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hrabnhpk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uuovxgnz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2npptcucq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2goryxcdf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gpmpbhce.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dnytervx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fcotkcrv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2gmrrayvp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vheyofds.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vlvzmpfu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vgbpzwrw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jfbvqsfn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ropusfjp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jztoytfs.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2bcwecdmo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ogsnuigt.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2owmiqoge.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2creqdqfb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2bhwfrmks.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gquxsebf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mwrodayl.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2sgllholk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ksmapphy.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jaxvoxoe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ccpqyejv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2xliqqwbb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2zwdgqzqy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yeowinsb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2uoiiukcl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kybyetdl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2atpopmzy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tdnzvbhl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xixgridh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ofsvvazy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wkqztlym.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2whyhwmzh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ywytyftw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uhymzpvl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tluuwfkj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xlicubtm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rzlnzmmb.html


<!-- 参考信息 -->