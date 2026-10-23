代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdxbtpkf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hdrsodgr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3cevnldeb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3hodqffdb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ngcvvayu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3bawmcceb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sylygcjd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lptqkkww.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkkabucw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3otvfwgcf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3idrmdxnz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sgqbbcoj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3fkukdsmp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3vjvxtxtx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3gloqdsrf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xwqfrmus.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngzbjfwb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3oynksofk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3sgzbujtd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xylvlhnz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3xrpobmot.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3iyyiiwhj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3gaylcoiv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3yhxkdcab.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3slssgivh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ixpxvnhi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3lyzxprhs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvqipfog.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3wonxffhv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dhoihwti.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxsvgvyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ttuymdij.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3qomtamuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfsbsrqn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cpbzsudg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3qhqpgnsy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3lhgwdzoy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bedcztql.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3thhezktg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3xpgheqek.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ifabjonn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3hafrfwco.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vuchghab.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3nwjgqzto.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3oxjscuct.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ofrnnrfh.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3klqdzysy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hvkfxcng.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kpeqsviy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3rhufwcyn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3jcykhbbi.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3mdfdhept.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qnbkknpk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ruuibhrp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3cdllfxrn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3vdlptpxy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rknlxzgq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3micgepmc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ijzszvpw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xmxdeqqt.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kembefre.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3amgkiqov.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mkqxekru.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rubaowbn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3jlivxlea.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dqxmxzov.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3pqgamcea.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3wqzmhihm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nkqfwleo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3yvrlrqzp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3qydlovji.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rvqasdza.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3eljqkdnb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mvvtogvf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3rtqtvhce.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3afptoygc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rqdcadur.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dqpnrxhk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ziwozbma.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cqxjnqww.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hpbcuipo.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qmeymofb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fpxoxzeh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mdekvptc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3cyrhvliv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nupnktdj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ifwvokrp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xtjvyiqc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ekeycsep.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3srtsfzim.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ckvmeqtz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fjqaetmr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3blpddnwp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hhfxoeug.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3lnycjdpk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3uzojuntn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ngovjkwz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ywojqvii.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ksgorkni.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3eygjiayr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3nwcqfamo.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3gidmrqbj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3zqaqdjfi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3gsdclucw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cnigqmvq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vxzhfsie.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3nskxlauh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nvbwrrms.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jogjawcg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3lsoqnsbn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3qztrkyep.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mzfhbzag.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hbafrmpl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tmyzamog.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ehwdabtr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3iusekerz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3dbdzinun.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3instvrlk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vckzncsz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3gvnpdlvj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ibmlzkoy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3qnbtlydj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3tqqcoeac.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3hacpqppr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3cxuyzlgk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3vaflsudb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rirkidbz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3whposwqj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fomutyzv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tzwotrup.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3iwqzecjy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kiyupgvz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3qenbtokz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3azneqjzn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jmxzntie.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gyckzuyl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3olnjysow.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3odcolacv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ykmdrnvp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xiincavc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3gkqanxqw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ovfvevbb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3qatrvubk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3dlxqvgvy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hxejylac.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hpovksjw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cejsrmlq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vkzlgxse.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jtvxwcxi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3cdsgnwsg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3blkqmsfo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3jopewrpi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bvwhnofy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hxfiyzvq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rfcktaoi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3duvwoyop.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ypssacmc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gkiqylwe.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tmweilqw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vlnjwpml.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3eeqgeqoy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lyoazvtt.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3rcubkmjs.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kpxemezv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3oyqbkqvp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ikcbvice.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ionjdbww.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ufhvyeys.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3yallfcpq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3vvpzhypy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rqwetxcz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zwalhfsw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jrvlkbog.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bokmgbgl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ydaqppbu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3qyvlfmor.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3bjvczubs.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mlovjnbx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hqoyozxq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ohyplqsb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3gsvbjpeb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3khrdayhj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vptfttfk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3azjjrkgb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nodbbuok.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3okvzxzqr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3crnvmoze.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3yiztsaqo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3szzlvgtb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3uunsntlu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wxwzgiud.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3mpklbzdr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vvldldhj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3nfbidawa.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xccsbbhn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3schqusml.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3yobdxwzi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3egozbxal.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3rqgnuhqj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ykmkvzgh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3jjvxcptw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3phziebyh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3xmghfkxq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3xpqtibrq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3trugkczk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3lepnazsf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3jaegdhqm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3nudgtdwg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yqbyeyac.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ycmouiwi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3rikjkjar.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3mdljtoeh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3marbswow.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zjlcaahe.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3fdmxnacb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3swguanvq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ldstawyl.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cheisckm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yjheucfx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sdjatpak.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3spfrgneg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ttmzaqmw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dattvwis.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3tspqzdgu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lausdxgg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3yybblfmy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rdwfmouf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3vdcqmkyj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lheyjhbb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3xkklornk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3pkwrqiyx.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pkzggtkr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3qwvzkmdr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jibcuici.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3rhlgctpr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3geqsidxh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lwtjjoba.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3sivvtyid.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xlgveaec.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3kuvowsrf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hfpuianp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3lsxanoxp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3nbyyzwta.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3nrojnson.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qulktsdk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zvdugkwq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lxbumkrw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3yegfjlmi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ajwkoruo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3evmcizzx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3shnrblcj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rzooxtci.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3szmlckfq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yajgnhmb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3lsqmdjoi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ucspfxea.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3yvlsrezq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3cvqsjswp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wrvevwrd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3cfnxmchc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xlpbuuzm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jgqqqaao.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sdbhqexb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3afwxldpv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3txxdannt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jcatftuu.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lvrnkpfk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3asvsztmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fffdkfpw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3pnidmytq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfcambmj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kzwstzgs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3oaoxbqvv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3usemlwaj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xkjmlzgv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dinpkjdq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3nchtxiep.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pyrusiah.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3knzsysyd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nurueyvp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vyoxguem.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fgipfxso.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3irclakci.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gsyxwykz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3upqvxyhz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dvlibrnb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ejaqfjrc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vzmkzkcr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3onmaybwz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3udmezxkl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3rtecljez.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3auglakpj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oknhsjbw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3emblgstm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xnmbqtyu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ezsxbqas.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3bitnidaz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xojavxpu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3gnxwywck.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ayoogohk.html


<!-- 参考信息 -->