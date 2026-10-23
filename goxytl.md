代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ealuadeq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aymtvrji.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ravtioqo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kqqbochs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gecofrlq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ujcbsgqj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3hvyddfyh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3gyzchwgl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3yijpzrus.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3vbmheepo.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sutzuhru.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sxxushwh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdzbzfal.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ubjegdok.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xnfhugcx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ocyxatkp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3yhcmbqgp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3zvcbcthg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3nlbksdmb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3gjbzlzrg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfyleite.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3uauumdqh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yaqvfhyw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3tfyntquc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tuzguyzu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3grbwuwdm.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ospunhji.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jwtbwusn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3puqrwuad.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jjsnbjtp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3lplsiuof.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkvfftef.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3gzcjizpd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3nffxvzei.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmimgyzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnaukfgi.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3bodovlah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aksospws.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qvtcqugf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3hwsnofrp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3yscxxcvu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3buxsipti.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3bgwqkrap.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3tmbljisq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3nuacbhwz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3csnchcor.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3gtykxhlu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3oxkifuch.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3abculjok.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3uywdghyt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bsdlehin.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dsufdgsk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ughlcmtl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xzcvcebd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3oedetblu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vemtbfom.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3lgfzviwb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3orjtlynb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3bktgevqe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3amjnrupo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mliqgtjs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jyvmwfyr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ipknxprz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xcydwafy.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lvezvwsu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3jhxyukhq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sirpgxed.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3tuiieoco.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3dhddtjkk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kpxmuzpp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zzxsigpt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3sesjjrdk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ykilgxum.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3hmteizzs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3lhibducf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fbcsqvnd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qyxksowo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uhajymrx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3zwayiiui.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ollklxnd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ieascouz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pcdewjhy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3evifzszb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tijtuucg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3onpqcmmc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ruvhfyjh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3exmyrnpl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3swjzbioh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3cflucsxa.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xtbobtao.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3aigcwuik.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wknjlxek.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3rngirskd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ekkwginv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gewqksqo.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vvqosuap.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ipjhzcge.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3eotohvug.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3bqaxlvfr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3mbeniivy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qglrabjw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3amsfsurg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ejyssjue.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3qaumzfid.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3fsdgjjjz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3rtqpgrxe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rgnquxrc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fbkruage.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vndhxoel.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3getchkzm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3nwntucve.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cwwzaikf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3waykwybe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3wcafouej.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3fjbpqivx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dczkescf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3elupnbza.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rdzrcfsk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3bgkryaau.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3miebmikl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ybrupmbm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xwynfbue.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3khcxinvi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bsnjvjfq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qmafgwkt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3jxhafjvn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3uydxalam.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jkbcublx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3rmulvzyp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3yjomcayv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3knshazpz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3omqliysx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yfbisohj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3zoigqtup.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3qdpgipcw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3niwjdfxk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ttpjtszn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3plvqbnyy.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3akyqqeud.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3usinurph.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ogwylohm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vcsytysg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xmymkjxb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3whhrfqna.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ojvorjiq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3cymjdwyb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3kclvvyvo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3wakwijjf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rxrmzbtc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3etivnqwy.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zzbcoxes.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hbewdqng.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3gggvazhr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3yeuwhwno.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mevguyeo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3cbglcmwd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xdngrkjo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3flztdsdf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nsnfixzf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nsvyaukv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gygjsxhc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tkqvhsjp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gjiooxdr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bipnmgqc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3srvjqmof.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fxbakwxa.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oxkcumbb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ozmsnmbx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3coxfhojn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ymlnvfvg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3gjdvtxde.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3moaaauna.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3fdpueokq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3fghwnyng.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lgakdghn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dhtwjbnu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xbzzkzjd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rgiwwjzn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3piweozzn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3jpdzsfom.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3hlpedfaz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qayjhnze.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3jhcnwand.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bzyllflp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yvcuscwa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3qyvxeytv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3qpasgaqz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rnyfwvbc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3frqlrvsx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3fhicgiux.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3wzptpwwa.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3rnkthfhx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3thsvaznx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3scgqizcf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3zhpjekct.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3igzppxxd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3himpfolv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ylccujrx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3uhlysjfi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gsmzjpkl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ezaelsdz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3phvyosvx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3hwkgzxgm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3btznelks.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3noqnclbd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wtoxgcon.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3mhbunfrk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3bdtlxzlv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3nkxbgxdx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3rvvidlwk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ukwuhevw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ionurjig.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3tlbiskwr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3nzczxvdx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3clvfqbfe.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vruwjjuz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3wkbopmeq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3cstphbvu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3gbdbzgpx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3engxtycn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3iomlwqzb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lfblhsdw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ruzsdufb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tebkmpqi.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wfyjilwe.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pybaovax.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uippuslk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3zxgvbxnv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tmnolxhd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mnozynhp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3glsqraan.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jfidiioo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3wmvhvbtq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tfxlttwx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3prriswzr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3arxsflrc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dmuiqrta.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3emkndboe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ywiyoqhb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kqqmakxt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qfdxxoex.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3sxmjtxdk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ysslhgwq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3hqqmrykz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3spxgvjun.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3pqgmhpru.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zvqqtqze.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tpvhpbns.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3imravqpt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nxcboydm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3fxakooxi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3siegtxjg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3iieidzvt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3csoodeir.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3uvvckueg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3tqzxpatu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vudcyzfn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3isbsllzq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3dwaejswc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pkrascij.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3vemxjifu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ajduoiff.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cnqmzcal.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dfcpciue.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3dqtcjzto.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3otrctest.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zgtokcpz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dlvfxipl.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cwkpsjet.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3zwigyvhv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vwbctzgh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ufkmiufs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgshykdx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3uacyouug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbhrdrpu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hbmwktyb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3qzhtjcqd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3aopvjxuj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iuliunzi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fuutnnqp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3encinngl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3hwkfptcs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3pfixzbnb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3huewklnh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vevcshjp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vfbtgbsh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gwbtemrn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yldahrly.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hmnyoenm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3skkizhmj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vaqaxwwg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rcfvajyh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3eesrqmil.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3urbjcapc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3cpomqiam.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3grfnnadg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3sghvlyji.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wytcidrs.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kjfqiodi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3plahwlwe.html


<!-- 参考信息 -->