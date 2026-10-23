代发 wailian999

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3omrrlgcb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3spinprtx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3afsrhlpr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vttpvsia.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3hzloprbo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3voapizwo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3usdsdwzt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3brnkyckr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ijwvntba.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mhowvyav.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3wvntclmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmjeqctq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3idfxrufb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgjyblzw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yhcndyhx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3pxcoloms.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gxnnhqdo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ypymtjhn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3papqxhis.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3jphmddpz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ldbsbwve.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3iylrjtks.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3xwapobtt.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3pozejuqq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3xeeymsib.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sogwgygx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oztrjieg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fncdrksi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3mntbzlsy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dewumauf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3urwbqiie.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gldgdxoz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bhufyjdf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3akmsydsr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3nzpcfkik.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3uicqyhrb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3petnqsxk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rkdyunjs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3tcbhbsfy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fdfjcdpx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hcxsfgyt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tjwiovzi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3octkunjq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dnvmzvml.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3vdssonpl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3yqxrblag.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gtcmpxmd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3darwlzau.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yntzsxtg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3gytqwycy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3fzhunszm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lyyiuahq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hqzdusph.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pqkxkmcr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3uhzvtney.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ebhldayc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dixaivex.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dmzrfbti.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wfnawcdc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ilttwobd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dccnuztk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mggcvebi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mzsaatig.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wpspytoq.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3nfhluloi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3detznszs.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3fetseybp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3uocjiokz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vhtbljpf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3hwelpaqi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sdotnxqm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3sfptmscj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gcxfguvb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3acwskhaf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3pdyncpze.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3srujuecr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xapvodmk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3bzecijgh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3oqiwscpa.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3utllzqaj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3lvotvjya.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3fsnooiyz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3jdxihpei.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3wspmupmi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kovwknic.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tszhcvrv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3bhkrsvus.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wanicgva.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3rjdquahx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3gfyknzij.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3tajkyyth.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3bcvepglu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ivrgpgpu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3brsjdyoy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3uyslcgez.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3vqyzvclk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3bkczanbp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hedwpsdg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ckdbhxyd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3amatlucn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3byfywxws.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3bimhxfcf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3antpexvv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3zvrnchxm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3vuhrwitq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3mxgxrxsm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3uzvvuldp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3phtmckik.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3jupfcaxs.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qkfasrnl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ignqpxex.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3izmyduur.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3dkpcwhsn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3qdhdnffl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3tqsvdbhr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aksvaiej.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gcrvwhdg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zrrtmtqp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ubaqsnhm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sgqvyokd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vjyzfeey.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3spgksajx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3xcghyhyf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3naqrnfdg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ivxiopiv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wkodcebp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xppjaxkl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ekpdiaof.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3tksphhst.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3nfbgcmyj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oraekbdc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3opkxmskq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hyfqkyfb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3huuwbvmf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ovhnanel.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pihrnzzo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3pvpnggvx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3aykrellz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ikgnjbfe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qtvocgbn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3czioiiwn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eplrknxa.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3rpjmuqjt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pmlndbik.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mhmlzkkn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3dewjixzj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3rynxnxpt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3thmxiilw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3vgjblgjr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3hkdnbaxa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zryoardh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zldmgrow.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jyogoppy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3uwwaptza.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3rdrecppr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3oiufgvod.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bmtvvcib.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ehvhysfm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3evuxrqak.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vpkbrrgw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eirvvaxd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3kbohfziv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3graahkww.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3invhugot.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tjgswkmn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xyjlzpdx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ghfvmkfk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3wextclqn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3msedpxhf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xwhfsyqd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3kjczpvuo.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3bbnjpqwb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zensnpvt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3gzgmienh.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3yfzpaubs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oaherzod.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3dqumcfsy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfoiopub.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3phuiwzmb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3vsxjfkpc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mmxhhffi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qsxqsqiw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3dbnqblfr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3hfgkzvbi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3nnlwytmh.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3tgqndjvi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3kfqpzirx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3httiyprd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3knhbzhyo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yonrwniv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3sfwgevhu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3slnzfxqw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ufcoqedr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3nbfafywe.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3lxjxsokj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ftoftzqd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3hlnfosns.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojmxoixq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fobalthg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ctlgykie.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvsphvlr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lupecujz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xlqmgvgc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3iymrvudj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ishnjvve.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3hjigutui.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cdkoowkm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3dxawzzex.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wmoyhdix.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3txsuvdih.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3kpvspoha.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3tedmmxro.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3rbvrgyzs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rvpvqjxe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sofdvozv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3feplmyte.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3eseznwxa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3bpygzthw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qbqvotuk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3nbjhdaau.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3cqkgkmlu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3atzzzaza.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3raydqfbj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ysxcnaob.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3nmocuvys.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3meyewtog.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rjwrgwkh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3oiwwncae.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nmebzfmh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3wxtbqavz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vvgydqmz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rmydumfu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3forittyg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rjluirbv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vwnflzgx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nixfqebt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ebhrjwmk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ryirkclp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uznjhigz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ecavetza.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3tssrjxwp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mczuvnpv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3akqtiyry.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jelkpeew.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mumyvpxe.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dfrqftra.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zlgoulzu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ddtotpqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjlhsnog.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3hfkzexts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wbvwzrul.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ogochfik.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3fzbjhsit.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ljdsqpmc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dignialb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rqafdodt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3kazxnpps.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3cuvwcdyx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3woisrrkz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fxpoejwm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yebzrfip.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tiexfojd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3psicojfe.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3natouyie.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ninzvffn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tfyovfdo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rldnhhiw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3sbzdpktj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3htccfqug.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vfssueel.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3jnzrrjqw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iehjpywk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jllbndev.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gknnpfic.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sqnmkevh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ezvwrnrz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3alkvuhhu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tyzrjdxc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3kdlrqwwu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3epjwatdv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3aqhhqyle.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bvbizkyd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zckvwsca.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xgazejki.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3njlaoonj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xaqkahvm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mubcysey.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3aotojywc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xpdasmug.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3mzelwtyo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cyfmjlhh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3xzdzjdru.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hxjpthvp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3tbvjehmp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3isdfrujt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hfffrzpf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ktexxjkz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kwxysaqt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3frhggnjf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wmnkpunx.html


<!-- 参考信息 -->