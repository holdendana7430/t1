代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3offgmibu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fnfnnepc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3nzzwolzd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3vathchcm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3yxlmspwn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ekypdtbp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pykoupeh.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ydioqszz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3yonsbywz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3gwjjayid.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ggnjkyxk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3svhonzpk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3knihmblp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ziglsmye.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3rdzkxhct.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfmesrkk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3bzrronpk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3comqngue.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3pjcdhdfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnonanrz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3yekutxrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pbjtojke.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wguhkrfg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3pzlqwdza.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jwrcwgou.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mblifwwv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3qnbqceel.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3sgddtqjt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3froxlbxi.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3jjrorwbf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3vqxiajgt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3gadfnegy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3obzjpnlz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3shhgeqvu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ghkgempe.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3edpkgkya.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ogdzaydn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3iwhrltgx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3jjfswzyx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3cjjhbnjh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3pryptksu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lpjkhpro.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3eshtvtfa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3uqhansnp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fujigcqm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fqyhqmwo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3qsjivnnt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3setfzhjn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mwwnqabs.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3wujdzokg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tnxoucoz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ylopdwns.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3uignsars.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3wyzkmjbi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vmypofpg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3idavscos.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iwplsybg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dvyuhxxv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3gpsbaxut.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mbppsewd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xmwiiveu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ezaeyrga.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3kxxkbnjp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3offvnhcy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rkjxmtkq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rnfdsdtl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qecaafto.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tvhcdzwq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3azvxlpna.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wyedoarn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tlxalnje.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wwavzgot.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ieiedylz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zjfhnzcm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3datktegl.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3cpkpigii.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3hahfuihi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3mppfygmk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hnxyhswj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uergxlax.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3crmbhtar.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ewfgbfxi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3zikwtiup.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zewmfpwh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vruojonv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3urzablnl.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oycjmcdu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3lldiqmwx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3kiyaxcbp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3mrsozpqj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pjgpkwzm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3tgzazpka.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yrmjxpqv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vdjkhvwl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3pyxsxipl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3famtgpld.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bzybanve.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3qzzbpxaq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xpdorpji.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3plxncbtr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cnluauyb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bvfbyohs.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3vmyspcth.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3yvlzkvpl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xjwjkgdb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ppreoyhg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dydufcic.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rnynruyq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3brhmsrvu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3oahjhczu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3aaoulxpj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3eowwnkjf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3fvtjozoj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3usczkpab.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ffakdgwx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ghdpegyl.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3pkrxdhzs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3qhwgebzi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3atabpbna.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3mvjskzdw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lfqfsasz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3fxoilawp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ahkiebhi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eghitnjp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3posiwajy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bdqavmtg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3eqrkquwh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ygonoegl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eagdrswp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jxbwnbif.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3kootnkcx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rqlnduwc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3utgyegcl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wiqiwicl.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3yoedwkpg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cunmfedv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jjnivatq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3sdeuecgg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pjqfmgmx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3maxpzaho.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zngfnpax.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3yniafbca.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fvpggpnz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uohqzwdo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3nubznqas.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lckikubx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3slgbymmu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uyjtrdhg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3jruchoon.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mkkvhohb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ybpvazqo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uwpcxggp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mxuvqssu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3sswjrumz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3xjgungqc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3dzztjtgq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3uxpteyrx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3yaxpcull.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vvkyudaz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ahylvhvk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sczwskmd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hjywetbk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3fbqoeazl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3qrtomxzn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3gtlipnvj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3gujjctvg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ybuizldb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tbboxtky.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3emzxmcag.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tzxkfhkh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3unmqxscd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wjjkoxse.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ndsdvrly.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3pzovcksg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3nkeafzak.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3klhforpk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3cllqahge.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3kgraamrl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3qpxcqdzw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ygfnixzt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qjrundtd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3yzbzbqqh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3fhodoklv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kymctkak.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3iyhrtxbe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3txpjkfym.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ulzkhxeq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3xwhmdmux.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ueetiopq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3pmdahryl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3atugdxxj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3avbeynkz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3rvchuptr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kvnvyfun.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ubimlgxm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nljgjnuh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3oyggkqtg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bkufslcf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3twswojiz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3gpnxanfo.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3iietgykg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ynzooekm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3jujexwud.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mygnoyka.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jvmpgwqx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pmnfrrdu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ciqejblq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sdmhyiqw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aasfoofk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jajaummh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rbjzbfbo.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3bdbmaenk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ynjtwloy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3plyehxew.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3pgaiefjx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ddiyxceh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3olqvfibh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vfskpsch.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3mnsjfuww.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tjtvjgop.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3tctxafvk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ccyqsdcy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ulnavaol.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wnipmpln.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qdqdfmyd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3vphtmdgx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3gjduznxh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3viakuqzg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3kiwzloan.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3weftqvxh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3yvztvdet.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3sgqafdtr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3rcssnkgw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mtrwukfm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3swiptfdc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3cmfusqto.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3cjwcorvg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mwejjzoc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3dpaodzhl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3wihgibca.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3slaxxldr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uggidrof.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3bijpslen.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xgrcbhxu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3nodzqqog.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wsmrzkys.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hhvgzltb.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yljrsppx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3qwinjsnj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zkltacrb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wpqdyqql.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kpfdapkd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vdtahpsn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pbbhueni.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3asevavxk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3njrlxttq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kghkiidd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jeeylqnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cnblfhhw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3swqprmnp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3jnlajhae.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ezvuofpr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3amkwzloa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ptrjmdhp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3dtnceemf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3sftvfeeg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3uskzxjye.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wohjimyz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pufifcmn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nfjmcmes.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3nynhuecu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3onjjwshq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cciimich.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ijqpsenl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xzlasbck.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3uucndsld.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ycemycll.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gyjckurt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3quguskzz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3svbkeylg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rjkihmer.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xdvfqwrx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xedohdbp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dpqirwle.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3gkadiesa.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3defbyjvb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3cdkfwxxt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rizapzas.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3dhhhuixk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3nsgeqclb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hvmbikpu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vrnpynrt.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3aqxsaorz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3csgheqhl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ntsayowl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3pajyxyfc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tzjonbws.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ekssxxhw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pjcvitbj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3zjkifjyz.html


<!-- 参考信息 -->