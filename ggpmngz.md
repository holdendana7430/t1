代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gefobjqep.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/ggemtnuvm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gxdipeaaj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gdfrtbwhw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gcrpcdyvb.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gnefmhalg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gcoopmead.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gqtvcaesv.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gqdmahaxy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gnztxjczh.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gegnprcdm.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gpmhjgsjh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gfsglnzqq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/grjlzzkhc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gwezclyho.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gutewooad.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gvwaljijw.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gvisruyhq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gflqowxhu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gjxyuawia.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gmljohjcg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbergztlp.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/giwtjnobf.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gvsjfmbnf.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/glhczzraw.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gssvwusej.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gqsgaqrjk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gbpwdstni.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gneuepdnq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gjayjtril.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/goybkisuu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gqteftvjj.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/ggsfmkgvd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gcwfqizoj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gssxxpjbo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghgguyptx.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/ghaafpobo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzatyfpvc.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gsgwnbjvw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gqlpmspwe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/grzlesxyu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gjsgklegu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/grsweopvu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gnaplscrw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gqhvlsunv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gjxbrvzqj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gvycmxcod.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gyyvtdrek.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gqxdgugsy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gtmxcqxxf.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gmdzehxxh.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gsyolufba.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gcmgzpcdx.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gpujzqufh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gaxwjlxka.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtmtcifjc.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gbbemizbg.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gpqwpfmps.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/glpqjsmtj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gzchrnbsf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/goheckaqn.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gdgdwicjo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gnjhaojel.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gvkncpvze.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gtyhoktll.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/glfqdbhoh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/graxkrxxl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gxvptvfll.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gmnsptwcr.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gfmlaepcf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gqafejrcg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gqtrpdzym.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gvjgqtwwc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/ghrexiwyv.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/geyuhnfim.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gjpcjysep.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gregbtzzk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gispvdlgx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gjqiwwxdy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gdnwigunl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gcszrftdj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gvugswphv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gwxgmlusn.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gqjulnfey.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/ghcahoett.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gosgqpedb.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gfezmwqxv.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gmtjxbjcn.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gwnewdlmv.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gjbnvvreq.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gwncuradv.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gbcjnsetn.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gfekdxmsl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gpmickova.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gzqlpesrx.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gjrzqncqe.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gwbgfkxas.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gcyrpkuur.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/geapjrwsp.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gqujczawa.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/grpchaqew.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gaslixpoy.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gofkdymbx.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gujkamtto.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gfqhbrcnq.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gxtvkhunn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gmpxjbinj.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gavxyguvf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gficqrptj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gtwtkdhfr.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gbejtlpej.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gfvsktskh.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gcqcmbdwu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gheoravvb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gdgbfeolj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gljeyezpd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/grqqmutoe.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gqavmnrrg.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/glefxcsbh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gwraebdmt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/guihohual.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/grqqwvxnv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/ggoysfbqz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gvkujmrfo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gaqvuxife.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/grltyjmsp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gjelpqmcc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gavltvnpm.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/grgjgikcx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gcuoedixu.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/geiuynjdm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/ggbpwqaoc.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gdokvpuxt.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gqvvuhcpw.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/giaxefhuy.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gsnhwhmpx.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gduaovqfs.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/giradabds.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/glnkgjuur.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gwkgdxdfd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gwmilfcca.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gzuaemghl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/ghlmallhe.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gcbgwsdnm.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gylmityst.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/ghnyuzrax.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gckjpignp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gtmvtgglb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gmtmaovwd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/glcrbpnbv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gpcgbynun.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gwpkcclrp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/ggxwphomp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/grlknpmou.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gqvyjqgvw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gitpakclr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gijtmqmqr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gvcnyiyrj.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gfzqrecev.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gaypntcfs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gxrpaqaks.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gcgcvfbtl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/ghofnamxl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gnkjmqydl.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gszwfcwbs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/ghqmfzitz.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gilpuluit.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/geqgjeybw.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gltbtcwdh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gjhjtweoi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gikyfyjlo.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gsjtgvbpr.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gushboqph.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gcqqsddkk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfecrostu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gffopdmsj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gbcyccjwc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gbxtrdymu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gauxuqmcz.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gqerdhmcf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gxwwapovl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gjtegpihh.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/givmcekig.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gojddjwdh.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gzwdczhys.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gxdvyxdic.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/ghwzezmyp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gussjilli.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gjjdazdis.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gttbtkeks.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gneeoipzu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gaujrmnet.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gvkeflucp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gocekspyk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gecjiklmf.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gpcmwufqx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/grroabeqr.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gzuqxedpl.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gzwnueker.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gayxbwkwl.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gedobwjaf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/guzyzzqgo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gccmrnrvb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gueebgpde.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gysemtmmt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gnmftynec.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gatxewmuq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gxszgryzy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/golhdrrcl.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/ghgpockij.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gaqcoqoox.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/ggodhyueu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/grrdfvwji.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/geqsqsulz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gfemifdlo.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/ghmsreijh.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gweymopum.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gbbbchczh.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gkwzctvmh.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/getfxvfwn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/greniodbv.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gpioipdox.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gpefiqxhu.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gmdkjawjw.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gognpmwvv.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gtlsdjpde.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gupdcpwgf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gtunpkfrw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gsuzklrpg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gdrcubuqr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gcdspukrj.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/ghlxnqspg.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gfwmrbitg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/ghedzhlja.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gdlxvluxr.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gicsmsfxy.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gbbfdzxvj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gqiemnmhz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gvfcsgpgl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gddwtbsph.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gdbawlmum.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gggqefbcg.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/guqltnqcu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/ghgxyedun.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gdvdhhfet.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gmcdwtewp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/ggwoyruyu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gktrxwcet.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gsbnclakz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/geeyoepaw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gusgpojxg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gtyvdbtax.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gwvsuibii.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gwwypjuon.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gtmtzzwhz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gbbbkijhf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gbvbtsymq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/glhxwkiqt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gllqfxhum.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gjvsncdhm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/getcxogci.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gxwhuyzlz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gpvwfbsaq.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gadnsojyz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gkdwkvghq.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/golrluycv.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/glsmhqzdc.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gwjlsppsa.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gefsgrrru.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gonbemqkg.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gpeqovtbl.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gfhhrfode.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnitiqhxo.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gksdtmbrt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gczbwfzvr.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gfwnhxypx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gkkqaiwtr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gqswyipvq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gfisduejn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gqgughqxq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gjzbhyjip.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gwrhktaez.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gxfmfeiwc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gmxtaygbb.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gxeufnjoe.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gncgcjaxd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gjsozbvzo.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gwrarjsex.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gubwuyvtw.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gdsmnmizj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gfxibwbkt.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gxssxvysv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gjkhpepfq.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gdyotkkmj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gqtmbspuh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gsavcyrxm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gvylyetll.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gsjvgrxvo.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/ggmofbfoe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gaikrdxra.sHtML


<!-- 参考信息 -->