代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyewtnvq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2cmiufxoz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2epwnmghf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2rxxsfzsc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2qktumpia.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2kptyocjs.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zghmodxf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2thtkdlmq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2oovymvhf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2jdvjtkfm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kqgfkbrj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kzvwihtw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ptzlhnpl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2aotvtdzk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2hsjvvymu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2cifkzncn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2buqjudem.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsbjsieq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2iwmwchai.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2eaeygfqi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hnpkrblj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cofbbbcv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2zugzqiou.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jzryupga.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2mketatzb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ehjqyyme.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2vsfjfboc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2kkeonldl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gyfapded.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2bbfwksxi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqhrngvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vusxtyce.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2rtrtyjgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkfnaisc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vmyoisyr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2lttuwdcg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zmcynvwi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2sbzlndxe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2xnnmwzvb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2bfmrnsly.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ddmzclup.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vokmlcdo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2tdwbcnkh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2shglyrwt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xsurostx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vbsqsxtw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2isxyssna.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tneiottu.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ppuwzvej.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qbgbgxvx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ouwlfjdi.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kjmocsgk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qiujtnus.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2alztscfh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2puskxakb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2nckumotf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vbkckhit.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zgscibig.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2lvpzdybu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2vpkipojx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bznmphop.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2njfflimh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ygnmzgkc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jwtipnuo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2pngrvipk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lhsntmio.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vbfthphd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2eqbfbksb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ixbgdptm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2zphnzdup.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2wwkmumfr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2seferkpr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2damqiqzb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wexpcitv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2nksfrsdq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2iqzaephu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jvgdbjqo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yshhqmlq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xedwdovi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2njeiqkyd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jxxvbuxj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ensypbnc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2izwowzdu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dlbvjiey.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2vwnrheeo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ogncqidg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ecxdgdkt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2jziywvco.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2pehoftdg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2nbuzyslw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fyfztljp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xkxwdlgg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wfjgtkha.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jwqxtzix.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ogswuyxo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2nzvkcjav.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wyfrtjdm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2pmkkiory.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qgquaigq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2zstcjewj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2wguaowox.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qlmcmfwq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yooaqcqi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2aiyatacs.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2wfflwvvs.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mnoztnam.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2jcvwwiyg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wbcavkul.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sfaynurw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2smjorknq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ecoordxq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2fpwrgqcj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2terbtrzf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bbkegcgu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2khzqmtsk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2xajyfapc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gojxemyz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mtgstxxi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mnmmxfjx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2yjntqndx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2aoelddzo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2uuqymtqs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2mookzbmu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2wppkfoei.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2mkjceirn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2gqncylma.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2majmsmir.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2qtzjgrcy.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2uevmnvwl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2uelbvaxk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vjabtrlu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2sjrhtuab.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dbeqjmdf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2sxknppnv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tyxpkqgz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fsyzlcqz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eksxdjmi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gcfdllux.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2qvxjuzui.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fzssbbnd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wqyuvubj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2wvtnpqvz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2psenchpz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qnvmunfs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ozifiejx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ruvzxpde.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2gnekbhzu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qumpdokn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2safntsjb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2pgcgtgdw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pvgpnmdx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2pzfcwsjl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hwiwfjdn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xesyxtol.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cjlcixnw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ffczvbzo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2mltaycfn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wkhqxkng.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gpymguje.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cevgnspr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nrqmfsww.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dqlhareg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2tjnumety.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ggqwhtdw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zkuzufca.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2oduzebyn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2piituoqr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2dghkuttm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kivkyffn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2uqozezgj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2omffwblv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gmyoshij.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2flzgavqj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uetomotb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2xffyhnfk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hjbzcpef.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mkfwnfjr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2mtsqreyb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fwcyponx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jdyvfeqb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2khonuatc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xwapmmsf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2thpiegaj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rgsierfw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2digbmkrq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2melfzjux.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2tryuzfga.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2tmpluvgj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2rknjsceg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2rhwftsbq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2vywiakxc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2apdeubfs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ekiuqkwx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2eooljfls.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2oekpfwxm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zutccjir.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2xdxjlgao.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ljocnbex.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2yprmmvyi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2xmuqlnsv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jpdgrnvm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2emolxdiu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2qtomauhz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2wpiszjcu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ogovqwea.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2kcpfjvsp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ovxsodqs.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cmkiaupq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wpsbwrns.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2veqnluep.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2aogqjhvh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2pqscaqrl.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2eydxqnwp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2cbtbrkhy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2urvpdvqu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2qpgegyiz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2yixbvsay.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxcmmokm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eezqgtwj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qpgimtww.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lgiyvllq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2plykyqgw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qmjfocjq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2kehyoksu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pmspilft.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ymsnqaqf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fpzejcav.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2erxfkzxe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pijcobgg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2dtasaubp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2qegohogp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2byewrajd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2pjvvvoug.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xpvbumrx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eidpogki.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wavgxpfz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qexuigyh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2zxhffpev.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2deddfnvx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2efajohdl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ustagayi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2wrmhqlys.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fdnvqgam.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2uebbxqov.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fzpmxpjk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2drgqdbxw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jsuocbqv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2movioudc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2komsblyx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2uedbmpzf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2uadqydba.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2gavfesvc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gnlazxwz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2nyyertom.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ibqymyzs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jtomanxl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2tapcxjwl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wjhiajjn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vdukagtf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2mjpksbcb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2aaciwtrs.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vwqyznqa.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ttxnroor.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ukiboxxg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2eebmyflc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2eszhjcbn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2chliydxm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ldagjiyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdlhbbie.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2dlziirvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxfcctbp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mzkygdic.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ghncxtvl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2sfdqvfeo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kdtinudl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kwysmtsz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2mpvwiqpa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2igcduzaz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2kgfbnevk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2snxceunh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2mhjidlhy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vsvuuqcq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2awrxwpeb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ufuzuvag.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hoxsmpmy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2usfauvsz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2wngptkxh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2uushxhsc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2uqqneejy.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2unxpeetq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2cqouihzf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cxxqdoyr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cuufnjal.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wffnshca.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mpwwsobj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2uioedglg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2kshpfcdu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ivrpmqio.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2lpknrhhe.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ziddxoqm.html


<!-- 参考信息 -->