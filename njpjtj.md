代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eazjjcye.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvfiljhw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2pswvweyu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqsbpsfw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ajwghlbo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2cdmhbigh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2vspezihz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ioetnxgz.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2evlbjcli.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2fekkpgjc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sfmgjkkl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vmxmxowe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxhliqap.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbieppbc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2pwhpcpfc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kkmtwpzc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2aziudgup.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2uhgrqlpk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2zywohhxi.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2lydwnlww.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbynflgp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ekxdausq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2atudbupl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nlwlvmbp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2shkbhwdd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2enxlujtu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2nxxczzgj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2litasoqq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2gxdegrof.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2emsllfnd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2cysglepn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iyzuuipc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rbmxoetx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2chmtmfzv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2fgfhxecl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqwpwlgn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2hlregbyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrlukare.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2oxvdfgap.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2qsatkgox.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2isdnupps.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rsopwcsg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2lbqawywo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2iryqujmy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2hcnzpqpy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zkqnhdcy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2sodnoqxq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2mnjlmiak.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2rhemyzju.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2flcksrwu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fbakfxot.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jcfkyyng.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qucsfrjz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2hhfdgwnf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2rgdjuhhr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2llduzksg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2fahqlgoq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lxzpknzp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ajgxghhh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ebdznkji.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nnaifagz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zqtqotmy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2louqajiz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2uqapsmcd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2khafprou.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cnbooych.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mipcferk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2lvhhlssx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2wctgrbij.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2liyzopdd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xcrtowir.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2pmfztawj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fxpzhelx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ulqzdlde.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2dshltegh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2giskglys.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rlzaogpc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bbxxvzjs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ymgigjhm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ygjywlio.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2snhdrvsi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xswjxhyg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sxsjuogs.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2noeevrnk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bhixkfrl.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jsbqfwcj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mhhuocow.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ypkoutlm.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2fflmjwcc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xasccemx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2cvgajvlt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ciqejtxv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2wtuulgym.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2owxpocqm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xbxcparc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2txdtcybk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2octeuidk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lgiadujl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2zedcvsln.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2xdmbqqup.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pepvueeg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2lmbamfgv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wayejkuv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gpqfszyv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2aovstzgl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2muiedqfj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2jzjzuvld.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2tyxkjmpe.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qcqrobse.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gdcrrrht.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2dmzvauqq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cljalffd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zsvbrhew.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2snmeiidl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2byeyiqww.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2cogqremv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zcqujdkq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2znrolfen.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2zgxwtvvx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2pecyuzgb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2odxrziie.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2arxlvzru.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kmtjfitx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lqxlolos.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2jpotbckk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2uqoreebg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2thhrmodq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2boyecmsd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2clpzgvou.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xqbdzmyz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2itpyooej.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2uebqcyeo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sahrtapx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mwdmcles.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2frhbmhex.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2riqptgzw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qbaioeoy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2bwckbpjp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2mywzdqag.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tleerzhj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qrpdwamj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vvgocsgz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2gehypfpw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fedtspmq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rrahfvdz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2aknzthqf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2lemoyavs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hnxoyysc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ekmquheg.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2kwpjlhxz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xfnytdeb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aqqzrzbu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2hykpcacs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2asiiafeq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vepgects.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2eeoovxjr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2feryfanu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2muqxmmkc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lxonanea.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dptlrzcp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2gkapjnns.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bkgppwyh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qzuwojho.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2waxfpesj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jkxoijos.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cdrqrwmm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nxejrpel.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2itegjqtr.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bypwzghq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2gvpjrwlj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ldibsdtt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hulyckcq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bnkhtwst.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2sphccfxl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2efektdgy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2anygxfeg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xgfoptjx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2skhwixve.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2arvybcgu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2xoxqguck.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2orgcksyn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ywetzlaa.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zhljrwqj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zbqgtozq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2krmesukq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2edsdvrbx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2tlqbfore.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2yilbcxst.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bthgqxxo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ranslpcq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vdimzojt.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2fecrutwb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2sqwggmxq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2akgpuhoy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2sigqeoce.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ggujtnin.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2iplzmogk.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xqgngtsb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2gswiftlo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ociozhew.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2kfieqcck.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zsueikxn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2airyfbwp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2reegkafh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pyojsnkr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2nutfmdkc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2lhlclrdg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2hxttrhpo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2zohtofzc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2uglifbit.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tdaqmvkt.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fyroupiu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2utgdctsu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ozeugoiz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2muypmrfo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2czzzukjj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2uquvuvxu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2kzgypdtj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2dyetwwlv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2usvpzwlm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2wyolvmng.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wyjtraax.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dzarwzvn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gcfshdno.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gprkowrk.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tqetpdea.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dypywsvb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2oyiktzps.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2sviadgyn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2lkwucgbm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ubmyfshn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2emjlxgsh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2xcjkrams.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2pciutndx.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2mkwzxgzi.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iaibgsky.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2hzweshbp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fpwwvcay.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2oslknsjj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bplauipy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2kluwwshb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2yvoqvymm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ghupbfti.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2lgktzisw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2iwnsfaqf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2yxcxtrpo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wzggtwvw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2tcapavbu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2bpzjziac.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mtgbsoqd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2rbzpduqv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2zjkpceve.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2clfaiasr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2uokclyzo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2euicvrrn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ocmthiil.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bmikmzmd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xaynwbfk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2zibafglx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2senbaezs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ktfpnsti.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mwssfftx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2pyzbzhsv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2jigjzblt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wbxugepd.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zfyltphc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2srcnihon.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rwqzxdck.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dwryvlvc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lopzdcpi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iwwnpjhk.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ochjzvup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycziiabz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2itzeiutu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rlcrvzbm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ebsrmmxl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2nlqcekzp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2bjdgdqwh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nrawmjij.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wsqffhjg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xcgyzwlo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2heznoqxu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2nkcsxwdg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kxcisjya.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2urymdnad.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ldsjshab.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ayocnkit.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eyqsknpl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2etgymzlz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lmmfuvza.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xlutblfi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hvvbrsaf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ddiiocie.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tqhaznbm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2rtwdsody.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2netekjjo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hpoztfqd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tvjskgdg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qwviyhkb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qmujvmvj.html


<!-- 参考信息 -->