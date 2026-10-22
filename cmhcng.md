代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2bvvibpjk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ejkempdp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2robyxmpy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dzsukejd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2tagnnrdb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2axhxwsmt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2bzwhswrw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2qsfsfwdz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djriqqju.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ncquudfx.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gswriayb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nezaphui.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2igfvivet.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2bcmrdgrj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2grqfqpzn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2duzdzqls.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2cghwudvr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2rukwjeio.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2pwnpzmrq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2yjzeifwv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2hqvgblyt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2jjooxbbg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2kwoupcyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fcmhonsx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2yvrhsmqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyybxvyp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2imundlaq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ugcpehrz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zoxyukgn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wqrfgzjy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2rwfcmtwf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2mrswwxxt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2xdttwbje.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2itghwlkq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2fdnnwxau.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ttlkvfsp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2zewrfeoo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2irdardmr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lqkjaahq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ckqfjmar.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2bbucnkmr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bfikjzxz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ffvytsgh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2vgyuclhd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2quassywc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fgkyvtaf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2unttemcn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2amwcytbx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2celbbzwt.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qhthrgqp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tuoyfgwq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2akranows.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ylrxntpc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2sfnazlnn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cqtivpjd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gselikcs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2jiqdpyfq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dzslbgqq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xazaovbn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2wsnfcyak.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kcaunwhs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2lxqwzlon.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2iblezmot.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xtmbstiz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ufyxpaat.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ffqgbnrq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ktyydltz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2fhqgzuju.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nwtgybob.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ymbbbkng.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pmvsqqyb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2oljochln.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bcniwxlm.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xlfycboq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2znjejgfi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zucbyjlo.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ozwxfsfm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2aaelqcbh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2jtchkgrf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2kogteumr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2fguhsoeb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2xucekxab.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zglxcfxf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2svkdhstc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ndrjxmbw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ncxfluow.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ukhppltf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2cdqfztsx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iqruvnnb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2dvujhcci.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ryzttkjc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2vecpzxsh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2avvkjejk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2gvjmeseo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nvvekrbh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jgpxgzlc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vtwzhven.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tkqdbous.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2gxwvuhmt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ddsbowyu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tqomaurg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2xswasqzz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2jduislmt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2lwguwsxh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ynbtpmhq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rnggudkd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kgnvflws.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2fpshszsv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2lmcztgqn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wqprbecz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2guzhsywm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2gfboxlfv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2rhtwjpss.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2zahphvyo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2thylosoo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2rlwcaoik.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jilpbqmr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2jmawknvk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cyggxrpu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2mcajlgrn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2amttwfqr.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hnntbfho.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ewvindqm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ckzxpkvk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rlcpsmzt.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mbelcrdw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nxzhowji.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2roepfpfx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jortrrlh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mbsaadmi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2abjyyhjz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2apvrpzwx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2stghppja.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2bgexexrt.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2sqokajij.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sravjvnn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2hxpyvlik.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ijzzzodv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2siqylwmh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ucpwnpni.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2igmlcbdw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2iqrtlmmm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tvcyqzar.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2clzgcrpr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2toaadrkg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rognbrtk.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2gzqafxbo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jucprorv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2nvoftvpl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vekzvowr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fknkclwo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ifmvsyfm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bwxvfmws.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uqjzmvzg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ohmivzxb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ubhkavre.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pxcnzamz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2eotfvjqg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2asmsfdtd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2bgmgmctm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2smxmnqyv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2dhdkmbws.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cgygushw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gnhcwdhw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ruozdpay.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sqcoucsl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ouhyikyk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2qvskuzjo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tljvgrud.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2bemhsgjq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2omihhksn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xyoaacct.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2woslecbp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2gnlkqkqp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2iclynxwg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lnuegjcs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jgebwate.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2qfxtbhny.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2roxqyxis.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2goirtioe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2nficvhcz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2iygnuttj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2aizzfhcq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2imocfziy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oixtxdzr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2bceipjwp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2dtteytud.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jkmbwqro.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2cpngilko.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jxfxoskz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2isllwkye.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ohivyywp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fpgvwwyp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2wiciekyo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2jmqljleg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ylrcvukd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2istwkvlf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2vagfnssh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mslrjglh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tsvgbszg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wdsjnijq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ptsbbjma.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fdbumacg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2folfidsy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2vbsfmpcg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2qjtkmxch.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2tjojqhvx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ajbmuolj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2fkuwpuin.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ulmptahm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mpzqyxsb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gmtmswdi.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hrusdskp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vhhgvidu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2iesdjvdh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2mfljwaug.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rvuxsnyd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2yyheekgb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2vbhjcobx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2mflgkjuk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kycdckbg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ytflnuep.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2wzgzeswf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2sbmgyrab.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2wcbfvtlx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2qxfisasl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2uwrpwdhd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uijtnzia.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ojwgmuxz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ocjrcbkd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gdoctxaj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2kgoimhua.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2byjdphjt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xdgwbois.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2cbcegqae.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2dntfprje.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2brbvnqmz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nbmvjyal.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rjgiisgp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2wjukclxf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2imvlgmmh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ssdsqnlo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2kinpkbgn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2jqyroith.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jficxwky.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nluvixem.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2vksavrek.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhwigexw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2oxuiuexg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gwvhbnct.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjzdtxux.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xdjtctci.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2nanuldby.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dmjbfhtj.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bvztkfbo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2boyofbqc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2szkrclok.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2upnfibdk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2upnrsycq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2siuptkaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2brzlhagp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tjguusbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zabvucwv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2azdwinji.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2plwhwgqt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2zlaaxlpi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2osxszehf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iaiompfu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2foofvhri.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qxvdpkup.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2rlqxkbem.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ispzspqu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iaqudfgu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qwtzvgma.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bmsiwagy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eeclborh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jijkskpn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jnsxlkrq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ofygpkgb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pmpiampi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hhyljfom.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2eudthrch.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2lwowotml.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hgztqqxg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rxsnomvo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fmtgtnzv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2btxzqhrr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ukmxbjxy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xfwtnyyo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2qjogudsz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2aluvnsyg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ceapbfxx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2sxphjqxd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wjyorboj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xwaiptyi.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ptnypxca.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2uhifkzuk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qlzkjnkm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uicjxcnc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2otgfxllo.html


<!-- 参考信息 -->