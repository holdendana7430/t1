代发 wailian999

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2dcmmksfb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fpevdyiw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ydgawdlk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmzalkzo.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2qwpemtpc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rqenurzy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsgzhsni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yechlxyo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2kvzknmif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zatbbojr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2izicqcfx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wyfitiqg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dqkzympb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wfjpuhvh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xdyktscl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kvoaibmy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2tgjfxesk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qeqlpjog.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ggtddwbp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2nnsfejhh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qmxgqzzu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dnxxwipp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mhbousyy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lazisowk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2nqzvqwwo.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2bswmwyqm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2hkzlymvy.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lizpbrcj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2oqxxvjme.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jwghaixb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2xxgkeajk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2gigfzcqr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2unlakqov.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2efvxuero.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wumcmebn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2hkpgtqme.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ckhqibkv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ttwezhfo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lhffqmcd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tnnbjhyz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kfqwggux.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2suweeqvt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ewvmndoz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2pobgtmjq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2excjuzct.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2mbtfogjl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2aobkbdza.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2maacyyit.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yuazkhgq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2crzrtlwr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2pudvxejn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2nsvpoucq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lwqvnlyv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dtycadyo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2euxtmwer.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hccsmnzw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ajfzmumr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2skwevngm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2worauvtr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2whspxxfp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2lwfpbmir.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gxadmtor.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pfhiuseq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2zulrgdav.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2oazkhkoy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qvzxgkqs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cuptrzok.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ruerunea.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yfbhjdux.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qddunqly.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ruxqzlyg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2oqjznfhg.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jrpeqser.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2pllzcoqu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ftpwfyow.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2tfycmftu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2zftkftpz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2pjibybsk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vwujhxso.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2nhicutjd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2suautems.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tgpnfavn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2phvalvex.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mkvttdde.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2peqrblfg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2pmhpbwdn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2cgxzpoxb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2hffhdjau.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qocrtyxm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rwxnmyux.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2jrjthxiz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2suaykipx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pxwspoqb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2czzpnkmf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2faybbpor.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tzssfbsc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ifkeyhej.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2tewswiqs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2efcqwblh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vmmfmexo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2qnjqkzcx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2bfomumys.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hhrsddep.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2jstvfmgd.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2nsunncjc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sbibkvho.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zqeewvws.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jqydsqoc.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xpcuwxlv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2jyznbifo.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ypbzgaoy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ntkfvioz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yxmlnufi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2baxjynly.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2vcqhkhuy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2penhgimd.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ewaofsxr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2nzewdvlp.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2lohiescf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2thqxbtkq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uprvgyoy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cjuaqovm.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ggzbjqbm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ghiipurm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2zexfbyxb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2okcedvcw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xywtbrpo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2bxxoczbf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yosnjlxt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qjjtmxzm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zhaebjnn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jhkzvlha.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xckkxsxh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xuzcvjmc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uxqxlvql.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rjooxrlx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2yepincrh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gdyesfhn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2agedlnle.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nsatlwji.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mktqvnfd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jlvgldqc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2uxgmqpqn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hrgmregn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wiokusgr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2yljagazv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mpgnnyaa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ppzvtpwl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2leknwsol.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oibugair.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ozsjkpkx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xgxwwols.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2atdsckfl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2xdxnjrre.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tepyecqk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cijkmxqt.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ceontbjn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mpkibssi.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2yosmoqrx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xgqxcsaj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hgvhdacv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2oriuidtd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2iodlmchq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2yjrqanij.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2dkvfhwtc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2usosoris.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zccebhpu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2nacsflnu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tgmfqwib.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qcflmsbo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xmkpsymo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2onzaglmm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2hmbccbpo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lkdenaec.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2gwnkpyll.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2czorutfe.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nchfupmx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2yvwcfcud.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2tbvtxufi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2cibgmpjt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2jbvcioez.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2lqxzxdux.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2chenbcvw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2fickftje.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2irajzpkk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ganzrtaf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2phsiehgt.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zqfhjtcp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2nywagtdf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2bcfdtuct.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ynkdxkik.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2xvlgrzmw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2nwyulapv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rldnpkzw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kchpwjgy.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fljdfqyw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fjkmbdor.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vfhkskbz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bdeulivq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2enraabne.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dykgtmbb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2tzhxnaex.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cigsiwjd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ebwuyoed.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2uaqycyql.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2oybnuxdt.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2vdqtbuzg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2thkimvqk.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2syaparhb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2lodopiet.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nuyjfblv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ajejudgg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xvgiimwm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2vwjoomez.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ldpmttcu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2lfcmujhn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2colyyycm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2oyrvxpmg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2bdklrcse.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kmfeeyfq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lyyuctpu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2djnuutli.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cuggztev.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2athygpyz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zbdvaoub.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2hzpcdjnj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2xhveckph.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2nkkbydem.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2fszoipvx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2nvwbijzw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ixpacffn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zcawgjqh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2xlhubdey.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2boydqmwp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lmrsyfmk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2yahdtigk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2hzzbvnnw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wpmzoptq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hblmbhtj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2stfhuasy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ludeuohf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2xuorshhh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2krrzpgsy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xijvdhum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcheuxok.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jgmsnyif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhpahyau.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iwbwjnoe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2riyksrqr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2malnlhhe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2llalpaum.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2geqxmasn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ekozfixp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ftnyclik.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2dhnymiaw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2effoqbap.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xldhoyir.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2sxqtktei.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2savepadc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2batwuttp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gpqsfajh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2oqgyelkc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2agyldutn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2patxdlcq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2aschtazj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lzjmhnla.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2vakmcdyb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eapxylsn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2efwfrkbz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wyjyspjl.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zstxpptt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xnavbqmn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qgvknehd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fzolnhio.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2dzopztul.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vscfyvkr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2cwokyezo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2pykmglyl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2djgmvmga.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dhzaxgqt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ypjjsdii.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pbfdvyyj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2aobeecxw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ckwidmyp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qxszkfbn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2xrdyuhnj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lsdbwbia.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yhkzhzif.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eeuuaoio.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zngoqdnw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2merknemm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2viunbohj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2blmcvldq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hxsupisc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2xoufbmgd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xkbeeomb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lzmxrkwp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bwgdsnki.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2flewmcea.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uuczvule.html


<!-- 参考信息 -->