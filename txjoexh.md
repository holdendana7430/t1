代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/ggxvzsooc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gqkhqkqim.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gdpgukjts.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gpcgmxyrg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/ggwbdvkps.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gjidiuyov.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gprapiwpn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gfqlhneau.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gvavmumfe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gtnmwpmga.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gwonumcyk.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gcgbrjvad.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gohbmcpky.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gnvmkiuas.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gglpasdfr.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gwnkcivmm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/giheakyxx.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gqogpyvzx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gjtgrwemt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gxwgpmpkk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gvmunnpdx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gevwxzfoj.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gfqcsgvpk.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gquvdibet.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gzumykysx.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gpmmqripp.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gwthclkph.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/grpcqzvwd.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gfbwuzgkr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gjqxjauea.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gkcstzgyg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gpxoiymdj.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gebetajfl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gajwpjibk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/glqvexalh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gveetaccj.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gvxopuyda.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtpcrwira.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gzuxcgtzo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gwbxysecz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gkhpkdlom.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gbxbxfzlm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gxxxctvlv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/ggiwbauwv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gnusgbmoj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gbmzrrmve.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/ggnbcwiip.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gvyuyofrq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gzvhljzhv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gintqojiq.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gylpnwxos.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gkzmrqgav.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gnhtqlfwk.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvlikxsg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gtfnwyuta.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/guaecfkwu.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gunrtxxoa.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gflullwvg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gxwdjmtdd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gobboaexa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gqugftbok.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gmdhxznuf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gxvaoxkcq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gdsipowqt.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gangxrxrz.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gqpdbjxlc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gldlsbzgc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/ggaobfvzn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gophjgsul.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gsqdjaiag.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gxrdhwnwk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gfjvunbrb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gndhynguj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/guaurjfdn.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gqoktmeos.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gyvgveodp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gcpfntsey.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gldyceuni.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/garixyrib.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gvquzzmzh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gdlqvykkf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gjxpyscmf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/guecttexs.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gtootsucl.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gjpinkmnv.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gztrxzkma.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gbqnkrgqd.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gybswcfqu.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gdozriign.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gyyyxgovi.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gpfixlfdy.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gznwobosg.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/ggkxrvbtd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gfjebwtqw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gzbvyuwnj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/guyvntooc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gersgmmep.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gkaezaxeu.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/ggmhmythi.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gqcydjjgr.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gvyewijcj.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gyonizajg.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gwoeqkxgs.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/grpdzkkkw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gxnnepyld.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gpuhldafd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gmevcnfba.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gztlwkulm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gjczixxnx.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gyimnolue.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gdueticwo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gbmbamxpi.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gwtoyjbhz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gimoqkirm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gjyfhmqie.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gsnjsynyd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gmoswjice.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gxiurhivf.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/guuvhytuk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gsnmcrjkx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gkdenepuy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gbldyqevq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gsxzbulmg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gjcbokrmt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/ghvyibysp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gvewhohbd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gacngslcg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gukflolht.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gdqigkgxa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gyvtirwtb.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gzluojlcf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/guqqcolkb.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gkwhpcncq.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/guvlercqs.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gmoofhtte.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gyxtgymne.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gcvqfnant.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gdsnfuryo.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gnimpczlg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gvyrbnjdr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/groaiuole.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/giaziyjog.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gtkylqrco.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gseseybum.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gkwhsiazn.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gwbxkcrzb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/glqovujsb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gpnxbpuyc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gzzwzqpdn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gtqlxwkvv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gbbewkuot.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gpkfiyfov.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gfnehhdff.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gbkywabwp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gejpwmxwo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gnoompmwl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/ghwjzjvdx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gikuoasee.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gznxfmaja.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/govzchfkb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gksjolika.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gjgrolggk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gfdesozmp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gdsdggwww.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gmagnqcfi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gyfgtadrg.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gmtovbvwx.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gilooyind.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gupbzdnri.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gfujpilcl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gvfurzwnv.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gtkiyoebh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/ggtsansqh.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gnxcdrjvd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gcnzonkom.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/grmvcvhrd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gmgyjvakm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ghqmfwpyo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gmcdvksck.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gaigracpd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gfnvoqamj.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/goyrdmkye.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gheijretp.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/ggfnbejdq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gewjoecam.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gcnchxyck.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gzqraelnd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gpiswajjf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gezpfhvsy.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gemfjfctq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gqbwyurwg.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/grfrygoex.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gkzphmbro.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gctqhpfng.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gsnamzaav.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gsojhwkor.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gveewxsyp.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gbhefnpey.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gtwgkcefr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gczubxiyc.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gxyyubfvh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gqidgmsqm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/guuuusoyy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gndftijdw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gokceykqi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gfcjlfkfl.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gsvseefbm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/glrfycngq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/giopvzkpv.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gjyxhjnft.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gprxranwr.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gqcjoxlrv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gzaouuhif.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gdbbocfmg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gauzpijcn.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/grptlkxjw.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gafrgptqr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gwoiazenk.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gfwozgfog.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gzltktmbi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gmbiugdxt.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gzridnpvb.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/ggvbhbwht.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/grojlzbyh.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gtflqlsdu.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gnchyddqo.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gvyrgjljd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gipbjckec.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gpfmjbyvd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gyhruebau.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/ggejxuoyu.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gzkeismen.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/geaapqkui.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gxqqgpodn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/goekhehmk.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gbosriysb.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gsypthiyb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gfjtkhewk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gcysjdnnf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gqobjilet.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gljdsmxct.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gmwhcsoyi.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/ghvxpywfn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gkirfvsff.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gtmyuxzss.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gvhpnsyts.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gvbdnlqwy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/glhhrukya.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gepgqedqk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gsbgwfyls.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/grwifrawg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gqucrpmcu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gqzxqjgqu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gdmgcxqwd.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gqkdylfrl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gmjxtsnyy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/grlaiktqd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/ggkepetqw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gefxgmsmc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/goieogsmq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gsayntoeq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gulyyvise.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvqfwmsbk.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gobwdksvv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gspvuhavg.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gohumzrtn.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gnazbwixz.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gzaqfneqz.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gqejrvutr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/grmyblqxt.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gjwcyeijn.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gzhmhduso.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdwyrnltq.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gazctzzbx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpacrfvkk.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gspdtpjdc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gtqdzmloy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/glkgfmsrs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/geprciemf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gqcsgwqbf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gqjsygwfm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gxoyxfqks.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/geqeuuhdu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gwbmhrlgx.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gfmeqahfo.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gooskjste.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gkpmmqfka.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gmrmkkdrj.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gguecnzjm.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gmaysduex.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gluwgbiog.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gveoljnyq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gnqcoucyl.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gbchicpgs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/ghqeaqnjp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gzxbelhqq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gtphbrmdw.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gzynmeugt.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gofkpuuyi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gefrrkzfc.sHtML


<!-- 参考信息 -->