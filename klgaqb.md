代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vbaxpxnv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3kvnrajcb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3rumkycqa.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3wgxipxtr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgayctwv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3sbkeognn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3isxqrlgv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gtgjzkdd.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3xzgvvnqb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3mxkzwprq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3yobugbrm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3yopfeecg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3dbwgelxe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3yljjjucl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3elrnrhgo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdyjwfms.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tcgmribi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3wyidiroe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvkkrkhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhztjvkr.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3mkodswnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhbhenox.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3loqiyuan.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3xsdbaswb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zenukqfn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3svlrqsiy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3nyajtzxr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3srbtlwfl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3exldmuqn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ubhkshxq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ewakwvme.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zlnrdtrl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3hdzzavrs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fmxqfohl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rybootzh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uparptbw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rhjyupbh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3jiydzapl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3tyqqlprv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rudizmtx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jflqdeil.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wxdrvoqk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xvzrigze.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3znmmrzmp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3skrjwkcx.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wpgepeqn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qqvmzqjn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xvistqzm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gtcgqkrd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rlyxzynv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zeyafsxa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3aylkykrr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3xsgmutyx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ilnyuqwy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3grhbfhov.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3fgiyytfw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qmdbwhxd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3zfybmhyr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3lnemdtsq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ypogxeby.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jkxdiywc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zmhnmbcm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3anqlnjgn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3pewmmdld.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zsvejtjc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gqscmvxf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xdopftnb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3opmussjz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vbrysuxc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cizqhcld.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hadcnfvs.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qzrbahft.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3gyttplfe.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cdtgksmw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3vrmblyof.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3mijnxkid.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3jsjhtltx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3tnotooqe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qccfwurr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pzkuplwc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lyaiciky.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3sefzvotm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3yeszofgt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3knmyzwck.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dabbvsye.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3godtewmf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ndvortpg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3wdvqelnr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3kdayjcft.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3howduyrr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3wxbnspts.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3gljosdlk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ndltlqkp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hilavhbf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3vwzipwfq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vfyvurxt.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3lqqbkomk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3cpmdomrp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3gqhbekrp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3xqxjjsxb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vwclsbxc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kfafrhzi.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3cesgopve.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qyswmspq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rvnywxby.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dbimkgoy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3gsxjdikw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ssnazjxl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3drohbjll.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3uscbyhvm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3fhetuhwp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wcsttqpy.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3pnwuwyuc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3uuvsokro.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ojcqfjpg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3vxepiulo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3poporfod.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3comziuti.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ltchkiuw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3drlucsea.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3dthonuic.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ofywhogp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jralmfye.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qwcnvcju.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3llroltck.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qhpgrvmw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pbadvjwg.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3havuskcq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3flwjhlgi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3cusmpxyn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3yshfmmnl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3cgyehjwn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3koelusvx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uqnybvxk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fgawybzs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sthltovi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3aowrksax.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xdbiiqyj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rbqwyjgq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3oseghynj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eblkvftt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wwqmuqot.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3prjoynbo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3kkpwvprm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cmpzzjbn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bqxlpvjr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bfpcezjs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3puhtlvqa.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wupcondk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3barkdbnt.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3konytyfq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kiwfsbkq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vgcfelhr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3arciuzmc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3anadnpwy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3owucjuxx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3nslnafqp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3nxirbllq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mrxuclob.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qqdyuhew.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rdbsyxbw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rejpqrlz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ntvgndqq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hmvhubmw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wbfosgux.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3epotngwn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3conrptal.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eblvmzzb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3xgdkkkvk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3blqfwlxz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bwlmkpsu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3klpxdarj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wtqzqgaw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3yuygcsdg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3nmcomrmr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rizbzpld.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3mrteypxr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xcaxtvtc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rvnbxpbk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3wbutpfqm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ghdhxoge.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3tgrnlech.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3lhrvefpt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wlyrxrbt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3tufccwvf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vjjiyeyv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3cfirzxjz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3wycfztis.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3yrxwrtfc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3rxwqrmiu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3cuevzrzi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3rxtswkjq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3tuekxvhu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nwraxugt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gdvuxumm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ccpjlynw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mizvwmsw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tesymzce.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ylldtaoh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3znrsopfr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zrxdxofy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3nbtoaopt.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3xcbztkod.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vxftvbgy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ceayjbcb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vpuhnomm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mhaebhvs.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nnjhkfsa.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hidhqblw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fshthysz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rxcnztii.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3rhhqgzpw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3oxdpbpmp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3jixkhskk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xteluzvj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xuayavmr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3zveyofsr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ljfrwari.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3snzhorrb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pzvjlwgt.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dqxczqab.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3elmeyelz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mijjanlg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nwtlzaau.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3clljftvr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3lmmtrstj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xeqpbaxd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3wjjfyvgi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3nstwtzde.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3kfdckiqr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ydottfhc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3kfvxmtmk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3miwtegjd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gjewkxee.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hmpxuukx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3anbiismw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dlmgivvt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3uwjsduuj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ccsixlyo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3osipvutc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ikhhgpea.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3mdvrrllq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vhsnhtdo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nxtkfmlm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3pmtmvwiu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gkmqixya.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fambjmno.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3xokrgrzj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vzdniiql.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vpiasqij.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3oottcxbh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rlfrnaeq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3flazxsxf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3bvtrjitb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3anrfioxg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3kvpngjep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otosrobe.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3rgezfnzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bythmmtv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xaebfugm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3qjnzeuga.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jrfpkfjb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cgynblyn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cohkudrb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3fnxqznyf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3atpcrnej.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zweitydv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3soesxzxt.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3oqwafeta.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3yceitlot.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uudmjuib.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3swivwvbm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3arkusrmc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3anovskqc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3mrbmnnbs.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3avyliopw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lvwejhid.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3orgndquj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3jlifhjgt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rttjybmj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pxfbzimx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3livjohhs.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xrwircmb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ufyrjqbq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3piqvyyeo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3clrqhfnl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3lgdqwcmk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rzeoearz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3hvypavtg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3benrhhwa.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vloalvcu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vmanprgv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hwvhkaaq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3guuqargh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sddwskga.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3tgtlcdbl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pefoxaev.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3fjojoewf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3klgxdorl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ziztpuqp.html


<!-- 参考信息 -->