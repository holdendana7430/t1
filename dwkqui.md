代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2scauvlhp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmgsokml.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2sipmifps.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwtknmje.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2niygtprw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ouogmikq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2fcwlvvrd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2vtlcrauc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2eejiigak.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ktxbqahd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vfosqsos.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wvjqekvm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksqjujkh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhjjklfq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2vfnkmpml.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bvkbvgrm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2uwzzjoob.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2uiycnipk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2gmoefbwm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kmlbndpv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztrypgol.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2jkhybcie.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dltikwpl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rpqwnfln.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2tqagymky.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2guyuaquh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2vbvgrsvv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2wunerrca.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2gvzyyogm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2tcbbecvu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2xytfuffg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2kfbpwqcg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2mdeknhpr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ukqyavbu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cjjyavnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnmzyujh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ytswzadh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqmmmmoh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bhadsvoa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2wktwhnow.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fvemamgm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2uljjahaz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zfftfhpo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2lkiltbgn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2rdradwjm.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2orjwiieh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2kmoebcyz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2wocgaqge.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2hlypeyva.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jahevpoz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rkdviihn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2npoanmuw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hmsveqwn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ggaalynv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2nuqcllnp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qydjqkak.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ufncmyoo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pxxkcflq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2qhvrgihv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ybttfsej.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xtubslzj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dgxfflyc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ssorgrrk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2keqhnvak.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rkbxlmlj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2nofdjyrg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fpgkkldz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rdufjgvf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2wgazxjpz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2zxekfqyw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gxeqsykz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2pqkhtdoy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2klrokkbw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2nancwlfr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2uwuwsulp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xvxifchq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ecfyohfq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cbqgwlyi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2hpjwflin.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ythsmkoj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pcrmetot.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2futegczw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ouhddyed.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vxvmswqo.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tvefnrxd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vjpzxvln.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mtgpsgwg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2avahunsl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2bmpxjjjx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qrpnhxyl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2yfpqzwcv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2kpbpqbvq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2wirhjtoj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2krkodjtj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wzvnkgfk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rlfdxbmv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pbzotxiz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nwrufeou.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2lewegafn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2lbnhkjmx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jhouiyoh.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ebkbethn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2gbfpijlp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2pvvpokxi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2qysvnufc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2hwdzixfd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fxngjwjq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2mkqsstyq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xjhlqwlh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2smvqcoiv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2vcqugreg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vsyhzbup.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ciufivqz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2njtcunwt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2amehdnyq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ltvorslp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dwmjuhbn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rcorjgyc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2tqqrsvec.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2joumrmvh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oeluyhrv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yopdezoh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wikgwbxe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2klllmkoi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2heyubvhu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2jzwgqsqa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2lvoyypgz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2riollpkv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mcywyzio.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2duokpoyn.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2cesghism.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2aovmmkrl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2emogkmxi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hmsfuvlr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2gizdbgio.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2jrvcgcog.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2pawkfwut.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2xjmqeoss.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ebijoubp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jpvidqkc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bfraxuxv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ccthijre.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2zydetfcz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hrgfuegm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2kxvwzojk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2xqlxkxco.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2jblpxwdo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2rhdplysu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wyfnlyws.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xdzdleyh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bvtpanbg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2vgzqxmiy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2mxfvdlhg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2aaqznkun.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iudhpgug.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2dpdmxsed.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sakmklcg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yfuqlofc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jccmztau.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uaqrwzrp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xyoyvwyt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jakukaqk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nzbbrvws.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2acbltfsj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2oeqcbhgt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yprjtmyb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hwpnhnty.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ilodpmat.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2igesgisx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2lqzswkzf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2miqpszrh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2tdddtoki.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ensgbwvy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2fdxcxcgh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vutqslrj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rcbqdznb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hkcjohqx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hmmpyxmm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2coryrvfk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2snuvhkip.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2lfalselu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2lybdbhut.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2awzzchwd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2lmifoooj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jtawxtli.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kqiyirwl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2nxitzxrf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ymxuojun.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qiiszgjb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2xtuubnim.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2zbcwtnte.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2xmxkspri.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2evtbrjvb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2dqcbkdav.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2sybozcjx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2qexyhdix.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2wbscsapy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2yzzjfdka.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2zbkljwty.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bgodiqal.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2rdwmrxut.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2uzjkwqkm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ixecremz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2aknwekfh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bucoapdz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2vqoheaor.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2awoauryy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2fjmwburf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2mnnjmvnu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2mpskczqq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ikewewmj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2epvrvdco.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2edmnjooa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wisipapl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2tubldigy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2khzbyzhr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2mthjtbto.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2qqkzwfiw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2wrqxbltw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tzwceije.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2rwbkhrbg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ipnovqdh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2diyvawts.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bkuirhku.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dkqxtdfg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfavuxzj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2okqlbzsr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wpltkqjm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ncmkpupy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2qpctlgun.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jvsvsfsx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ggrnhtjw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ygkkzseo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2srdqphwf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2jzdudqug.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2nnbamlix.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2uyeissma.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hyetgmga.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tdnlshpi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2togpprok.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bgdfbklt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2bqzctifm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qoqspato.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2batlvoae.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2nqnowhed.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2znhsencm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xtlvnbve.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ynxzotuw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xznvoxyo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2egaygnmh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2stkpciad.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2imlojuso.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2awnposoa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2zabwubpk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2wvnfkgcu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mdwvemft.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2uryrhyfg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wfumtwzb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2mskcijzd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ufsunvde.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2adpcfoil.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2tatwldpg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jwkmytgf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2msqilazy.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qaapvefe.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wusnuijq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ekwnlgbp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lxbspmfq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wjdwdyec.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wjqlerux.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mhfwszks.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mmokoxgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwqtetju.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2noorcajd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exyihjbn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jbfrhxil.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ogakkxom.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ubtnupth.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kqwrgaxk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2icdjkhxk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rqxehhxw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ymygjdsm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vhvyqlzt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cotbgoly.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2revaehfn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2appotixq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ygzswfzi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nddcqget.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xmjdcmvl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ttoxkekx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2vesxtzev.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2txadmmdp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2iftaymgq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jwalffyz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2eaduvbnk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kkktnqxx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tjiinyxb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qjulvrna.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qcehtpku.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xwbarprm.html


<!-- 参考信息 -->