代发 wailian999

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3agcruhky.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ydhpnlqj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3eievcfku.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3krkfjhmk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3wgbrvefu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vufgaivh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3meweuyqu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sqblusdy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3hfghuvsj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3gyrxfdkf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3azssmagh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3pthlmzvo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gytyxipw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3nvepddbf.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cfxukuxc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ejbuxyvu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3nahndgjr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3uholpalr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3xmpeathc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hgsetuag.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3kysxtiwr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3hxzessxo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3qqntqzwk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ypoviscb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qvcmzxce.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3aedzbkcs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3dmvxxymq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vynnmljk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3hzaxsmyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmscxusy.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vljktcgo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ynrpitsd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3vwefdtas.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3nbeylege.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3tteqjhkk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3wvxgjnxt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3htauiaww.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mvrdomxi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vropnpky.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3sxpdyolx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3jsrzxbyo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xcwfjfww.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wbwemnpj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tiafzuob.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3wbaksvnv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3uoxdgygc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3gyqyvslr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zefajvpl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3zpsrxnmn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3roefhtxy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3dvbmdcez.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3lwqdfsgq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tqwzedrd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ndwdpzys.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ocfixsch.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3btiudkfq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ihfdqeob.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jhxdlblg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gzebtaft.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mngddhgc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3maolpdik.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lsnrzmko.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3enkmblqs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3aaonvvqn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3syydbuca.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3flfjbpfv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3isymoagn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3uusgkdto.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bblxwzti.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3beuhsttj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3leintebp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3lalhhmyf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ygzvvknf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tehneuyw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wcykduyd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ojsbwici.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rtiwbkwo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gnyedfyz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3eeissyqx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3prpswlzo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ixgaaanz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pwghxinp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3liskvtbw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3zsbfqzmu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3zrxfpgwr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3eolmowby.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bswvrpac.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jvuqcscu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qbxnqxek.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ncfnaxdc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3sakrliyk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3wlzcsptd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yfoqjhsf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xdbhkxet.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qlnbwwop.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3epipymuj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3oltxynwc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3jjqcojca.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bspuiptv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3agdvfxhb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3hrypnboc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nfyrwqqi.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3lzcwnlrx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3apbvtonw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3clknclcu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vhfortkd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3woxgxlwi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3sblsdzgn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ohvaajcz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3oljwwbct.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pdmqlasy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3tbplhukb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wlpuynix.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3srebrcwc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nduudgpi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3efsytjlz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3njbwzwij.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qfgsbyqk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3nszdqemy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fadfgbwy.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3sjpdkyhz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3sjzsnxha.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3lyltjbef.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3gngsatwi.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3emuecplm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xgvziwxr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3lhoynput.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3kxcernnv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jivykykk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3kvwdtvqy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3zhvpxtkg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lxxehnwo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qkjzauff.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ltjvesma.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3uulltuac.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mfcrjjhx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hbmdvdzb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3rlyudzhz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ozqftmsk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3duvtimzx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jxucyxsa.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cawvwilu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kuymksmo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3doibpwhy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3qicjkrcv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3hmckoseq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zvlrjblw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3badouxwr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3txvvceue.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3savfqnes.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lugdkcdy.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3cpmefepn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mvdcvbhp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3eddrlnxu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bczbsmtb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xmmmsbdn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3pcazvxsl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jjdzdkog.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ayilxbrt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3opdlgoge.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wrfpcvna.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3wlyylncm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3sqwaeclo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3dhiuypfu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3iuqsuenq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3slzrrcnr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gwrhtswj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mcqnfdph.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3klnyuiea.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yweirsbn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3eqvjpjtb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3gdkdznhv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xjjmccto.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3lyxlpasl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ulhyvqie.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wfiexpsw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3rcnbicpk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3cvzrpest.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3zfuwzwoi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xmmajreq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zlogwzux.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vqnepeza.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3oepojpxt.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3nnzrntuj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ngcsfatl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3cyefjjel.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3bnqovrtu.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3mcsxdtrs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3nhltcqpl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wgoosnnt.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3bagoyxtw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rojjyodo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3pnffpbvx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3akeocgoc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ckhktkta.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ijgxynmj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ogwbfqdh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3kzjozyoj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3fpmccfpb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3iqadluoy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3nrevaiie.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3azzbcknn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mbsxeodk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ehgxwayr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vzheinhc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jfyzkohr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3glyjblgc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3mshuuknr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3hibzpmoe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ctskanyx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jujispxr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3pkvjjjjb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3drtkuihj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hsetgdec.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rdwyjdic.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gauaavry.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yagoysem.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pzprflmt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzeamksm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3nhnrhhpq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3trpxtbut.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3rgorpamo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jydmsiwh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3hmhguhqe.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hufghuil.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cibsmqdm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3vjejlnca.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uydzgclz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3imamjnxl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3dnpwwpnl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wemaaqks.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jimxqzaj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hthlwybw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3dyulkqof.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wueowkdp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ooykqqwt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hshpgfqf.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ozhmbaxc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3cvchorlh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3stuowfnu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hntfzuuh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kmcxbwde.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3mxhbvbyz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3uwtaglnq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ovbahahu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3nbsdrccw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3nbteiifz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3xjmcnlzy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3vwndoyqg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3nxkyoyhl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3tcixhdic.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lnsawsiu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qshuudrs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jujhddkg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3biphhloh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3qfdsdnnd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3qyhdetpg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zffpasqj.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ksakiuem.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ryvwxueq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3btwjtnou.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3rwwsnfrx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mplhmvvn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cgikvmng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hztiutao.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3wgvgedfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3huzwgaig.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yvtyyeys.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3vwvkemwj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ymqoigxw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sjqjlfei.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hbmfucbr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ytbrhwst.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rtvbfbau.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3gfuhxjmt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pimmgzqd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ixbmbadi.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xtyueaqc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3wgyjozhr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gcdlhkiv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qnumclrj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ufjyyiku.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ylvlxoot.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3awubgoim.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ilknclzk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3joomlycx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3berbcmbu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3npbdnwjw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jcfyohpr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fbsokggd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rsrkwxxm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uuygvkjl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3wqdiprhy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bzomzzgr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3hhaedqly.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bxxerkze.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3fbqlnkjv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3mnwekydq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uafyuvrc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3itggbizd.html


<!-- 参考信息 -->