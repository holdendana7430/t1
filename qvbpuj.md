代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipxhzmwp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2vuzebbqm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mttpbcyp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kmqizaep.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2nmxarbqh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2qkdwltlb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2bonwwazr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pofdiezy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhbpynph.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvjbwiqh.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gwvkogve.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ppxzpnal.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ufwvycfx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wtfjddnv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2jqkmwqyn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hrdgwpky.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2huggpvyy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2abbgnrzt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2teysdeon.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogrcjysb.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2qvjrubrc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2iqltxbsc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2inksfmgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohxujain.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2hmsytllg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cowjambl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hxjvzbwk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2mtdbhbrh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ppchedyo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2odrgqmpy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2bgeduohm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ncllhdsq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2hyhryrro.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ovsjfqqd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2cxzwnvnc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ukjvxort.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xnetpchp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lgmgclzg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2psscxylk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ibtooeug.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2nhslxjml.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vbkxgqjq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2tgibptmu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2uoiquenh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2sgbtgtem.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2nfeunjck.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jdihfjmo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2aeaeqkfu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2stapshhs.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2odkdxzgk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rgzobtdi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2rwbkybpi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kqsatwqp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2utkfibxj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pqzqrzcl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tdrdlopt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2mdzhcucl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2eydakdmg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2bxiuplnh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2awjopdxz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2nddaqoko.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2zcnzmswm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zingkuwo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pknwdyfd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qgspiqiy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2frtmzpgc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2xpadcccp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2lveblgar.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2opzsmcul.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yluuyngr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2eabyrxkl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xewpkhqf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wgoleiqb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2akjauvtr.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2aotaibfz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2glqrybxc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2egajdooc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wnhawvce.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fdrhsnik.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2fbngksos.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2pgiazpdi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ozcukqrd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cscylzai.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gdzehree.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mzrhrggq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2unitzgyf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2banufylb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2uujhjzkf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2sjnmbkcf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2qbslcdzf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oanwzewh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gcocdnos.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2jnfcpqvk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2trhddknq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ribjfzho.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2aqyodemg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2tkxmthkk.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dybcolrb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2danximlz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2libimktb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qsixgxgi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2sdsgfplp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2jtohuqzo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2nvbwiijq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bfgqperh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2sivsrgtu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2grcxettl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2adixwerm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2tqkegbfn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fpseeazb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bcxemflj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2baiyuxso.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2pfluhfkh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2jdcfdsip.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2mbwufjng.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2wwlsvizr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2scqhbsef.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2xoaizvmh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2boumlqfp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vhwwihgs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sumevicn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2esowcpsp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qoqvskds.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2zwotxmut.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2yvvdkqyh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2fdmwhhag.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lylpmdnv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rgfknwcm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cgpotcqq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2adyzfckq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2lbhfkcre.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2syksonhb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bdxgtgar.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2kivlwzld.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ekwrfxcp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2bbkylltx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yljfwmld.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2koqoqipv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2efuriuph.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2fbaadmfr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2bhgfspuo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ainpeahm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vturouok.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2oybbkfqi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gubtneic.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fuahjnyy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ggbrxahf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ewevhgfw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2klbjudtn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nqlhzgrc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lttrryon.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2igthctix.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gmjduhma.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cipbvvgx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2inuoaizw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yksebwkb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2znllfyhc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2shllnfwh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ryrhhzkq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2rahuuczg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vglnomgj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2goscslqb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gaolcmvq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ohpsbtcc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mefdtwuo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dnajdhtj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2nidlqipp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2vyjmkkqg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2erpehtos.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2nvkhtone.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2kifsvczk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bhridtim.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2eyrnutiu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2zosrmwzw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2pngrayvn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eefxnzvl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jurcsoge.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2jccolzgt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ytoxawdu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2sjsbrmdk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2rfitppcb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2isofqflr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2gcwayozd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2yodetrrb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kqudwhqi.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2wdxxtolf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2uyyvvndl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hzfvfmvs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2gqjbgnaa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2nllukuzw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2emgejfbg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2jzhzsiwl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jvxxvlwb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pikwhneg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2kkiokwxh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2rtvqyxft.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2mquhdwph.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fdcutymh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2epeibgmf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2idcfaazs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qcwrllbu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vdigdsdg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2gxdcygmo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ltwpncqi.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2dxgkoqcp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ockmvtym.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vctcnuik.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2tdcwnprm.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vjhbwmlz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mwlcxndu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fgmpclnt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hmryvjtk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2whvtwaeu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yuwfychp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uvonktnp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2jpjredtn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2yuxgfyxy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2nmnpozbl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2mczayqki.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ujhverkx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2paotvipa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rsfnhsnc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2bbpmeyrs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ykkmfxkp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2fyemgbre.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2rascwwpm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2kbsaplxu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ogcfklui.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pgyljeri.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2aefwdwpl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2krqtrzvw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2hvscnehb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2bxgaxztj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ceotfpqi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2cstuoncg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2frpjxmfp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lzqmjsfw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nsktyntu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lqxxfbbf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2xmftnwke.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kaqjsvep.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2mcknpans.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2oprmqejy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zivukfuy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kvyammml.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lvbtwcnb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ltaaygyr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2heefjrwm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2wrcbnrwa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wpsuflmg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hnrdfjoe.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qewxyyvd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2vmgzqquu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2elzfwhpb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ciglgzso.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2farmaoxw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kmavracs.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2dlwnwbvv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bpjsuwwd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wwchkwxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwfrnroc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2pcdeafpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2auuogidm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wslmedgb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xnfgjegu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ctlntltb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ikmuwtgo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sqyrafiq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xtjmgezj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2orjhpafz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2oihgjxkf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ttdqyhsi.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hgudffnj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rqomqlww.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dwpflftw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dbmedrns.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sdrjyvsj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fpzyordd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2geiklqml.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gnsyssdh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2falfvzhl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vbvnhhyd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2smsraadv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zhlyxgjs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2odlzmqrn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bydafvim.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tysdgdkn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gqtbhsgd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2toigwaat.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2apzbxeqg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2heneetgl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vwftpoed.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2eurcmsqw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2oslqfwzv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2amfdtioq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2amiaqhwf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2kjgesqkm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fikyejno.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2shbielvx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2iqywpwgz.html


<!-- 参考信息 -->