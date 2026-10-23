代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3evtvwabj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjkdkdnr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3fhsmxmrt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tjxrramf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3jrttbwnb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3chuhwjct.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3fuoesymj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rygzeiau.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrsrvswc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3whejbsxs.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3efeccqgn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qmmychcg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3zavsioky.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jgdikpbb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ocdkbrjw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3wnwaunnw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3xvaujixr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3hvszvstf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3wpnsqdql.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3yscsmdio.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3rgwaeqov.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3gqeqxfkm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3otvfqyub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ypjhipvc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3mfnpotpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aoeihcuz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3anufcglu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3uctzflfn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3vlzaiafj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bmuuzkzp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3donjdrad.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3pezacfwp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3dsmyclwu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jgoorsad.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3cegsnndx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3cfbvofde.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3rqctylnu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qpsgpzfe.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pqdowaci.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mnsgcazg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3tenogkue.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lvdpecrn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3stzaasvd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ifxgebws.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xqyjugka.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qwcbmufv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3pfhabsyn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bpcninxr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kyqqhpfa.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ezhuyskm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3jcxymayd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3vpqjarno.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3uothvyoo.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3amufeqib.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ivwmkmxh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gaxfxwqi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3yhdkseqk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ogyemgma.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3igzjlrde.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3fxhmyaxq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jskvdmvp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3mlcmmtze.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3bdvnzyvg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3eagjuvka.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fxuzvvix.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mxblkmgq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qmfrzend.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3iqmwsuzi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3sjbczzsx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kymjkiwe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ysagfpuo.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dutptykd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3druxlflx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cvqbwqky.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ouzewach.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dcuqwlom.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ehxqdanx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qwytgtty.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3jefhkidi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3smrxrivk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3kkvuzmdk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3gyptmakt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3uowmafgi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3frermilb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hzrpkkhu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zkslbjkf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qjnijkwt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3odlxbxmz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3nvcksrjk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3hsrimfzz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jgmemnmn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3juqcsmip.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3yzzcyudn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3suunsldr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jrxcbzpb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qhiqqecp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3vckbuicx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jplwdtyi.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3lgqdtbeq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3drlgfjys.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tweckhia.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ywaofcms.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ayriqihh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3wevcsqda.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cujpteit.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fpswlsdw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3afbqusfc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3hgbpxvxx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ltlyxocl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kehprxqj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3togkukax.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3emaqpsdr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3dzxofxjc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3atolqqst.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3owvroehh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3uuojllwx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3qjtaanzc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3enqvhyjq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3wiokxsgq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3omprwqlz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3dghlwple.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3giaepxrv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wytbaxam.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3dhlhrhqo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wqoexuhs.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3omcxlaol.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ctmynscp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lvjytgso.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xmypaeqo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zasygkpb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3gzshlllu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kpjecjcg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ztphllun.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3pzbenven.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3urbycwwi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3aumqbjlb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3trbybzat.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ahsulfae.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yxyscgtm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3swwdhsvb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3prosndzw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3zwgtsizk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3orhzpsce.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3woctvevy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3txvibprd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tropwcxr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqfopps.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3clvcajuw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3foebxpgv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gwgwsmkm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pvasrcqo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xuxjnptz.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yadmttkn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nmsthwni.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xifdlnvg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zamxqfpy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wtjnslrm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3bkumyhsm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3jumtwoam.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3hbjycvhh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fbnlbwec.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3fruixayl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3arlygmun.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rmnicofs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ecqprgnf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3seuiszyk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3oeshjgol.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3woowclvu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3qqqkqubi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3resjfquk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bmmdiewf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lyowbgnj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eavzzogd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xkpwbbtq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mlzygyjn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3saljszmf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3samppbak.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3gkkruymm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3rhyfuebm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3vgunvvox.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3fyzcbzqi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pvajnvfw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3dxmrqsqm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3nblptbdy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ojpytmfe.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ymzlhfjs.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3uicxheoy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bykzchen.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3mwudqtbe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qiznfkjk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3zacdrkfs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3wvkcjzma.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gdwgphbj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3aqclmvrh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qrmphiqp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3sccqooci.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3noaklfxg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ymeymhvm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vijvkzmr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rfwbarki.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cwgmrwis.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vkquwnod.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3xngcgojx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3bnavztbc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3swdmwnoj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3yahypftt.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3nsepwqut.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3nheelwpy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bfnspdhg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3szznoxcf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lgvixcev.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dolvfygu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qnkmjtfo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dhkcilfb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3priqtoxh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3gqayclmn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3xzxcpbqe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3veryxxjv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3uvuszvmd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3lbwxdmji.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ayqeikko.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3nrhotmzq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3pyecakww.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dpesjtuu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3caxexvfn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3htavdvxa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3fivirtwv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mvtrlmiw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yczxtzvl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3tnfpjnke.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3oourkimw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3sgjizzks.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3czlachan.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3rsxhmzem.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zdsxqucu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3tshaxsyw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3psnylycl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rbmzrvma.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3orpzqydh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3hueszqjf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3bayoshme.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3krinfrvx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xzdlctva.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ldwyjznb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ogvrssup.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3pfivdlcs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3lenvsfdu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ieogyeyt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3xqvlckfo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3otsigbju.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jfwzvsiu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3lqwevvkl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bpawbsjp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3orlfdybw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3swdhhmnk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zdeszqvw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3caqyjrmm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vheepaxk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yqupbjuq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3kmixrzzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hluxbgdu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3scpsbfax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlvdosfb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kimentdk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3mjimadtq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oauxpnnf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3unpccgpe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3aqjtsepp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3yiovahrh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3otsvpoxa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3mthpbzbu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rdggcdnu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mreadtwe.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3sftiipwu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zihzrrah.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zyyyhsaq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cnkjqcux.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3enhlxmls.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ffsrlcwh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ifayfwpk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3xtncbbcb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ghoponhy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xzhbrxfk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ogvggcre.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3okkpneuj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3sxzmqduh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jgzdlxfj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gvytifuv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wnykueqq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3boydozbe.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3zvbwnigt.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pxonqyfr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3tnvuzrtw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3yngfmpcr.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bpwcqmcb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3azaaefjh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ygbmiubt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3utyqfecz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3baqjwbxt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3lypizsqd.html


<!-- 参考信息 -->