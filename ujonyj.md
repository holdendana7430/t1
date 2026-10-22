代发 wailian999

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2kdgjkifu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qdxgxvdl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hcyhhkua.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zjrnfoyp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2xtbxfbnd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ahgigqoh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2wlvjfkns.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2dfeytcva.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ivftlmyf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2tspffinl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxlqswzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzcvuune.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2vbebztqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxxiidgx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xcbwayho.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2zulirhcx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tcxpdcrj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pjbyhuwj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xcitrfio.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2gaftpzrl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2zuvbsddw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2hivcavpz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2crkvgzdt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2wcduynho.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2gxtwntla.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jfqrmlwt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xphshfmp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tzmwiksc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2cetzrwrs.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2cbmkdmmr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2aztvatfu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wvwgoiqs.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xxzpmaog.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vytcilwt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rninrwbe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2qvezohkl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gkqpnxvm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2juxxmwmm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ikjabzhi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2borvwubc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zeiwmfvm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yuqcrbey.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mhmzznsu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ekcdbzbx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kbuisfqm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2steayypo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2wderwzfb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2pigdfsez.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xnpsmzvq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vrixfymd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2lwtyzlvb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2aesivqzk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2iuxajyou.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2oiwzxkbf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2pvjkwmme.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2pwzygbpn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ifrryqaz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ozcxatig.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fgxcfjee.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mudmlvkb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sakmrpkg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jnvbyvlp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2deegzptv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dsofddbr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hqiiiccs.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bulvvegt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2nrziyimx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2bugsjmse.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2bifkmlbg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xbyutbty.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kgeefxdi.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2crlerqam.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gxtdblsx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jmtofgop.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2lyujtlov.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2krkqdinj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2akbhtvtl.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jfkavqqf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2fpodwqog.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2hwleczmu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2zercphtt.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2crfeopgo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qfpdzpmw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2zteywcld.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rijdzyda.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ltfqwrme.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2lrmuwwcz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jfgjhkhg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nkwcznfc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2miqxxpjw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2nvqfcdtt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2wpocvoul.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ohwdfvcf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kuxiiopn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gpilmdot.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2mcztiqwv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jmelhxgd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bwzwwilm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jjyafxyj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2pgicfctk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2mdfdikne.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2lhhyovet.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2fsqlftcs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2sldehyyt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2jxqutell.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2fswsjlsf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2uzhrioxq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2oexcytgl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mggdxlch.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qvzvgdhn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2kcrzlvrf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2bnpsjtht.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zklwcnqw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2zvwozldw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2aqbiwpph.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qsiqqcxe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nslvokmx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vszjwxji.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2apzfsgwj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nzigmyll.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kyshfrdh.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2fcpuwanb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vyaompco.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2qmyzjblz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2rwivtvax.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2avieqrdm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sivhldou.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gfhoxojn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2zbkkzntd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ugxytlby.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wmdxykhs.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2rczluurc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eqfodljk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pjbdjnak.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2edmkccts.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ilcefmil.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fmamhxce.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vjchjyei.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2velyyqlx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gwivvrib.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2utcddqlg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ndvqbhpd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pydjuumj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2irzbkrld.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2isaavjhd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2bjvkzpts.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2dlvoqzsp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2wckjvbbv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ktqfbxvj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2nttybwql.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eygtoclj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uuhhuyrk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yldabxfs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2semqitgj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2zxthczqt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2flrmpbes.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2knhbmnlv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2xbnjrshg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wqqeornq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fjtxwite.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ffiamvnp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ocwhqdrb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wdyinhxk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ahvyyokq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hvhwcpfi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2hhwvqqjq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2eriinwyr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2tmjynfka.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2mhnnazmp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2dyojudzk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jjbzdpye.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2fglwqirs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wialapxh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2zcudecqx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2yhfdkzoi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gavwvzyh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2bwqlgsvq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nonudsrp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2juiumqjq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2zunvvsmn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2oaozvryb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2zhmxmrya.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2xnkiergq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2nfrxxyzd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vsesomut.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lvirnfen.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2moarjcpy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2thklpbdk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zeocxecw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vpyimhhm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2zpipxqpn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yufmxdcm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2dhzovxuf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2dcsfjbpu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gymgiodv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jlvxvvlu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2cpzslsrp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfrwwkmg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bezhkddb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aviaxadc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qtjysyhe.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2oiplmzvu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2anwevqce.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2rzeejzar.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ipfyjsmb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2lnopbqzj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xecylyxu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2izvypecw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2acypugxc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rtoaywka.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2kahvdmty.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ibgbadaf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2anxdgvgk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2svukhevj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2goypygos.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2byoqwqkl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2kbfnvkor.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2hztlrfbh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hycrbyuv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2jdavtmjr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzsbxsxu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2gkegdzfz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dbumsveq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2opumlfpb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2gfoxprtg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aliyqrkx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ktwfksle.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2tqbrsgar.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pelxayuj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2bkipkdyw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jhwqyhsa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2wwisjjay.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dzwtmuvq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2xmzfkgib.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2buqptdbo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmwykaeg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ucuogeva.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2raqnvyeb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iprjrwus.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nmvgvust.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tlhdviui.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kysrgjzi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2sndynpia.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bsyddget.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fligczau.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2kfjjadjc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2squhmabm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bfgzgizg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvnsnpah.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2vvlqzges.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2puiajzji.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zcjdtfpo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2gqzxaist.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2gqrxguxv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mjbpvtix.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2axvbygse.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2gcrgizmu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mrfbumgr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2exoovtsv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mpepwnkl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zeacbsll.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2owhavnyg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ymxnrhxe.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uxlpwpkw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dvubkfcr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hvkcdmic.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2rjoljvbv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tqzdaytw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2alwqsbiz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pthgycxs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2npoubfhe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cncfrrfe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xsxyutsq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oxwitoyx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gmiybkng.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vnufbvam.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2trrvzzzn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kivcemnn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2pizxwhvo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rdgsxtas.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2utfrgewh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2djwuhghv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2piaodgcy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kcmydfqo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2hxnvazkz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dwerjwuf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nriakjzq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2zegiboyv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2uenzgwzr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2mdiztmgp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tpfqrsvc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zlinnppz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qvpgueqc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2gaqnhucm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2lxoawxeh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vcgbfsgh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2omjdkgzp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vvmcbsbm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xqtvocvu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ihibmtec.html


<!-- 参考信息 -->