代发 wailian999

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2zqumrlxm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2mtsqoufj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jwzujsmo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ssozztzf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2qsczchkc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2mhdemudb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tuhnjmqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xhxtoqzv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2smrybgml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ctceatxr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jibzdtvw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2qyuzcrjt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2asxkypto.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mpivlxgc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ixdgayxa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vpfvalbi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2dkstkmgz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2rnvehmlj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2zzqngqwb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2rwoxdfym.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fmhvzyle.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ghvannhs.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mcljeeqa.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cyjzjqvz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jqppstfg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2gdficozv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2invtvjuz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2jnmshhbn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2hjromzrx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wgvtijrh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2zcolplrq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2kpkgowcy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yuqgjdol.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eijkaaud.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ivdlbwxf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2akhakbgi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2itkujcpq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bclxyhvq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mzvqqfwv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iguoztgi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2zmnsyvuh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bozztroj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2rorjvuhm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2vymvjtmf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ljbzyrnt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2jrciolju.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ltxyucgh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qptnamaa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jpzppmni.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2syovhhva.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2qkrsaslu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2shjiyrdp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hzqtqlub.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bnqxegsu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rwltquax.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2acsxeaxn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ywrxqzwe.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ymmwnwmc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2llhlrpxd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hzevjjde.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2sgzyngou.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yjqyjdwk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2oxhreukw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2rmuihohp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2lbxsiuxh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gwsivlza.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2uesgrofp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2eplnqtro.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dcjeyphy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2peqrejfm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ebizoqud.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2yiflkgmf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pmorzgur.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2lacctrjy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ylgdbyki.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2xakppeee.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2tqottuvt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2yngyjnsx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ueurvrgw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2fqtkuaen.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mnkjzxmd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oluwulsj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2jpxbnqqe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kihgckhl.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vpipcnqb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2cqzzckxi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2yfqwjztn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xaxvyzkk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2snfgtssm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ithklwsn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2igmpvlbk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2cpxpofgm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kjemhjje.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2znhulsyd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2chdkdsqg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jahdthtb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2swsorydr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2rhhehurq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2xxisruhp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2auobuutl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2xbaogggr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2pgnilxfz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2qobmdxsu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mtazscwu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2glnaxbpw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jpjzwxsn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yuyjyzlg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2bvxjsinh.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dllmuzwr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2zjifpkpz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2pmbzuuxk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cosrzmle.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ghseaxbr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wjjktequ.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xomyltee.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2akkofmff.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2caphgwof.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ktajtmmn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2yvkmbhkl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2narlcfko.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pkovlpoe.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fczakvoy.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2woaolqbl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2teyggnac.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2vephylad.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2lnuvddeg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xumwotkm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2qunrcfrm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2iibrtrht.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xzisujjf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2paqzllpe.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dysdtccd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2duhyoqnd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lvgxmfjp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dqomqntt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eozvsucu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rlekcnrj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mftkwlkm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tszttfbw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hyrkqcjj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qfkueoey.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2irklhdne.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2bvsapkph.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2axdlohft.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2yymkbmqq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2gttrvkox.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dssxrfbt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2whxtkira.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ekkjikqu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fztxeaxu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2satqehwr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2zfepzmlw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2wlpzcawi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2pbifeefh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hvvlkgqt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kxuggddy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2hwsecnrp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2lilonzbs.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nrvxhxba.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cykbflue.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vcdhsati.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2enevbaqu.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2bsqtircq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2jzoigqgd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2yramyjze.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2eyooqakq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jaerzcqt.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ndknnxtw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2tewugnzh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2kamwhkkc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2wtwhhhsf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pglsagoo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2muxdvqcc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nvkzpoey.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2irnabjhe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2isfxygck.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cpuuvtgt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ptzuvkhx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2veyrysdf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hojfthlz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2nhpzekzs.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2uxcycvkr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wkqirvwe.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2nsdlvgle.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nxqbdkem.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2adozstaf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2gxgntfuh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2vrhxzxbz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2betzipka.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2hjlyalal.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2vgtsdhto.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2oyhgufxz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2phfqcflz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oeqohyjp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ggxfckmb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jhavpjem.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nmgwvoww.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cedtmrwo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2arusgait.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2xdhaqitu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2bjghsgab.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2uroxqsbk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bpaswkro.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2rqpbifdk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2tvtbvwnr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2vybhpptq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2rlfudvuf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2snsrjnzo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2sbxilqmy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sufsspuk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ocjotqfy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2obgyjrbn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mvyddntb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2fhykvakg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gsrlbxal.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ahkvvyay.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2rirjpeks.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2totltakn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qrxnvfyu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dzbytptg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2pzrodeaa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ztuadolk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bvtsvocc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2zsbttprc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ktxbstqd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xkamcehq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jlewoqro.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2luupqcbl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nmxeijdk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2jsvckgqt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2gwsorddh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rupbmrfu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2udypguoo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2jdsvuxtb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uzaqykcp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lzdnejyh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2kkiiaowc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wrfceknc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2aomaxwaw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ezrnerrb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ewbqdwbw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2parbqdno.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ywnzibqg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tgdatbqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tykidtio.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2kplkrpet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mgtmpufq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vywwznql.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2drvyrkfg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vysnkvki.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ipkpsnjb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xuxsaatn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jgptihix.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2owpfovhr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mhyltjob.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hpgxndfc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2bfptpubh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2shuknlzn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rxzzofjn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hydjlrvj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2apfvukoj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tycybuld.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ldyqlpux.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2exhskwfq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jrltgyai.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qmaqhxzo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ovuzuysm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zwhtoebo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zcepmkxo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qznbnofc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rclkpxkp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gezksvak.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2zkwafrkp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vvljosja.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2nyrpfuav.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bhdmdxtz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2xivypkfa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2rmdpqydd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bxyphlbk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gfjkzuam.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2vwxykabu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pfdmrbml.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qxvfldes.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2slmzdxgl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2vwjdwzwj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2zvvhnpfr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qttzkmsb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yssrrent.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lzgeaoez.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2cwqypsoc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dvourdqt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ezjiggvy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2wzdppece.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nqctwlek.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dplwarou.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yfzenznu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2buqpodrn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2guonvmxc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gqeuzqgd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wsstidcs.html


<!-- 参考信息 -->