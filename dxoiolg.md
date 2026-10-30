代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gxuqzgqcs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gomdvtgnb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/guawgjggs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gttatmzmp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gfmkqemwg.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/grhftcsbe.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gyhgaogvg.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gvadpooap.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gmckgdjgz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gatohelem.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/grfcgpygj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gnffercub.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/grtvbciov.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/grtujxdsw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/ggiawwsuk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/ggrmxtpfv.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gxwenldcs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/ghxoycqsw.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gyrekakav.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gydaqomyf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gnjdebmiz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gllskabwm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gdmyafebw.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gboydrnod.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gxrbuinxr.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gvhapbaxa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/grfeqaihe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gscpnrktr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gmmkebrbo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gxhmxztqz.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gmwetiamd.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gqgvtqiqs.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gcflpaenc.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gfsaadkvn.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gtczvbxht.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/ggsjhhouo.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/godlspmks.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/ggvbapogk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/glurdokgd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gqhqieuxz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gdoxmalkp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gsihzkyoe.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdenhcugy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfqamiiwc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gbbynmtmt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grhdycydg.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gmhbrmnoi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/glxftmjwg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/ggnrlarpx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/ginlqqrde.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gjkyvovkz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gnxcphqeo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gycgerrut.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gskziqxtr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gnbyhpilf.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gvwzoblgc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gopvsdgqz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gxbillclh.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gqopripzj.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/goudwpgvs.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gkyxlowhu.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gickogqoj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gyfhcdbke.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gqlcpotgj.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/ggpsfvazl.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gmtbxwqft.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gdktqfuiw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gbwzqzhbl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gofpkgdba.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/guyyftipa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gixtigwhz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gnhscvuyw.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gkvjngokl.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gwtomvjrn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gsnjcwfnf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gvsadugnx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/grfwtepzo.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gxrahvsgj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gflnsbnui.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gsdsxvlpt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gnpdelxkk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gfhvqfysx.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gsggmblnl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gnznwchra.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gtqnvncwu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gublylsgr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/ganitthxj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gtadnaqbj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gcvxcxqdx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gsgyfbjwk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gijblsnla.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gkskwkjya.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gmmnixqgl.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gfmalpiqh.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gryldckvg.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gkfazsmok.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gmngkeety.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gsphzuovk.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gndlsafkd.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gonmecijc.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gwrinrjbi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gyovylnkq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gczbqgdeh.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gukmmunuo.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/ggeteylyf.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gcuurrvah.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gfsrnrmtk.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gmsfhskbe.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/ghbjupjdc.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gtdavnrbz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gazgxhagf.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gqgtqhygb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gonurihdg.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gplpbbnpn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/grfoutfkr.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gpgyoedjh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gtytpboxj.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gizpmogwb.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/ghqpjvfhf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gbccvrwoi.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gfkmpzirs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gcgzkyxqk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gceraoeqj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gjkzupodh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwuxvgglz.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gnzrepxec.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gfwvyydet.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gyfxhafgo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/grevizxvd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/godmrsyin.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gczfljwgy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gcpyetbsw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gkhivronf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gqmzphnxk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gwlnntvim.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/ghfedlziv.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gvcgpdolg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gvofwgmeo.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzduzwqba.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gwgabnjeg.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gmoxfnqmk.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/giwwylpnc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gskuguiar.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gfpquyqwa.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/ghpdlxjpu.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gvvvukymz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gevvsxgxv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gkszihpnz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gjoxjibmo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gqizlpmvh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/guujwfows.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gxesdqwsv.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gnpcbpzbc.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gtneuyerh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gksmahxxe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gwnkegdnz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/guedebzgn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/glyapbssl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gadiuyura.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gczbaiwcg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gklmetfmt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gelgumray.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/ghdjokykg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gljwkvgiu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gyiecuetz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/grlnltvom.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gmotqzapj.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gbgfdqxvc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/ggktiaidp.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gaaivmsbv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gqctxqhwp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gzeabrweo.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gnazwnvyx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gsotqkvkg.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gqxistcpc.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gyezmgtdi.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gjqwjmyxo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gsspolvkf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gqmeuhybx.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gnxoeaoaj.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gknmsjvjm.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gtuvgfujh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfgsgcyxa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gsqcbkhwf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gkvdesfvf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/geywdwtob.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/giwpngfnu.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/ggdvexffu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gjzhyalfp.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gsjyubozf.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gjwcdftgv.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gkrwtqqsw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gtxrmvdpk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gktwmiptt.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gnmrkapjc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gtbkhupcu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gwvsphyvg.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gyclsymtj.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gqrsylfsb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gsxiemvix.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gubsqpowc.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gptcxwixw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gkynyofej.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gdxvuyups.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gvbdzbffv.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gottzdsly.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gmcquwcuy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gregylnsg.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gyyornkkn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gjnjspzvb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/geyipkdbp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gzaidxoot.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gyishlabo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/garpixeet.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gkojzjgqf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/govielepm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/giyjsftuz.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gwleqiqah.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gyajffesc.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gxrycsjqo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/ghzexxyji.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gasjdeuwd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gqrqhntsg.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gxbjbuoba.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/grxsmrjdt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gcfpbunwf.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gigxmqyby.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gcfhiltkf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gjidvgdza.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gqeeyqnbn.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gqocptjha.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gdfqngzqa.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gsyyjnbyj.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gikgilzsv.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gujyvliqy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gcpcaiaav.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gnlswejud.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/glxaikzty.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/goazfuokt.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/geujsazzm.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gesbxcgsl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gcbnlhcpf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gqiqbwoye.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gvrhrdyez.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gdjtmrbwp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/glqhexmzp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gsxffnezg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/givpywapy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gacswugrb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gzpjvfrpy.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gyelrccfk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gmrscndei.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfxztqusl.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/goqdrneqk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/grmhzbqnj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gpajwiawd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gmywmkcti.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gimednqlz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gtcqmklst.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/ggftkejyh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gzkbbuakq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gucvsvagx.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gedxnlwbh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gjllanneu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gfpbhornp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gkwrrdwsm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gjtojziiz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/grnyujrjt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/ghogocqle.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gjowrefxe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gfkyegbnf.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gxbgyfmqw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/ghuxknbkg.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gsckxcqnh.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gkeogllgb.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gojewspeh.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gfnvcanpl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gmtsollup.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gvpbfgkgu.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/guypodrtu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gujjbreyu.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/geknzvuoz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcjkilqww.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gwbzrwfcv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gtjycguvr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gcllmqahl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gklxyftpu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/ggqkjicpc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gbvedoejd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gknrhdxil.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gzrxvabmn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gworzlubo.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/ghjfxtjqx.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gqblwyfsr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gnaffsoyq.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gpbgfuhls.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfyxhhfq.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gacyvwjmj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gxnhgplqe.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gjkigombw.sHtML


<!-- 参考信息 -->