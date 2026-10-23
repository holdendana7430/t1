代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3errgwjkl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjydisev.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3eydjvyga.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pcdcutzd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3rytqjkjb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3qwzjigdh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rrptdxyh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3aogsypke.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tryckfub.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3oswjtupu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wijwgwrr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3uicaukjk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3takpnmxw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3cxaxrevc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ncahforh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mpcbklrv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3pcqyhflx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3eecubfra.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3mkteujat.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3fzwydlvy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3yaeloagg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3chkwtiux.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wouyntcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgykrlzn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3bgslwyyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xubwhdcm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wmiwjhhg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3basamybm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mzyygsqz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tftlciyu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3drahjdlm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3lfggizyg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3tygjrudb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3buomazzt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3hspsvnnp.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3dpyjpqbt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3hnvhyzmd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zafozqgx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kqnngqbl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3mugyqpbb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rhwnobxs.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3yepfqiwz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3gqyatsbi.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ozytbqka.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3mabtxrxe.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3efavvoyp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3uzfmxijh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3cspkdjzz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kpdpdlez.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ojnggsjb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3naykaeso.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3zrfcpagv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3adrbjzyt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nnuedupq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lwzxvflp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3frcywwbk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3bppcwxey.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ximqcvnl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3hlpodjjh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3siraiccy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vpjiyxxr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3mvalbqgc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ezpzegxx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bmztrnll.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vjacifix.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qzqhwmpm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3mzirakav.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zkmftewz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hrwvtxiz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xmrdfnru.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jvcigcwu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zftsmqhe.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ctyqbozn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qxrcbaql.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3blucusxp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pzuatlwi.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dzpicfyo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vavujqtj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hpjjnfdd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3fjfzswpt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3trkrukmz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3rdwnjcbo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ussqwbzl.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wtkrpywq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hjfzevdq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fmifsdqb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3diaqvywf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3otmmrvaz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mttpluda.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3rtrpuzxw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gzkodngg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3qwflxxqg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3yyplzpgg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3jukoxams.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3uafawrvz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3cafolgwq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3rmtnfkzp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aktvqnrv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3lxopybxw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3inwgtzkv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ywgmvfth.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3lvklwaqc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3flkaunfl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ucqhlpms.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bzznzhpm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3iobqflpo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jhnomkhy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3xmnvnmmf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3rmkxkmnt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dnpwugps.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xhirpqnq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bsrkmnqs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3kxotsxqf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qodpxfyz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3peawkder.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3xzxwumml.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3wlkvnuhb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3mrfqfdns.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jzaesfsa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ndbjrqhs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wrbrkqpk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lfyuuhjo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dwzsbion.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dqrlmcol.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fjwcisac.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3vfmecyyi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3tarycxtc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kmegfgoc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jirzmior.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qesajjpa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3tielwybi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3acrigfzo.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3scweqhga.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3msypklzy.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ztexuwqw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3octekvnx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3lduazsee.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uerdedmv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bzbuuxkz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zdzybigs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wcsynbyz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3zdjzkcls.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3eovmgtgi.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ruzdqvao.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3zodkqlrp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gcymcgcd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vdxbvywg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ieqtmnvo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3iqkrvube.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3dqdolluw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3chubtfft.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ojedorbx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yukdmurf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rbopfunx.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3vylkdjoi.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qddahiqn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dqwzgoif.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3eanbnija.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3tkitmvlc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3fbuwtpgf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3hwvisacs.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3yqmhgcas.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zrtduwat.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ukwkhtlj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hlwotcbh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wcdkqozx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3zgyhahpd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3uboeonvu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qtkcjfvl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3mwnnsuex.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jyooihvy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ypqylfzg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3luilfdwc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hxmlscpg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3aqekkcth.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3lcfurdou.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gehhpyiv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3swmaaqcu.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ppgejmqe.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3mmlukpit.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3etgyuuoi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jsrjjosu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wslicugy.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3yxxgqdta.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wamnewcl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3tppgqibe.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3pzlyyvcn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ylsfwoyz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3fwmewjdl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3soqxfpof.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ufufuvtn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3gwdbsrqk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3uyznxkds.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jvfdoqfv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3gaiamceh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3wkimpdgf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3yhnsjetn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3hztpmdsi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3lryzmsfn.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3coyyismf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3adpbltxh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kihvdock.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3cdnoxhyk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3sstkrhny.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3fhakvqfa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3dfwcrlih.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3psqsnnfr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3hbgsmgpv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3dishvemd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xeluzyzz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yryqlxpv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mbofitpj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cxsgjyxf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kqqadxnz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tmrvkzob.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3tflgwoox.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3apzfoxhy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3oiveacpd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3vkpwfjut.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jxxraztg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cwuugndm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fnbvmxij.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3sircmhdm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yhstvqyf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3jbgdiyub.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ectedygf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lkrxrfaq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xamdjecg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tzdenqwj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3xbgzqzhi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3aheppvuo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3wcrrzvdj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vcfiqjte.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3hiroqilx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3xbfglzgd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3bygjmxzx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ffootbws.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wlpvxmlz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lxslmwty.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3gxbvqqvt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sgbiggqf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3piestysb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3rbpodisb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3yorzvfdu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ceixdjvk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3orggmsye.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3lentdagz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqijxwla.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3piwgocex.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3hzoadysh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rtyoatrq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3gqoxdozy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3zfiebxsf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nipaqqba.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3alkdmfbr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ygkddmdd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xqavfnyr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3yffprkzq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wspissvq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3sdxnozix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlrkaeto.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3lkcniwsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3auakgkhv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bsssgjpl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3qxnucket.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bjcwywzg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fushnbem.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qywpqbyb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3xtqajukd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3bzrihsou.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3nfnuplvj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eqkilqub.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3illnoqoq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bwnaewwu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3mqhdjsef.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fqwchedt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uxvsyjjq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3byyhqqpv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3mseifwkm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qptgvlbd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wcedqfyp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jpsqvztn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3koingxrc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xaichzsb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kixqsist.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bpzmyiqp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3klkyfcms.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fobzekzs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3whihnule.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3muhhyagp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ewgdkfop.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ctwjwldo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3lhnkxrdo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3riuwgqli.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dekdceca.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3siooggdj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3eeodfedo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gvzwijwk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zxqnswjt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3txdggofz.html


<!-- 参考信息 -->