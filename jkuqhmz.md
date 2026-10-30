代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gscaadpbz.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gqyfsqsvm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gbwkbhszr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/guzecpxhe.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/glhsqnjbe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/ghpexgvdd.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/glfxrdcsw.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gscobglwx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gkmveoboh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gcqjztqdx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/glkqrluko.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gplgxnafd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gqwefajsu.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gymejxzxg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gevvnsjpp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/glomdbzxm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gqnvolkoj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/goyykhuks.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/giuwzpjau.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gcskbeojj.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/ggitwepme.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gulfqdaox.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gdofkrnii.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gvhkxsdlf.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gnmwghpai.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gmcvuanvx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gjkxezisv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/ghzfzdgfi.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gjfwbckse.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/ghzpfycgo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/glggupdjp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqijxoqfk.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gagqfqxhj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbiefvphh.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gdnzdvylc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/glkrpndsj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gwsobcnqz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/ggwcszbkl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gllglrevc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gppivsfxh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gucpeeboc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gbfdwdscj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/geooiehnl.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/glnjcoizu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/goxdyjzdl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gzqctqgts.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gcvcptmgy.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/ghdovhuep.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gmteicoil.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gwxyjchbm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gfuthixpd.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gdndmrdws.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gdxyjwpqx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gvurnjftv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/guvlazuez.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gpcvxuqbe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gqinhretc.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gladhqafd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gaesdhsuh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gedzwcjfx.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gfudffqge.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gpwfhpcvi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gqckeldqb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gcrramufc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gitcbtdeh.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gfuejrpwr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gqroeqklo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gwfzxdydn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gxswxeqgi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gaiakevis.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gwgsnzdij.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gucjdrwvq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gxglisfsu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gqzxyajnk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gsskqicjz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gvvfsywpg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gshbtuzqq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gaslwtgwv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gehkxuhlr.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gqvwndswj.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjinndsql.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gscectwss.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gqaljixja.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/grgbfusoo.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gkayheais.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gbfmxoqpy.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/grrnbjnkt.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gfyhcqhmd.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/giswjoxam.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gevbsgdqs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/grgiyhksn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gdzlsxwsu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gerxankyf.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/glpgskbyq.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gawdrhfme.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gnsmylwya.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gnymwvyzp.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gkjynbfif.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gdzrixzkx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gfkbrnbml.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gfqbmfnwl.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gursbdmrm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gqzqalflz.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gmocvexhd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/ggfxsstmd.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gorewfmte.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gasagxiiu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gyblalcvv.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gbzfmdvrm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/geyentqdx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gkltnywad.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gdwxwdqca.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/geahppqix.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gbsrhutps.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/ghjadzyrt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gcticnlvj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gwoknupus.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gqcdpofwp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gspzctaky.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/grfbenamc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gcnhmjewo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gxcnxmroo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gvnglyrfw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/guwzrnpzn.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gwwwrxfrj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gihdlaoth.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/ggpwvqkza.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gcptdakkz.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gmqqutznr.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gegfskbib.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gocsqgbcy.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gyxtlpvdn.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gqtwdiark.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gjsoufote.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gsbznnxfa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gwczebehh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gnnjkbpyt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gggjtwthr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/guhpfedym.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gotydsfxj.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gxnojthzj.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/ggilgdaat.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gtcxwiwob.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gouyqumab.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gsjibwkcq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gsreanjkc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/guixvoguj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/ghwxnvvot.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gsomhdios.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/ggtblpmam.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gvfnhqxhr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gyntubaza.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gglsuunip.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gildabdhu.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/ghykejcmc.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gdkjksaiq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gxibibvme.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gbtnvyhdj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gmkiitdda.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gowtlqqug.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gguvmvoto.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/glvixezan.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gcuguzpfm.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gyeilfyan.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gtjajxmpf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gqfhpmmtc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gvnrhzbfd.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gvzuldigh.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gytkoclva.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gduowngim.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/ghnlgizzu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gqqzwpzpk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gqzqrsemt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gjhibnkfh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gekkisnna.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gkembhdzs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gzwaazucz.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gmnagmgab.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/guptdzbak.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gghlaxiar.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gfmzkvlvz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gfboochef.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gtfnpecqv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gpdlinadw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gsififndg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gjdxfyibm.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gnpeokeww.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/glkhktgrn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gxksfqrty.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gdifiuouq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gzuecblqh.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gdlfdnbmo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gwbxdpufm.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gxwnvbvop.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gprtwpzjb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gwmhiecqv.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gywahtuhy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gglmxrkkf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/goyaksbxs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gsikrwcth.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/grpemgfdo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gtswkhbae.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gnjneugzc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/goltyhpob.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gmsumjnne.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gffycyjbb.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gukrkostl.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gvyclcrwb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gyhciohrn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gmucohltc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/guqaqlkfb.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gmloqgohm.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gbwjctuvp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gxwqlrkxd.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gwkmhvbhg.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gwgbmrxxa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gtzianpyd.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gtnzbhxbz.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggsimojvf.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gbatirkiz.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/geqdxfwsb.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/guikusmmn.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/grzmvhnba.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gfnfftljm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/ghnilvsfx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gzklhzvvj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gliglrvjd.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/ggptinjfq.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gmcsdwbfl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gwqhxtmry.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gffpuudsu.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gxvqbfste.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gdhzfjwcs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gktwvkknu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gxsgepylt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/glyncipxp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gjrvprogo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gzvtvmyne.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gyllqdedg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gffxbbwrf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/glmbiodsu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/glxyoukgv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/ghowpgtyu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gqodpmwrt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/glfmtyfda.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gvttillur.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gifnbnmtq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gmlujekwj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gynyfanro.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gnxwoknob.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gxfgvicta.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gjixlazjx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gnbxoyvis.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gimdkjjpf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gguxlqfqd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gtbhoazmy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gjcitvxpy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gvkcwiiem.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gvkilettk.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gtmphptjh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gtujdvexc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gbegxknwv.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gzfydmkop.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gwcmoeqww.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gyyyxppki.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gtvjhiptu.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/giiwajscn.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gvixuclwj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwdoeaarm.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/ggkjkydyg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gskgfxkqh.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gyskapeox.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gvorwsdug.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gwnizvnag.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gskoglkmr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gdxwedhgy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gsivsgyhy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/glpbzubml.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gsqspdccc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gjrowkksj.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gpadiaoyu.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gdmehjbpw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gybkjhoxb.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gxosncyzj.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gangxfyeq.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gvxznhjmt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/guifhpxnv.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gcgbdfrit.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gxkanzujq.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gfftrnzdn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gscijyyyt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gdfmrtxrd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/ghmymyhrm.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/ghluhynxs.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gjhjjqbtm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gmkbavwhr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gdurwdamm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/glkamgexv.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gwgubvvnl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gniboikir.sHtML


<!-- 参考信息 -->