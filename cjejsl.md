代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pfamssem.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hkqiurny.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ejrnwfek.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3evsfjnfe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlwpuhcs.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3lnemssnw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ilcmybsi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ecuuwiod.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gvfmaoes.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ynqkwtzp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cyhmlvdg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hixgzucj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3pcwotcqp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3elsfkiks.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vloliwfw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3iagxffvf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3onltngyp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3doadqsxw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3doryqbwk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3soazayxi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cygnteql.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3zhejjpob.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yynuubgs.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dsgwahxo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3efiljdvr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3gfatsthc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3jczpahai.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3twhsfzvy.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3nuvealkl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3iwqnlfyh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vnedhesd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3yyvcdvul.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3cbbjyxrh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3xwtgiwsg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctfczidr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xspydufo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3cvnepcfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzijjphp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sokwkhjl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3yxnjttxz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kwltwupo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ntvxzhex.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3yauifgnr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ymknvcbo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ztaqxuyc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xnkbbprs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3qngkervr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3yqbgzilp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lbgygwiw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bsamqait.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zvynflbq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hcmxkucb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3junipdqf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3pkwbvzgk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3zwkfbsxb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3frpsahib.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3offhtsdy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3vodgqont.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3bzdawauk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3fefihmkn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jguddbez.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vefxqpna.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mblqdjkf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3lpsakfzm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3svyiihhx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vhhwadav.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vvgxqwvs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zxvhnpiy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3iirjffgj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3wwpapahs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rpjgusse.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3zlynoiay.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3rgbzqzsr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3lpjqubmj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3zzcpxjip.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3eezraxqx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jkrofyja.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3sjavvtzc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3bkjlqgnb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3thjeppwt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3upuxeuvg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ajeghbut.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gbovrvvl.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3yiabdvfs.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jxbnfhgf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gxaukrwv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ouomyqem.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yxmonoxe.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zwdkvmkw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mswzwmcy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pkdjmohh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3pktzlpzf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ldqpfauh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vmnqhqsq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3raiahjuv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jooyrbuc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jhlrfhyk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hronuirl.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3oscsnlrm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3rsdlxnge.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lpzzifsh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wzfzfvcz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3savbxfta.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3udujaprl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3bxsdcwxs.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ilrzjzhd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3htabeipd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3jotmmvpv.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3qzrlqbdm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3njqffcin.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3zlvmxycy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bgmjhast.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3zzsfnhlb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3periedqb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3thivdndn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3kvezvxmo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qxyxjkzq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3comqsyaf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3wyezzfio.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3gsadbqfh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jisvashx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gveczhgj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3olitigpe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3sojcvxtr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3iiuuxdzh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3domyurhj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3lxsngrgp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wahyrjzq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3kgcmdsac.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3towzdpot.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3addjtgjd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3exjmdeym.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3nsoadzfz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3laemxojs.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3grcoainm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3iteuvzcq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3kgmtihif.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3wljpxnso.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3hfqvknan.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qtssjexa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ewgihjbc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3nqcptqqg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3vsbotwkf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wizxmdpu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wojocynz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vtxvwxkt.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ivlmgnop.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3blgfzuwx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bbcgfmwp.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dhswascz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zpntybsl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hkkpaqcl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3eudxsakq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3zugbbrhk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lnpjfmdk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3zxpspmlg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3urutvknw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dxywbtjv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rppezylv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zdpiwskj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3txiuoojb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qgeorvud.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rbhedaok.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kssfzrfy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3hlywmxml.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qjaejvtj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3mbvsnuxw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jiikbrgo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kbblfmzp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3xzahtyvv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3atskalqm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3uchkdjjc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qaaocycu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3dedsqmwl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3exnpfzsi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pshulpxq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bnzvdimn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zbnnewyc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3rbcnisqg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3oxxjqskj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3wwkklhbc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ftvidcpu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3lsfjpvjw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ostikxfb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3hgigoiin.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3pxqfujam.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mtlvdulp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hlgmfdez.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kqdgffhv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3lvzaewsi.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3nyvpzmkb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jreofanq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nabvuhje.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3triirxzo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3hempvloz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3dbcjqril.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mequtwzg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3iuzfebns.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3zyohxmsk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tpgvifyl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3urpovpog.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3dppaywfu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3evvxwtqi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3elfkqmzi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zzpnpglh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3hutulqbx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3vntuvafx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3eedwuqge.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3rrbobovg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xnutxlsi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jvtywxaj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vnnpnhlj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3tabnprox.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ckywhhwq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3arvhaxhw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3efnrxfja.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3yaddnsvq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3lnudgfke.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3qzzrjrhl.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3tqizcnwl.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cbjgiknq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sixmpnuw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hfhdnkex.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ofllvvnc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3plimniki.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ocrtlmvj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mksrgfua.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3aqwjnfiv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kjsfoldz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3paxquemm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3dfynxxrn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3elsvyppn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3adyichcf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ccsyeugm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fmnvvdpw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ennqipbb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3wkiafjal.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3yrjqtlev.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ahuqvtkn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nojzqcsl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3cbyeimvs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3gcedtzla.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jiokzpdx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3diggyzad.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ayctwtps.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3zegrgjnc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3qwpjlzxj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3dhhmsscz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uotumepv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rrjmdorn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cpomchfb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3gkfrxoon.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wsjoevfs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3hnghtytd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zehmqdcq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ebotybsn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3wwvxaxmw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3nebgysfe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cxcrltzl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rbqjucnh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3czdjjrew.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3odvsvqxy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3enqtdspo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3iyuwexhz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pautkbte.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zaibwxya.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tipvlyff.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3exveotzg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dhbldjdv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xtmpathc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fqrtbwmc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fdhhlszw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hczczgex.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3zoydhzft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awtedbys.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xvziepgp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3dpuujaiu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3inhcisgf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cpbzswjd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3znmlxnqr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3zxwuylry.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wojzggfj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3modbnzxt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xdfygnxs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zjmskokz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kzmlguxb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3okfuwbxr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zoonfyld.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3czoefcqn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dxueykym.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3cvpzlwik.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3btsfghrn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3rhgbtpfi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3imjifxbn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3uwolwunj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3isrlhzrz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ieayovdg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3foesizgv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vftpmjrc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xxjkjhhu.html


<!-- 参考信息 -->