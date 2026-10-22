代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zhxbxzze.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2obuvtmyt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ceajnlei.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hjvdifbl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hcdorgby.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kicwlspg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rvqiqgoo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wysidubh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2laacnrex.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vreiejgi.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2uihkozbc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dycisxlk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2wwycwoah.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2zdzoosrn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2gbmvpdtj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ghohvxrb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2jbyzojlx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2rnhwwwqp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2cphyvpgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzrrzvdf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kxwgkvyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffyoxgth.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ffrmtnid.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2rxvyfazv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2tpwqykuk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ncbvetgi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2aweofnif.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2uhwfjttz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2rkmjyuxe.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ofdgrhdz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2dxjmjpkh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2lxzkenxn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2llcoguku.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2trafsyue.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wpmacycy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mvmxthbr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2swmmknca.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2joixfruj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2qjxteaci.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ayezcjrx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2geblupnk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2lkkfsslg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2zqljzibh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2wckiwlyt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ucmclhxd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qxmiogtp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zbeoihkc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2nclsdlgo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wdsolyli.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qacnbhxk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bvjjuzpb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2csitqram.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xyxgyhoa.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2axvokrin.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2etgoemko.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2lcmdqjtg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hztzuwgp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ptrrjjul.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2fqgtqdhd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xiaovsry.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hjwgrvxg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zkvszdsh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2wuddfvcv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ymedjike.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2weqotxdw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ixjywujv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ctcuykvq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kggkqyyg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zsyycpzc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cokfxqfo.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hymjdtgb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2capxnmmp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2jwkcrngf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cxzgektb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vsgjekbl.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2sytnwawi.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2yzvqevnu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qvizzzqf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pwiqfmop.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kcolnivv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xagjukri.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hubeomwv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ietrutor.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cwmvkgbv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cckqizol.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ryamznft.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2chsiyohj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2iytuvfdd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2sxnyagqv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ggayvapq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2bzvcumof.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2xbeqnkho.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ncqdatlu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gbotoebf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mqrrbduv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jtxhhqxs.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2fmryrpww.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2sddjfsnv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2nekehfck.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2simoxrrc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2aextlwke.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pbgiynsp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bphficfd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2fmlnlcyw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2tolhpdus.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zhlgueug.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bdlquvjr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pgjoqfvm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2zfrcqixw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2obkiyjpe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kklfnfhi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2sfvkciev.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jnwdgjon.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2lgfkxrgi.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2kybmnlxb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2seeevqri.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2eaososvf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gzsecjdl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2akpxcbof.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pxqnfnan.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ryqnrzcj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2qumzmqun.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2etjeaoym.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cdnvnrit.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dykyscpq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2luqqvfnw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2lkdhqrce.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oszsfypv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wskxrzvg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2qmyhbgej.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2dbdztghi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2liofocyy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2eunbvjry.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tgcpcxnb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mmdcfijq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2arlkyybh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2rthtmpll.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2dsdplxbm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uwlkwtyi.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2vbsqpwqj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zcuojtdq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jblezcvx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ppaakycy.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yxamcasg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cqqggrxe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ukblmhvv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2iyrkjznr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2okqwjppg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2paoqcpfy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2egvsijah.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kohphpjy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xyyykkzt.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sefykkpi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2vanrpgfj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2pxtbxnjt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2coohexcx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ppeqyafs.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2qvomwenx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uopcctnw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hephthrh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2byovkvrd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dxpmvakd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2rildadbf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2qojqlrui.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2zagulsjv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2hsrxvfnc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qgesdsql.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2suoicuhn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gvcifkzq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yqvwrhhy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2fjxvtbze.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wepvkwhn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2frklebtb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vevlriii.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zraxqihm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2exmogljv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ctzmkoqz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2mdepmojc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ihjdfbyh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2znqjgswk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qaekcljv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2dsikaplz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2xgusorhv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wqyiicps.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2rkuuqwrk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ldxvdifo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2utrgxahp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2xmwjvgrn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cpsinnyq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2elubjhgs.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2wxiwqqjy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2woqekgkd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ltdpbxbm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bxgrxutc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rilogepd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2futpkaht.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gtcdyhnd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ksczvhnl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2yqayyolp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2blfgymja.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2pjoboezw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2wjbjhykn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2yzufbifk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nvmimnfk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2xqyiefgd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ajlnmaip.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hxpzpnpt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zrfgxetz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dlcimaqu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2clapdmbr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nuvjivad.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ttwkfnwy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2cuhjbhlx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2xpcwwzro.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ctaigvqh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2xaqtdvie.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nofgjjmm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2tzfhougo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2bnxqldxg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fznwxiok.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rbbouuvf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2iykebdhc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bkmlcaxn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fmbxqvvp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2owvzmgpp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ebhjchvs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lxyphtfk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ujeznztx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2jxpfdcmr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2fpefrejp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2xllxpzfg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sheixqwb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zejsydrc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pulrrnoc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ndivqmiv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2urvqsyrw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2buqliywt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xkzrxzdj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2adybwtjk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jskzwbwv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nqspiduc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yrsvzypl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cchyaduu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wtxkkuzq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hkpvggvt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xlfyctvn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lphaxsyt.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cldrgvev.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xybcilpx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2givxtpwh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dlzsjjoz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lsajidin.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hzefjzpd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zuujlndg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2olkuehtd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cgbaoujx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sllnugli.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2auciaihi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yvkaqsxd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iqxylgbb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2yfsossnh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ipflswqq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dwpoptxi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vxfaarts.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2tpwztaey.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pyqdqfmx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2yhqazsyq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zobvewbr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2turqjsbg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rqravxue.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2maqrztsv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hfrpsmwb.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2guqexfvw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nzurrsvb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2azjgogqq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fatvshmg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2bthdpfbx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hrxktxoj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2fjypwpim.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lorznsjc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vnhvwctf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zpnowwok.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qoqitofl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gytjcbkr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2rzlohwgu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2iogczkec.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2grrmtleg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ujlpaffv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2bmdvxcnt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ydtuwozg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kvcwuzux.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yklytzof.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2jojqcvxa.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2riocvtam.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lyegdquk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fdgdyliv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hshmccgf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2imlwhujo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bhwppevk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2oaojoxnl.html


<!-- 参考信息 -->