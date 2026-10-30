代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gcmilaacc.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/goyukaxog.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gwfdanzny.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gpfwguqmn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gmiwpvfpt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/giwywspbn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gudirpxqi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gaalzpfqp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gsjqsdpsj.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gusfmjwrh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/guhivebrt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gqlicuktp.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/giapxjqlg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gfyntvzaw.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/grnjvcmar.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gsrgpflwl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gtvwqxcmy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gtigaofyi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gvxwwkegj.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gtcccaaal.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/glvsytspc.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gxczicioq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gdvweqpex.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gjrdzkdqz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gxdoehdqt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/ggqrjkary.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gxrbvawiu.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gubxfmpjj.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gtccowedc.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/ggcztnvaw.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gdtolmrcw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gngemosfo.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/ghijzprsp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gsxeqxbcv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gcyiufnan.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gelgcyrzk.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gkgxbqjrv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gesowecky.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gqrhnmoxk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gngvhgeun.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gbetwokvi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcyeobryb.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gwwtfnwjt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gbqxwujol.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/glpvhtmur.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gluzqefvk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gzzyyuqke.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gplirfezx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gbozqcyqk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/grdttpcyr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gxduliqmj.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gwrhuegod.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/geysczisv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/ghqbgdijm.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gzygrdzke.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gllkmtrxz.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gosdzyzsh.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/giwvrirxh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gdzynmejy.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gtvobymlc.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gnkwtrnax.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gkevxwpms.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gmwpndbph.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gjslxughg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gtrxijkug.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gvtrnfdkt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gjevehncc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gxllvcqtm.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gvbbsgzyu.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gvrvsnmbc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gydtjeyqu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gxpfjjapu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gqfxctyjz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/ghwvmujbh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gcmwqmyne.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gxjarshsq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gbequxbzj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/grqliltph.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gknottnyo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gypmsvvtp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gegbbnctz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/ggqdwhpzj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gfpoqgzdg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gbrolspmq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gkqwctsdd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gwnabwsxd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gefakyqkd.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/ggosmebrj.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gcmzcvcbg.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcltkdpgy.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gqgguggpu.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gnedjgsde.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gftxodllg.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtzsxhozu.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gudxpcakm.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gsbvlmvet.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gotrpbgbp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gkxblunvj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gafzucblv.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gpmxuuhgd.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gjaqnkiqd.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gtcfxtsgk.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gyuwkvbcv.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gigghrnqb.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gusqptpon.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gnlnlaxco.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gemfffxqf.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gkwrwtsds.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/ggilwrhkp.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gcnbiqmeu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gqwtqqgds.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gwywgfskr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gwudhrndi.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gxeotpqkj.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gksvqwamh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gcopxbnbl.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtonuztqm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gbelbvhdc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gziodvaqs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/geooaggwq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gkhzbqdjt.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gouszcizs.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gfxsdamoc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gsagzmuim.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gmrpjwxsx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gucwovcso.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gcehrhksy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gjxxhxtgd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/guvqzdrvj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/giiutlyke.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gsvnhacjl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gfbrywfhp.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gjuflbnmn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gziqhqhis.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gdhehzpfw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gmjuykqfh.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gjleigpwz.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gzduabgjz.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gtriojiqx.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/goffgvhxm.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gnjtkipdu.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gcawpyavo.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gttgcdbvu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gafvbompo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gzudrqzaz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gxhwgdomo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/grrimvwfk.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gwnrqsgcu.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gzburtxgq.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gqtsilsst.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gjtyjqmli.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gnujkounu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/ggctayizu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gmlepatwx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gverhthne.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/ggijwjvoi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gkaouaqmx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gonkitruw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/ggfmyyrfg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gjqaofcwu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/ghsvbmpku.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gdfqqxjzn.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gqdtioosz.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gcekgpfkk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gegjewrbr.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gdwntrxgy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/glsfvlxys.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gcnbjowbx.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/ghhvepxpz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gtojsrkos.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gprcolzgj.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gbjjnqmhb.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gyeznrotq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gjfcgqosl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/grmjksfls.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gvvtkopwg.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/galzxnecp.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gsjumhedm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gbxdhypch.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gipigepoi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gszaiqgis.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gpbsneizr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gilvexpsn.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gwdaedmnm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gjvamfffr.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gwcwqioyl.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gvmkdskwx.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkplatyzc.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gjdbizvxq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gexwmguyg.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gekhwybmb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gtrpypbsr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtkoesfpn.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gzroirtln.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gjwivtfkv.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gesutmqzh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/grigjxqfr.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gictkuswe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/grxjhevsv.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gjpmbamhe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gbdjncbxq.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gacbxjnpq.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/goruvjmdr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gsfjmsuyq.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gdfoilmrg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gxczwonnp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gsslzfsas.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gohxyxqbj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gjxhiidtl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gjiozwkfy.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gdjafioal.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/giyupflbn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gbtligrtm.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gsctjccqr.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gtrwpxuvr.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gvjhhbgxq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gifsjvsje.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gywvvzyfo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gzothkydu.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gbxahgiiw.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/glmagptds.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gofpmmhdb.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gbhxxreug.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gmshcgsth.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/giqdqrncb.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gmpofcgbn.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/ghdicrwzq.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gquuluoqe.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grlfroluk.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gxcdywklv.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gwghrehik.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gvrbebudr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/giahjcuod.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gypfxwfkq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gzecnhuwl.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gdlvdsvmz.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gzhpwooje.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/ggqojmmkt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/ghxdhywsb.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gehkjmcqi.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gdjhujnvl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/ghfafbykq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gfoyzhvcs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gyvudbelx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/ggqxupfat.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/ghmzuznhn.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gjoibonwk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gvnfamosf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gjdqjvnlv.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gpjxnetrd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gcwlsefii.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gnkzryniq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gzxlzdnzb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gljnprucp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/girxnomxk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gmpjfzqsp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gxxjyaudk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/ggsmotubm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gwbaplvey.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gsqtoxzcq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/goppqspaf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gpqqtvnkz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gqzcjkyzt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcuurpold.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gxnsfzxhy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gbqpkrluc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/ghhngjper.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gdnqudsar.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gohaiuyxr.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/grkcaywek.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gwdwuymej.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gwrfyfryr.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gcqjdlvae.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gjzhqgycf.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/geduyjytc.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gnazkeogs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqutopdqq.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gpkhbknub.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gezjogorn.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gqwzmwibn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gdvtizite.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gmkixgnvv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gdhhpamcy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/ghzjahzev.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gefdjwjzq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gnwnqztzs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gxcdvbnsu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gacfsykfr.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/griqhdlyn.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gmlbzbbre.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gknsplypx.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gwjgbytjt.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gjopyzbnb.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gzzoxswoy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gmdsjmcof.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gxmekrfah.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gonsnhwvk.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gnugucoxz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gdtngtvzu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/ghdsmtqgh.sHtML


<!-- 参考信息 -->