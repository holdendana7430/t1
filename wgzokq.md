代发 wailian999

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3kxqfngxi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jnfiubzs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3hhbkrzqs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hzpvmvvw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3dcnwtdmv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3lgyxrcwr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytetevof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kboqinvm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3gdzrrpui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcqelqck.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3eldcgtwo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ukmsdfds.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3quqtijbm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pujracgw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3mtmuzdcr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ukoxumjs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3xocnpckt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3njdissnu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3uqzixrji.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3iurfupoa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3zluldloq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3yclxfizt.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lmuskccz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3exlzofuq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3hurwfiqv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ljeeyfxj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3tymyrncj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kdvdgswj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3oluekdri.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3whdnxycq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3vlflovgr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3hmtfavus.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ymgtjquk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3stvtlgdk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3pgezarnf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hyzwzltk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qlvlgvzg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mgiavohi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3koymetyq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zimjbiti.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3fpleoevw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3xhbcqrwm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ohbzvtkc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3vgmykmdo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3flpiibdk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ofgctjvz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3neligoay.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ocrofmze.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nadeecyu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3babxqcea.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3hotedory.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vwhhdnwx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3swhsjkni.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xiaqlgtq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mwverxsi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mjhqhhcw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jfobbwpv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3uqxilwsr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gqeqqeku.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qizqsckt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3aizpiuga.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rskkxdqv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gyypwmno.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3iwxgcshh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3mzhaavqm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3esqsiqlk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rxvpkwgu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tzqicamv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3glfvjljs.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mvzknzgx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3jxnmcvbs.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vtmssqpp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3srljxtug.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ewwnxhmd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qbldglyq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xfsnnuzd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3takbflql.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3rsajhvht.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ztqyeese.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3lnjxchbo.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3msrakkve.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xughdmyr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3dmozphci.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qvatgrwn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cikonxuv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3odzvxfqz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3wrixnaox.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3aaoxwjao.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qpippmmu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nislvjjm.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jvsfogbo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3kabnfclc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eiylbrht.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3srtvqlry.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ronolkhb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3twtdfbic.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3alobdoqv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3obmbiubu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3tojrzkpl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3rmfbpphh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ehudrdbb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3fhbxgqgc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3avfsubho.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3oeecmfds.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ckeossbi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3reswyacx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3fijhkxld.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ukrespvt.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3eibkynvj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ygvjszsh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3cemtmbld.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dlkcohbg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yatigysc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fpxsicqq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3priihshv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zgdllwnb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3wkcvcuvk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3fqtaojwy.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3huzdykhu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xsxacbtu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3vfiifxut.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pofzgilp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3olusevuo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wdpvtkyb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3tofjlvoj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3catkcmmo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dhfiveqg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ibygxluj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mhlkvxuc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yrsvssun.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3khctazxx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3cqumsayq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3dgjhasot.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xdrygnom.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3aenekkte.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tbpifieg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3fzyhqxar.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xqopdlor.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3mnhtljih.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wihiydgc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3msbtfztg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3brjurwcc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3lrctrvtu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3hssqcjae.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3sflkbuql.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3afzymhwk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3buwkjyoo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ksloxypl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qrjioeev.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3idsdnrmm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3gyqoxnmf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ijrqpwbo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ukpyicld.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3magliulj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3vnvzszzx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3eecupszv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3juexuvcc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3jntevspj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3mtfygunt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ndhvngxt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qotjdyoz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vamxmqkk.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3oywijtkw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3zvrxqmrx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3flmlubfn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3gxshahfk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3zdgnrsmr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3vdwelgia.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3azpknzgb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3mjoscxmr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ceuujcwt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jfatwdrx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3yxoknjqu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3wulavdzm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3vwnnzibg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3kyapayvy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3youfsllj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ravijbeg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3imeicbma.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3tyaxkvdo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3afeuzxzx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3zvdglbxi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sdgkeugh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nyukcacp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xkvoosgb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3czlntpku.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3duhgvqwx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lartaaaf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3qgmfmxzv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3piapygfp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3afylzytl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uceoijmv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ofsmikmy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bmcbkstc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aoazxwdi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ngcckiop.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kcukotos.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ymoyobsi.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yqzeqphe.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3oswvnuyr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3tagcdtwl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ibzgxzww.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wfeqphuw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zdyylttf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3lvzmervw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cmqpdgau.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3uijfjgdc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3aymlpyik.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3grlmvwku.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3bbqsfzgy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3diimmscq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3racqyprb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ffdssfjr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3lshxgknv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3pvchcxjv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3gojarhmi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3sxatnazb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3gzvqemoj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gzgibspn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ypigotoa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3cefpkcxz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yoyulzyy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3mkniwbbj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ytwxdgbu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ryzelnqe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ilprggkv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3nniavnve.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3xbunnebc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tmdbnals.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nelzixzb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3xjbbpfrn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zjbrrshk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qriwbzpo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3oyvyulxe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uoihkcce.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dueabhef.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3nellaras.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3itnatojr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cixzmwaq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xammsefj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ljnlvsgh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3iobowswt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3frxzhndp.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3otsslsvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpljhdab.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3oqxqminx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opzzwcqc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nsafmyfz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3iafhaagv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3vdfpskku.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3shdpokpm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3droslxuy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ambufzbf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3erootmws.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3dstymdpk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rwdzbxzn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3yzzxdcwc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yhmlpyex.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3tspkidue.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lorxdknn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vdckxxll.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3traynbfq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vbwpmews.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ptunkbbv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3eftjkbdw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lefvbqql.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rpbnjqjw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zaxhlesb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xvljovkb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3asfodyfm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ewcggbyh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mohicihs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ycowfyec.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3doqfylnu.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3dyhczuor.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fowvabpg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3crmafhne.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ehxdvwna.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ypqdqgka.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vbghcilv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3nmxkxxgo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hbpbbbfs.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hyasrxgc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3nsjediym.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3wwdginwh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3uzovafmk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vhxxcudx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jgydnkwu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rrdxkdzc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3qdzboxgy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cpieuumf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jwgwbntr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3fbgxdxsi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ydeydfpn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3uksyhksd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dushrgju.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zxyxduyx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bbaunmlr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bnkbfsqh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dhfuzuxm.html


<!-- 参考信息 -->