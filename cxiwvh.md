代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3rpndafwa.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3qwhhqusy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ucvlemeu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dexipbjb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cnlqmipb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugsosiek.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kcwvuahm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fjcndbam.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ponlbffp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3srrsdxxv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3huuztovr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mhaoowgk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3jfeptmaw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3dyeexdcq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3lendtajg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdfzoyrb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mmwtyyhp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3dsrijqxq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpdgmfeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzjgttqg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3uixmhgxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hoiiwyye.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kcytidbn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ydvumeri.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3pxedjktk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gnueeygc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3kjraemkm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3dlozbkbz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3qebhyefl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vvsahizj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xrqafghu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3pimlkvdy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qpxposxq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3dycwcxly.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rrknotyo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vbcpepip.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3mweocfxg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tovjelwv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3grcnhfmb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gbbrvhsh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3trjjskct.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3cbxvxquz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3kbomcpmu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bzgyxmjc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bhzaunco.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3djjcfcsx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3wumamxqk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3aeouuzjd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pwvzfzfw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3zetfqnpj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rgnvgrfu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zfmrickb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ogejluvs.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ayphzvpc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3skokfhqa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ekkgaiyv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qhcflcat.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ivfrcfrr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3mdamizkl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fourtzcg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lukomesz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3reqgcydm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3gglmiacj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3bkcnerpk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rvwmfegb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vyrsvxvx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fgftioyd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bhqdximz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rqzueoaf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bjvhseqf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xotuyxqg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zyupisxu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3xmryosrh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wyzahsio.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3drckfrzg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3dpcmpxoe.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3mvnywaaa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3bhgtpfpy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hrxlgsok.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ccxbvgiy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vlpammdx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jhoooubw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3aoytugvi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3rvhbjmsb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rklfvugw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3adisatdy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3huympbrt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tvvolxnh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3gyjyoknz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3zrphuocj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kilgylfa.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3grpcvjgs.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nyllpqvc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ynvgmjhb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3nhmgoioz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tanmdhoz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3yjgytblt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3vrgexasp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3igitbaou.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3mazkbgwv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dffdsoac.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jwinezab.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3bsmsorlg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3lswlyrut.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cxlwbqkw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zrfrqisa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ioenzljf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hbdlpdzc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3yncoxcoq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ccnzhqcl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3wdjavznd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ndbxghuz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3wltetipv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3gloxxvxs.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vtcfupvd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3swfwtqvc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3khsiyuqj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3pvdhsidg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hnzjsxzr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3znpxtfhi.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3swzbtkio.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3jdwzbxmu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ypjbveii.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ztjumbnu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tttkgduf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mpmhvzmf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3emnvliyd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qixptcmo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cinqnuvf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vquraalw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3knogndii.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qeumvfwx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3cnnszjsv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vcnuftff.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ziihkoyk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3komcxike.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3nftfgyon.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3gkdlcaiy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zwvfhqaw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3yshafisy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3fdegywdf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ssvckfpb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rxztknrl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3cjaafigh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3xraiixyd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3rbzhaqld.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sbglgxpy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fudrmyfv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3urbtswuj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gjccstab.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yenxmoqz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qkpqkosm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3tfyevpmy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3gtxntcul.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ohlsnwxd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jpndgnxi.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yrsoyvmv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3zbryuumk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hfktniyb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3chwgkprp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rfpsdclw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mozjtnos.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3tldzjzak.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3zfylipev.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3majcmtzz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3kadhzgyz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vhvezkpu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bzoqofjj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ipobyawf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3icdcphym.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3kclxchvd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3plyvwwvw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mpgoynee.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3itxukuan.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ohjdzopx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jdtdgfhs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3hayqmhav.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3tdmjfugd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3remgyrds.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3tqczdfrs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xzenpxjq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3iakjipaf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3femprxdf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fesgvkul.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3mfguctkt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zghtimvk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3pyhlrsrn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3savyhbti.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hzaqnbqv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3rdmbanni.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3zdigqlbu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3kaestjep.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ddufutgd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ahcmlbtj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3akexecwx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3dloxvcib.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bcsjwmpc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3quozlsvo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ljltmodf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3msigluwy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ffclxfke.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3yhygibuj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3qcdxhrgf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3eshlgjcq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3hqixyiph.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3clwgjgxy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fqiwkfbu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ofrgvxqu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nuxnxfvu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3boboiuxm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfvkswip.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xalknszd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3babmqgty.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3inbpuwzu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bilbdrns.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3wkhastrt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ilsmzxxx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3pgengajg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3azdkwdlv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bkpbvylu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3pdcxktdz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3evbxlakf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ajfmlkyw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3summahxr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gmjnyfdi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3nxqslvmy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wqfitnii.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3wihplwps.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vlwcvkcl.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3necrwfgb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yjrfuhae.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3igpirjrd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3awyeavif.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lapyckql.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ssxfqgsx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3wkqnplye.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3gyojikna.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3vsqjotgv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3aqqftlku.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wxyqbotn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ahrkbkwm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3qppzvqqw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wytgpsec.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ctdojltw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3hzrlzpec.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3nyqzibxf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3duiftswz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qhlzwlbl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3niuufutb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3exuzykmz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nnuhsmok.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pmczrqxv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cjghuqfj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ztocgukj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bdaxpwch.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lvgkdfvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jynziwhd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3cuckwekt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfibhtlb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kfiacvog.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3xkhlavoi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3oagxxcou.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xqzevxqq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qrbfvolc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3fstemggz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wgnyfozv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3gxnnysmg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rvmjknxs.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3kkrafzhh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vijunvmg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zkpzanbn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wirrsuxs.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xaabiyio.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xeoyqbdw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dgdwihec.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vltwatdn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nacmlmof.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mmpptjcj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3qsyderzd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3upngxntd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3osqxriyx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wtflwfie.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3niqtsndf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3aganbbdj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3rjuqivdb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xtdmaxfs.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ctubiceu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nvraacck.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3nrqfubhi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3cyqyjjer.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tqjruibx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tiztnzoo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3dxyaaeul.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fwvwtnka.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zxboedsa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kwtzicgs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tyejjklh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3pgbxcirs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3eyaabgdp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kueyvxob.html


<!-- 参考信息 -->