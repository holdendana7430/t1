代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2lmurhhdr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wqjwwsxi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2mbxsfgzb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wtqobaxh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2enaphdub.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2qjxllxtp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hclfgwgr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tvjodtoc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2gyxezkpu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zqxmvzmh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2rhlqjiby.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ngodicdc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2lhfqowvb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2uijovtup.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2zmaycodk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2xpqufxht.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2fzsdxtor.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rtagwvfj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2uaxrolvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxqlqxgi.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2moiaznkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2njfhrdgk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tlmhvsme.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2rrkvanff.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ibcqvdse.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2bfmphnmu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cvuujsrr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2svzmaalw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2evbymwdk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vfiilaxp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2pekocgfb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2qskwkpcw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2vneqnqfz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2cizqxegz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hamtfvid.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2iuqyrwee.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2zookeaxp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2gtyhbzyo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2wpujpgjy.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fhdtdivh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2pebxkbfx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zrcugnzn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wawpbdgn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2fkqpnwvc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2orysaalk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2aowtothr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2oqbxdnib.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2mudygddm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vokugmdb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2iewvvhgj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zfqyfwsl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2spvayrkr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2yppjjovr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2nomzldvc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ghzzxxkx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2nuuoajtp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2qvkvebmc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2wgpmdntk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2pttjabap.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2drtzmfjf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2efwqrlwp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wswyeyxa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2iptzisvz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2eomlumva.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2opyvwfgq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xspkcbad.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cfgyhvmi.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mrdfhmsg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nxoxlsim.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2iaakjcdw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ynpxnupu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2oigsuthe.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2zhselgre.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rxhcwzhj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mcyssbwq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2opcbxhkw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2yzegvefm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2tswbhvyl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pyywwnlo.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vbacfkgy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hmoyinxs.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2snggnafm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ahyhzfre.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2nzjtbkcm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rzgnuqwr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2rxlnlpqr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qdmyfbpj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2orkemhbc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2hfxabbdo.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2uktnbvjh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2mptxkfgr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2kxkaxrpx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2vqwxquvw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zpcbgmku.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2umkxdtqq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dittweol.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aqwrgjft.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2hrbcktze.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2yepfcdpt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2zsupvojn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ghhqqvvb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rjvtnwqw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2kamgqzbu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2himczwsu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oqadbmyx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2preaigun.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jljstjqa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2alobqtit.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2muubvnsk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2egeolqub.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2mzgimcqi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2giikmfte.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2unpmbwih.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2yfopkilc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zmsxkjpb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nralcejj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2gcscmnjg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kyhzlkxc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2broblttj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2skxulnvy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2bfyiavnd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2tkgclahn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qjwaygid.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2umpfnoxp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fpgmgftp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ylimpafq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2gqnnssgf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xephkmqy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2gbudvmlo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2hiqdotia.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2yixhmgsn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iwigkncy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2syvxxnov.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ysiwnpbv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hjnrrvmn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2znykqysw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ttpthgoo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2rzsxsqlq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wudrwbxc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wtsgkukr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rximthzf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yhlkqtuk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2prwhonzg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pwiztsxf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lvyrumxo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bxylozmx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ifdgsnyj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2edrbhzrz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vgcdaumr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2johujepu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nrfufgcv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lgielxzw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yujxqynu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2cyusqjoz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2qtjzagso.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2nkxcdndf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wktztzjd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2btnjgddc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cuwifjxc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qymykufb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tjlcytnj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ndzmzwmx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2edntacde.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ynkhlvfo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gywvjish.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2cbunzkhi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rolubpsj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tluzxxuj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2irmhhxro.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2cvtwyved.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zgnpyhnj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2tttskjst.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2iujiejro.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2mvguvzxt.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2axoyieuo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2fbpkawmr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zwpsbxjw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2lpiloujg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2nwecjxom.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2izzfpcgn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2awhngvhj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qesvlyuk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2yuvtgowc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tfdajjpi.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xvvyrktv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2jprqkdff.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2cpbbtygs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ypivsftx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2whkpbvbd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2xgjrpxor.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ptkevkdr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2jqhdkedc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2snkvhvbm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2rdsdvsyl.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2nhntewib.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ryzrxyfu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ljiduxpl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zolqidwy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ltafnuqg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2cvvyvwfl.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2fmakggxw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2zudkraid.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2vyrjtnnf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2rrpfijyt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ffeempmz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wncewmgk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vqkmykta.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dbkppylc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjmiixid.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2btxruxce.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ldsybyxz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2xqrplxtm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2owyxtlcl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2fjgbpijs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vmburerp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2qylowdqe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hfhcroew.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2taqzqidp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2buamouhc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2mlfcyxgt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ojvahvux.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bkpsdjwy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2wstcxvpl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ptwacagz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bbnizkff.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xijvemuq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wyemmyxs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2wexfrwxw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2husxttsp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2axpgeojn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2lllyfjzx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2efudrzkd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2txqeaoeh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2drjzjmtb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2taevozan.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2phjkxbqi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pkeexpji.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2gapdqnpe.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2lmhemyjg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2rhfawrdd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xowhresg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hzxtjrse.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2dachbujm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tmubrwum.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2uwkrbffq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2hswsyqzq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ewyyghdr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vkhqmria.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2nqldhgmp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dmayzkhh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lhxkvcsi.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2aetwiyfw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rwbdknwn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2szjblfcr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ruyzcsga.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2oktmyibt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btmvbgpd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2rukqxsjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smsbcmfk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2csxdedry.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2tsnhmtjr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2clmwppps.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2somoxyys.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vnsmhjkd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2bthuzfkm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ymzpsntq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2edcpuujt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oprbydmg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bidsivbj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2oymbkgyn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rwzbppmu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bsqhuuha.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2iqmqokls.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vasxdlyh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2idmcemgy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xtccqwbb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wyeifcol.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qgbcefys.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2zlbedgzx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wavyegcj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ycjmzaly.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ylewjtfd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2opstpilt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2izsyqgek.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2tvophlpl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2vespeisx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2mrnyudfd.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2egxrllir.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ppvglbbz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wkmkibff.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mtvbtcbm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tqexjjng.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2jwezmwvu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kzhmxqad.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mstmexlj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2doplgmra.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tcrhlwmh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2wpruewgh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bpwtqzhk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2emnlashx.html


<!-- 参考信息 -->