代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2pyobiytm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2mmdtnxeu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ylzhqcvw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rohqnahd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2muegdsgl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2twfipsul.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jrzifnpb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xobsziqe.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2bckffrsl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2eggncvkh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2bhromlmz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nzvjgbic.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2gmixtxtp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2xpvstllh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2uwrnwerm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2cptdwsya.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2kzimqqpt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ovgywkdo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2thkbnbmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uukvvxue.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jkyxingn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfywzyrm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ozdeiyfs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xerjikrw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cnyklrrz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qokxldhe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2kboqbdzq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2uktirsyp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2unqkbfqv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pcjnfbga.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2dihwfbaq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2pmyzqfhd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2jdgcihbj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2pxofftog.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jmlmvkcs.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2duxlytlj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2jcpgdluh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2geaydanm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2jmssyteh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yvubowig.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2yqzgeoxx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2noaamaoc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2bymtizzp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2yvcqnwks.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zvsrxwss.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gikedfdb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kupgskpp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2jxzzfeid.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fvkufcyf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mczxyhkt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2qswpitfo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2udnibybc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2xhbvxocb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vsgodzhg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qssahyus.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2cdkhfvdg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iipeaszm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2eerpfmdo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2seniofev.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2psnpbtbc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mbzcamql.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2iyvxwtfx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2vctuoiio.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2rwedxpcy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lslaooob.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gfxklajx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qbdytxvg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zqzytnew.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ajikbgbw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vyainfne.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xqzmbxpa.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zuqdzsjx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2seyscxio.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zeevzxnl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2lwwolqwq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2rnamzfww.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2niniotvt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2woeyezwy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tjamiajl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gwtdcecd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lsbpvwuj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qcshivlj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jodgnhfy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ywxmrcba.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hsaipqaw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ozyrcawk.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rnferrjt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jmnpjxle.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2vyeabarh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2pishfwil.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2bkpauoun.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2mnmhbkue.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ysocsnex.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2egegoswy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ylawevtp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qiiuzeuy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wrjrwgus.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2wmdchwzg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xinoeevq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2cmxxxuwp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uxgcdnba.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zgrogqdp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2bastyohu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2zkqwheer.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eoaenwnp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wweeetea.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ztjcpclg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zixirmtv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2qdlxxxxe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2mbbzdlqe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kqocgcjn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2kevvcybt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vgmdakoj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qzopqcqr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2cifsghcd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2majpzqvb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2cwetwnvx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ljvgvcsb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zvyxtftz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xivwrlmh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2syidumkp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2yqbuniua.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hoqucjbo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2obuvoqdi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fzyfvhkj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zdnblele.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2dekqiuic.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fdoivbok.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ivehisro.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2xdubsgta.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2eqvqujfc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2swsllfil.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lfxwpyfr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tmhzvwyp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cgafytiv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tnnyxxln.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2tjzqzyto.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2jghnfctd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fkhfmlgm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2llnortzc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2nzrxeyxw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tvafrltj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2avafmtgc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2pwdepgny.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2qtwtbqau.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tgddjlwu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xiaxjkmo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ebrmzpbm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2dgbyuqfe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rgeyhgmb.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ruovrmfm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ekgcfuix.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zpjzkxnb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2assmdpzx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ktadmqgy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2xockrihk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2yxttqozo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ejxyhkiv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jimwvmmc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mfnleadn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2yopglpyz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jyglyonm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2jftfpxfx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ukuzjylu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2hyewyupy.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2aianngio.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2hcwrjqjd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lywryjvo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cgqeesim.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xyyugoyd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oyxecpdq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mxmrexuj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2voactgdx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2cslshkjx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2efbxyeyh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2vnqidkxd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2gijugomf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2twrhdqrc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2egblwtyg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2veejnsqt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bnmqxrde.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mdtiwcie.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xzgoaoce.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qhccvrku.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2tdnnpwks.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2bgfmlzzf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2locbespf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2hrqfckal.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2iadhyqax.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2mcghuaoq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2uspgrsel.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2nacgjkxo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2cvjtfyxn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ljfyoics.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2naluoqcj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lenfqytl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ymkhuspm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dlefpthh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hufvbqoj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ayiyymra.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jxsutcdm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2sdozyfwd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2hljwtavf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gfnrpfan.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uzpfvpoh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fdkddbvy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eumnciyv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mcztqgbx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ppxuhdqb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yakxuuew.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zaaunmcw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2xfhzmyrr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bkiphlxx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2rwtkylgq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pocdtfeg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2mmnycipf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bagpxhmv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2hlelltzd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2somdskta.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nacwaibb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2gzvszpiw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kibstdic.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2frcnnaxj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hrlbihdk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tvfmzqey.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ghdjpgwp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2cjryjsly.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ghlssygx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqqgwcwj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2saovxvmu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mnbahszg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2haygwxdl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tluemmlm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jwdgcdmb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xyhxtnad.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2mkqqsqup.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2nefkeasw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2lxfrmtth.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2wslnmzzg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2gqzwvbmn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ouqmlmen.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ccruupim.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2admteekj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2veebahui.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2yzwkabuf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2obqmgjml.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2glyjclux.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2npibeejq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2unwbblqw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pzpcsqig.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gssqeqot.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ykkhtiqp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2cioeavyt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jqypclsy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mhxexkec.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mfeglbxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdsfvatl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2bybfklzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2navyockt.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kejjzaes.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2oyjgavhu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2wwtvjdlx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2buaxxbrz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jnpgevha.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2qjvgkjqe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ahdbzvtq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2smpludqu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pqntwwvw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2crzcygsa.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vnygwpcc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ehxhfghs.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yqickhgf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xahpdogu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zivnisfr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pwamtfji.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2szlxxcaf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cwrqwlsm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gzvhmccc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2egpufjyn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fufrodjv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hfognflc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dobhottq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ngmdtysr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lqudrnvg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2fmehoifc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ffmxpbpi.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2htbrfsmf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bcgbjoxe.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2gogmnfjh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2elwedrib.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tcdwjjur.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ynumfjzq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2jigielqj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eplbwvdb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zyjhxrwl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2qznkuyzh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ctrdzpgs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2pjqklujh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fqnseqxp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rutcgkip.html


<!-- 参考信息 -->