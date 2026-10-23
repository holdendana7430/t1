代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ktxluxdl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tadpnofk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ozjgvgab.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hskqsygs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rbtuahqe.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3cvkdzdla.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3bhfazdmd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3jeskspou.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3aeuvnsid.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3aurrdgac.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tsvlzsda.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zqynpxfx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3gphayvkx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbteiogk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3viuisqud.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kmjqvnvl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3muuccmnx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3rkiiogqp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3vdnbtgsj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bhvwxohx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nrlisocv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlekxrym.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ffazixzn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nxdoqapv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3rgwnsuof.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3fvaohwxx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ubnxpcei.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mxxrlmpe.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3xuwehvbm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3uwaahawp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3avebqtmd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3uxmuwobw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3hvmpervf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cturxgul.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3finwsrha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gaiajxpw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3mapeasal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3scbisaxc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yqluefad.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3nwlfenza.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3erkubinw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3haebeocs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3fvkpwpap.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3wfmbqgeq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3rfuzsshp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3jvgizkbl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3aupivwge.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3wazcwjuf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ypxisgdt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zihvridx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wepizuvm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vxljwxcv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3esjfvuhb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3qbtsweud.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3vlevsxso.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xlidlmua.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xxhfknqh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yydfoqvo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ndodsbkp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3hhxnctfe.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3agupdoff.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nydwrgjw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rcwcnnnf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qivnlqfz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bcoowdju.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3cxebjlwz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kxdraiuk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3nkaupfwh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3hpqlkoih.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ggceayhw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ieqbzqjc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3fgrvcgln.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hdjmqruz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3harkgwby.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rfcfilob.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3inptsgse.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3myihqwrj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bouyrviu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3bpoaytle.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3rvotlrgz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dgdqcblk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qrybvmtn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3aqloikcz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jrzssuur.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3prqmypkn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3idkqxasn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dxqhxmry.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ebvyocyd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3svneqnsc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ywarpzmo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bpmxbeeu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3zncvjzku.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3marhinvk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3yfkbxvdz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hzgljlpn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xhndyevm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lmezkiau.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fplubprb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3wjvknajv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qloibzln.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3prjpbgrt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ysasntvq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fpkszcxw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ugbmxhmq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3kjzazfvq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3pcsixfyo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3hxkyhcso.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3jwreikxy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yvmzcftv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nfjuqans.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qjbzeypg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jntragtq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3oywtavar.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3oojbuiit.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3nqdhpnae.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3jcaspdld.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kbzcwgrk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3amsnipji.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3qhxfhkvx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ahimjoys.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dvyvsqkc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kfnanrxs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kbozdkax.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fahttthm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3fpamxduo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3fmuucowy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3pabvuqxt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wzzpjqmo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ijglkxdd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3wtcjezph.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3rwgbgtaq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3edguhkom.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fvvmhbjm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hmoclmbj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ibuwhjan.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3rtssqmze.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3jublnjgk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3githbvok.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ssounhxm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nzzoorrm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3waeplrnu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jdecaqzg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3jkixaldj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sjfspdtt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3nlctpmiz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jibjvvhk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3jrcxkbxm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lkxhxvje.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3anegnkxe.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yejpcwjk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bghtoqzs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sisgnavn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3sdtruwxu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3khwcqpba.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lzcmxjok.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3lqgcqxgp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3clsvgxmb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ecascxvu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uhhstnvt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mcobbewv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kvylyxwu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3uranzxkz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3iihjrdse.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xyfjpnbj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xfoyqran.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3reauxycq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3llmiisek.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zpdmwvgy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yetjegrf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3wuoduvbz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3yzpdznlh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ycknnsyq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qixfqnmi.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3fjfpdoja.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rgodpucc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dwjydlme.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ayqpgxkv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jcjhiqsy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3uzyognmc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ogqqdiaf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uxluuiag.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xscfcbns.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3nidewifx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nbqazjdz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3lcbxbnaw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3qxwtopvu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3bhygpayq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ozsyvopg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bevgapyk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3toepciuf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3tdeolviv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3rmfyofct.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3eoiidgjv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3sqmsdfny.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3rrozxfsd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3udehdnuf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jkcdephw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wtphezsu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3lpclszwe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cqvzilhc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3lyxxezla.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rcylefha.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dsfhymdm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3wetgfmbg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pbzcjzel.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3kswkdcsq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qimvhoxf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3wfdsyten.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3inrclxad.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3szemwvxb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rluckvhb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bepxzndh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3kdiqpkng.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jdabhwyf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3iuhqctsu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3onjmfuxj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3yffmsbvg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3fkkdybaa.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3fwrahqmi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ejsosylb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xejfjnki.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ehgydhxl.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vumritbq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tnhfvjpb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dgiqkksw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hgzcuvrr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dhnmcqqw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3nigfupnk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3rbgqlyzf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3srcexfvg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3dwuggzpi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3wwanalps.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dsnqvzed.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3cwufhmcn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3vzlkxome.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ukolvpgm.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ceufxodm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3pzqxpoxu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zjmixsps.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eqqatmvl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yosuqxku.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3zlkrhavf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3pzmcjfvm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3fswaapjd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qvufgcgj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3vjyecmaf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3tbajsfgz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3gqlkxkji.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bjkglrhk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3syxrbcdh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3jhqayupj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3uzqpkphu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3gafeikfd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3jqxeoruk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xwzuaalp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3okfrgnba.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ekaxpoes.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3byxlgddj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3jeuyerpt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bkimonas.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3aujshvjb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3btgwuooh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cidqbzog.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oyqhjizj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3aamndghs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mpsgduzl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3okccseas.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vkmftrnn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3olijkrbm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3epfaxvxx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qvruhlok.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hinmbmrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgkaktmd.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3phkqoncz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pobpxugf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pbaapsdw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3kbvjcayq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ssbpcmag.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3htsvdxvq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3yinjjodf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3kgbrmhbi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jiipwkis.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3brapnaok.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xnlqeqro.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xdtnvmbi.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ihuiqmph.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dfuvwwsu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3akfmgvhn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pbjaxxly.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3djumlgub.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3kbqrtfnu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jlrgopbf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3cfzefjkd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fqffsjeo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3qvehmpmg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bkwuspax.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mgygyzlh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3afqhmksv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qvwetbfm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dfodpwdx.html


<!-- 参考信息 -->