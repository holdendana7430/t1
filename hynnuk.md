代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oqbcujcv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3eccckloe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3etrodyjb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dblhhbak.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qgxqdaen.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3bnpejold.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3kewuquwm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3wscagsxn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gvvpznpj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3bywdztrm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pcigjcql.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ibtnvsbi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzvzldid.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkijsykh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3eskyoyco.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dupcdyui.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3uvlgcewm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3rhwoxyqo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3dplmgfet.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3yyfqvdtb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ffzmzfif.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3lnxfvhke.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qyudtjfh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kzixwwyo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ojbhvgfp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3uucfupsh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3bgpyinxi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qmvqvhhy.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3elcmputz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zzanadgk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3imclnhtp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3tynktwsj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3putguljp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ofiusuem.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jklepzcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlbjrxuc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3cixjqdpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rncpyrcq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zmlklicm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3hdgsejcr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3nmaxjpqs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jusahfit.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3zmonlnzt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3iqhysved.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3cscittqp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3xgztayqo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ptfdamlu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zobnsgev.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ktplonny.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3sebwhnqh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3aksnwgdl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tzgilxop.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3yvyfiwkb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kvrzjxxz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3housvioy.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ixhuqxag.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3pidonkym.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zwohtada.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ycymyowx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3amucymsr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zfbafszp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ftctzkca.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rcjfobpw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3nbntzzfq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jmucszwi.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3dgqqdwit.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wbgmzoaa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kaonjdmx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vqnzflxc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xgtralet.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jjnjftyq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3afyconiw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3joqwzsws.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ilmyxvko.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3hapuqboy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cuwbbxfz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3txmabafd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lfxuorzi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vbxyunvt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ehtvonfo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wgyoskzb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lpvkyclb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3eufxmrlf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pwcthijs.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3luobiqpa.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vjzhmxiz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yyjhiuaa.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cxskyqyx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3tlisutyt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ugxnsbqa.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3dhodwonj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3goynpqay.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3abfmrtlk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dyycebcw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3grdnxqjl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yqnbpsdb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lzjinaoz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jxrlstln.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3liidpnrr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ufqqnuxr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tqcznysb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3pjlkcgmm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nihrpvyb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ekotmxiq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3gowwcguz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dtzehmqx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3angajkyw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vjoevznz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3xwuwcwkh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iwcrrrtb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ywmucqxk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3uecpfcfe.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3btvnpabr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3rfdaftms.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3tfjxkakn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3wtcwlzwu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3btqjcqko.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3upqknulh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3wixtcudh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3jurpnntk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3dfuydcas.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dgivxutp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vrzsolsi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mlzpsicz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3hjaecdlc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3toswytxo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3uhnsxahd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3obqkihgs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3gptwjllv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hgpczktx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3trdehsce.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3hiqvwbyd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lrzgucej.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rvugodaf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hnoekqma.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kfhxkktj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3fakxtfek.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3iagkuljw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wudqzdri.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aahnjmoz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ehdbnfdh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3frcbgcvi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3mhmkzuvw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oxgovnrv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3waliwgfn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3kvgxuvpx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ehzflevq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3whlydzfq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3caiaiwtz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yuxlheus.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wnoqudrd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3vqkjhvva.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ihkwkgev.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3veswrrbb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mqrsbufd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3iqzytzoa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wwyfsdhx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eeiozicm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vojxsjnt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3girbjevw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kzfrjfxt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mwfsujnb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ehqladip.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lxyxpglr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3piaudcht.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3npffgihc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nqlnhbbv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3opelmuwk.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zfokkugl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3acagqsai.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3dpnqtvsb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3xfjiklgj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3higsnsja.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3czqlzqnz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zbojynou.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zssrvxzx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3agardngt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hqdpzugt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3mjeenohw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3oykllkqp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3cjbwbndl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3zhfishuz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3utcbvhhf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vycmnqia.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kxxjvtrg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3qdlarfhz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mmkvjjiu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mxhsxpfl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mavbsaek.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3lxvlqieb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3xhqyxfgj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3okgeqlpk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ucajbqef.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3nmtnnely.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3egsipnhr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3sdymkbdg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3cajvfwxz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vavkqjli.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3mufwvgcy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3eckgecxy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ktevtfzh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3kdryuioe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3twbcnlxo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3zxlxwogq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3uhyipogd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3vmeqnrug.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3iaxaurfy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3iqbyxjdf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3uvxunrav.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3orvreppp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3yqrozuvh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sxsqpqtc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hhuelaqs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yujcdfpp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3xsbihvil.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3jafnjsbl.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3balsngnv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ghunsflb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3wtscxgbu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3szdrdzni.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lyiphbsa.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mzxaoucs.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iwpkwqju.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nacpfjol.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3shdwkgwr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqxfiwyc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3abblfkan.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3oaphkpsz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3otopnvak.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ncplooxt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3twfcfwwj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3cpmtejzi.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ihdximrg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3uwlishup.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3uwypxbnn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3wspogyij.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3fymzxaaz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3prwslqbl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wdizyalc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3avkhjtpz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iwrhephg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3sgevmcso.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3heuonsfs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3djptaabx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jizlculf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3jxlkqago.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3pcceecjl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3cmevfmwi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3velgktpl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pjihzgjk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3klvwieta.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3fwermdbg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hwbipiiq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3yaycjlms.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3nsibkjim.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3yrhifbsj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ssjgdmds.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3svgwybep.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jzrdgqiq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jprafcsv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3bcdkeibn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hrchxkiy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3csqyqopf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3bzxawjpz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3rzyvmdep.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3puqpbmeu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jhtmvmfv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tycyscqt.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tmrwiiqt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3aiuonndg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ugnjafsf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yinpiecg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkufpemk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3fndnzmcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zomfbwpi.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qvhsbtoo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3mzarroag.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3dvpchvbc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3elxmimii.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qfasjrzg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3lveqrhps.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3nodybjep.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3uocadkll.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pshqrnfh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uaprbkke.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rxxnqpyc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pgwrjatb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ikeemwyk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rgjnzjav.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lpugcaow.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3bjysghex.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3oygxubkk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3gwpmlxhd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3elfyuuis.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3yhvkznqw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qngolnch.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dpstkqae.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vkaiqpod.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ielqpwvu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qcqykhjw.html


<!-- 参考信息 -->