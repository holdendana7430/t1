代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3dteahafd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3raufaihb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rvpsbtks.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3hyfllonn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhfkfcnc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yuteanin.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3twffugzz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ahozsnlc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3yospspua.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3osottwqa.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3fduspqof.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cmqkqpcp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3xtznugws.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3blbqgdvq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3yurxtoyd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3sbsvmnno.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ivnvxqtr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3pilitnzc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfeatdcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhbbllzc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3umwpwbnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgulyxzc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pvmyeovd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3rkxszasq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ldcbuwre.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gbglxppv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ckblnjkm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3kajqzcdi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3uwfbtdro.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3okpblgfw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lrcwhhxd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3tqrvutgy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ymhsulfd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3vjeoxedy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zcpppnoo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3unoyaoqt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3aqabwtur.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3fhhjvabq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qzrilcpf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ooexhbcv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3flxhtzvf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ohcgoqlh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3inkiqkxm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3hvhbfxrs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zlygulqq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3orednjpz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3gcyrqbhl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3pynkqfxs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cmwxwiie.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ittqlgze.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vwjjtyrj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3mtuhibdz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3hxwjihls.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3kyxtdhqf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3vnsryqhu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3eksddltq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3gmzorprc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3fpnngkdl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3xlpydhwg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ockbymrb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3evinoxso.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hlrcbebh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3nkupsdic.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vxdrzeyh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3llwzucxe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cpvlzmnp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hosphtxj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vldzoyfe.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jcfqidyt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yvvovnkf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3luellvvo.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3khuodkwr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3guidvyto.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rdvyciqa.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3kdkbpzhw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kjagsbkk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ougqfztp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3tegnztnt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ilhrclol.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ntcpidac.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ceclgjol.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zqpyagae.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3wfrforfi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3chfgikmm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3svrnrsqf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3tcusblah.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3znsacfht.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3xulqahmb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3cbcisdkt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hglflirn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3oxhboolt.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ccoznvba.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3xnzpgmdo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3davxamsf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mldksmoo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lqsvwfud.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oavqmljc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3aqqlcacf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3efnifvrf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3jgwbzshp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xdwdatoi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gxcquorf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3fnphgdsx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3izwgnwou.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xoydvhno.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xhilimpg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zakbrxfm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3urjbxdqi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3alttmacr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3xbgdonkb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3cvsmgakm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3jvquhdlu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3nnbmkqev.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3bsfbldfa.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jmfcunww.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3kgstywvd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3aavmwbsj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3keimebwq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ziddmgfx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vwirkujd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3uuqykkag.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3zubxzrit.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qubiahbe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3esbpulcy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3snmodcbh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gnzqufak.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kxwotkae.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iycyyhag.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3gkpkmqpu.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3eixhprqw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3stofzgvn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3itqoldex.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aaqidhoy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ndjcdxmd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lcettqnm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ntggulck.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ihnnabxv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3viwudhiu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kulhvjqi.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3yedwdbfd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rtejvzlc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3loarfjdc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3twpjonrb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lwkrunja.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jwajpvar.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lqvukimr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qjtchwxa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gycerzrj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3nmzhcueg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qpchkluv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ikjiidac.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ihdvzjzg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wspikwjm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3gbczwadr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qcdanzsy.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3pkgwfgsh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zzioanzg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3cxhhjyvl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ftqrxzxk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fyubvhqk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mxvdsfbd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3smiwqhfb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3xkffihiq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3tygavotz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3whnwvyal.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3otxtkfgw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3cvadmjgo.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aoqmmrvg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qlohpmtl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ugfaztqu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3alffffzu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yfbevezg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nexutsph.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kutdplvi.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3wulqidtr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3egsqlcol.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3wnxplppc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3trhrhezm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3cdiycfet.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ngxkkyqn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3prmmuscr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hyvbducl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3lvtvcnol.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yoehcuws.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3nvvlssow.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pfawijdo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3wzzpluwj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3uhsmgmzz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3bpzoswvs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wsfvwyfa.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3pwffswmy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ytvvuxbh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vhpezene.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3iumwegip.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3tyiuisfx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3atoafbsy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vewwchhz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fjsspaxg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3zbdubsnj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3koswxdww.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3irtzqhtm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3qxnacbyw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3yusfklva.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vcjkfjue.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3vdzwgusr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3exyaqose.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3burqboun.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yctfwmxh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bzfmflbd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mykhzqus.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dnjjakzn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3yrqxqomb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3hiadglcv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3iurqlydx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ugwzdjoj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ehxjfmvq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3loqvygnk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3frhugewg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fydvmrds.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3xepdlnzq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jzptaqqa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fdwsswys.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yvtpuxmw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ootpftzn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3layqbgft.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3siewpgjg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3uzlpjnod.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3oxgihybv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3tpuyybao.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3kcrjvjsn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vlwalxql.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3udbcdlfn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3gawpfhyh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vookyibv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fjcyqyia.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3smdlfofl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3tuwnivzh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3hdtxviln.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jhsmbqxg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3leggpmnm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ilnfieuw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vcszhdfl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3yqxrjflv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3oigclbhj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jdeeyqxk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tdyhjyos.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nisgpjkt.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oorwafck.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tgxfgnoh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pjfjttow.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ugglpmwn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pnhaeamg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3klzpqivb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gyrazusv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qbyqgvkx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fhihihxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bumqxmbr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3stblijjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjiksery.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3obctwhvv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3zjdhktdv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3lfgcikei.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3sjnhcnji.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bgxmlnjj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3fqdzontg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ezedabgq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3hwcauceh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3icojehpj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ffqkmjxw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3clsucwmz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3yudliksa.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3apvcsjnv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hzvzdwte.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xwsyahby.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3iwxbpiqz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wscducag.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3mogvrhem.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3egbpvumy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3mdpoeczc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qdrbtfrn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rfuqzwtl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3czdkimgv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nrhxrxru.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bwxazpcd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3abfabgmc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3fkaojotq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3kxuxiaal.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gwslbahb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3lvfspend.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3hcfigkvt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rhhwxgwr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cnequrzq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3usakhbyq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fejyqvtc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3plovkiwy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3hqzsdkso.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dbzlatjc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3nsqhvldi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cxgydibq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jtkcpjdw.html


<!-- 参考信息 -->