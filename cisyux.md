代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qhqgetvd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3cbjotxrc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3sgajbjwb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3cygbspec.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3haqazwfv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3npcmratd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ybhbbstn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qporvmlh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3sletsfva.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3wjsmtubv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3mzrzevbx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jknxdleg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kxkwimkh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3xlvwlqct.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3jqqydrko.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tqlfoesj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mawzzomw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3abhpnstv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3huaggzak.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nywhfdpd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3jfaktisa.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3khzoxyhk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3imatteba.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3tprtyzzz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3avgpgbag.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3wvjqasja.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3hupbxwwe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3tkmopinv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3lypmvvil.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qsxtcssd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3rtsrhqbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctjizyys.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3seqqtdmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkfdlymb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3orcpuuvl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3pxqndgqn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mtfmbqyo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ykljkiwv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vpxqfpps.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3xpqyosrb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3iujmufvp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3frwzhyak.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3tsnxxjfz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bfbgyocs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3qrilqzla.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mgeihixi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zjbglbvc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ohzndvsy.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3zdurrtgy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3zxoiugcz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3waqdabup.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zppztlbx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3binnpygp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ymmrdoes.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3jwtbtlyf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3qbrccxfp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gzqhdpmw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3srxmvlyz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3nfshhcam.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fbttnnvo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qggtpdfi.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3fdhuexbo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ducqtaex.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3stjbfuac.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3uflweyto.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qqcgkxih.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3vriijlqk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3lxzhvtke.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ujkrgjzp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jfrrremk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3gjugjnpn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qjxthzme.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fvvbhmcx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gjahqoao.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3fjieknyk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3hvatnwbo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kzjiejho.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lapbkpey.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3osrjzrhc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3pldiuamt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ckmflgji.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mfcehrhr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rvdzyffi.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bhkbrylb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3uucnsfpt.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3emzhszqv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kekoufnq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hnsfzdtz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3wvrqwdlb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3idlfulmq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qrpquspa.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wkixlxre.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3epauzrpa.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uckahrlz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3xfxfqfpa.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ceusyvza.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jmtwwwzf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3oldxymps.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zoogkumy.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3wwqriqna.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3frolglyb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3etiqffha.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3dltnqqgf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ecuzlqbh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3filgochf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bwwuvfgh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3pmlruajq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3eiftcagh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tlklgkhl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3kbowrgat.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3wdgzwtaj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3nimylfjm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bcgjysik.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pugxjhnw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3luduiqjs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vkxiqgqz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3eyvxzgvk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ntdghpbc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lemhlrkf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vmzckntl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3dgokocec.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3lrnwifgx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3raazpgpj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3uhnpmhtx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3nfwgrmcz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3klqoxsvt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uojfvfgb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jbrifllo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3hubgxxup.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3nscrfjpv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mtdtuqub.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3jzbtyhpu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3dyxkvrvk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3brvyvgix.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kqrwlxak.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zosirbhc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ghcudnkn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rllecoht.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3qarxvsfd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lindwhsy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3xlxnggpi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3jctjrmjn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3osibvftz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mtvghvih.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3obutpstc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3iuxendhi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jouhynum.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3npwsqyae.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3yldtgwfv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3gscirkke.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gohhwwqg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ylciezmr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3qtyjhife.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qmhriyor.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rilzgxug.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3teoqzdxo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3jloskztb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ugceqbko.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xlhejzhg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jsswbqgx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tsgcttfs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xuuckrln.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3eixptckk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3oyufxliz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rsnfeehx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3rtrrpaoj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ztrrmkbd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3dlkxbayt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3tifhzabw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3czqkbnsw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3aejjxtjm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wdxxjmfq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kzwhcfuu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xkfhqofb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3zhcbyvwh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3emnknxxx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xzyphkgo.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3raogteto.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ynxrztjm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3obrlcohs.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3xzedjjef.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3cqwxngku.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qaeoyxzc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3dpolrshv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3stpjdypx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3dftretgg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3fhiwtjux.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3iydlkwny.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3hlauubfo.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3obdvfqcw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3dnobwurb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3iqsachqm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yccrtgit.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3hhqesprb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ieyrfxrp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3givwesgs.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3dplpuobt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lqbpgoom.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3gwrzfcek.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qvvfuonz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fhcbtaba.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wsykgsdy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3fhhpurou.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3moctyaxb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3hbzdvjxk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cvwuszhq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dkqkhlxm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vzxichgq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3elrjhuwi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ifxyshtf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3zmtgbxst.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3whkfqnsd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3xqvjkwjt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ezgwleux.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3qbnbtyqj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qhpuwhsc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3sbtaebhf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sdwxavpw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jcqwpcsl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qrrhlodj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tfhgzkgz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vtnniadr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ayilhmcz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3gahtbdrg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3gvqfapvo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3yctvvwmy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3keltrrue.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3mxkmfawg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fyffjlwn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3iwcqhxia.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3nmurqbnz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fohxksdg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3oizersvy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hfqllyir.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oqcynqwp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3muaxblpq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jhdqirvd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3fgkuiabn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3uyiuwbxu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ritogrwb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3gmmrtawp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3rasllphg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3tozezdad.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3inrzlgcu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qnccbigu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rdbvrztq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kebrblrd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ghmuhgxs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3brhnyypm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3rslkefjx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3hnfnzrer.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3spksvtdx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3brygjpnc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3dtnghvfl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3gwttaegk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3flojsicb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3odxfnklz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3kdogzznb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkksfrbq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rswfymao.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3gxsobzrl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3uwvwvlcd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ligcmazj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wvixtqzq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gxtdsxoc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3jojunqnn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tdbmffjj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3erywnbwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avwxsdly.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3mqwbzqiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chxqphnb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ximiguvu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3xnbfpoyi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tzxiadlw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qbaicedj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3iiwglgsn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3izkadwgf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qdvriicd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3qekjtcjx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tlcutvlf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iebiplpq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vqwwczyt.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bbebrjah.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pzgapnpu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lhdhjsbe.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vdhijwgf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jihvkzye.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3echklpkp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3haaapnhm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mhvrssrm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3gxmqxfja.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jdznbhgu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fjftkthr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jcczwrdp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jmsgyqom.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kfcaaxof.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3tunijojq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3zdrxjhtq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3gxettjso.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iidcxckz.html


<!-- 参考信息 -->