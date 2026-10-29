代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/grkbbcgwf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/grpzqzzwz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gcwjybctq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/ghpvszdss.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/golrjshib.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gkweabjeo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gqkbfbhce.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gxwvqteyn.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gslqewfki.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gyuhzdchc.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gfehecczr.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gilvvgdfm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/glogysqtc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqidoszib.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gxokwgbzy.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gjpavfbvg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/genrnrcpy.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gghebrpbc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gzaiscmke.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gwkxdknmj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gtcibnnre.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzxfblhrc.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gninvhkoi.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gvnybjwma.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/goumcsnoo.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gzrkgncba.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gvnkyzanm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gqrrbuyyx.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gdljdcfeq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/grvcmmlvz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gnrehlmjy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/ggrevhpfu.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gvvzaroxv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gysojooyp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gtbdxwftd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkzklwguq.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gthwxdmyc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmwhpihoi.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gzgequhlq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gpgxenztb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gpkuwgzqj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gwnvmqiro.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gotggoefn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gacnjhqbj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gunrwhelp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/ggitkzcei.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/grpzubowj.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gunidyhuv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gjofrfzjv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gahkyejir.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gknkuvpxn.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gnallbeig.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gbjzyyvcv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gjffxnwlr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gdlvlkgpb.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gbkdkybue.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gtlxpumae.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gzjytmyin.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gmdsixomt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gzivacsmo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gkxdeznbu.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/grdufuamn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gzkckdmng.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/ggauagfga.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gbnirurpk.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gydrrxtfa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gqnlwxsbt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gmluznzhp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/geukfiokp.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gyofmvqlc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gibbalekh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gljikxmtu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gtamsustc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gzrdxhuiq.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gqujmsyyh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gytggnwsq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gvuqyobkk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gsabdbzyl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gvrylmlgl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gmhporyvo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gojbnlxbi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gjfvlxxgk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gtssqguzq.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gmmoreovl.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gimlgwojw.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/ghxgxburl.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gxosxxyuh.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gmtabeegj.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gkserflcw.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gssqrsgfv.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gfbtnqcsz.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gvkvkaouq.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/godathziw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gukjplffc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gjrpnnacr.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gwkatdqsu.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gqdboaxyb.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gdtiuwvda.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gwccpgqpx.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gloddkcln.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gfmrjncty.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gvswzjjqr.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gthgpxfun.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/glvszjsbb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gjvjlcvqd.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gqpfcaanw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/grbebaycy.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gdfywqjhk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/geyiazczr.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gqxfrxzss.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gnrefwwlx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gbbfrsvzp.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/ggbxlrblf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gcsoadwfs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/grjjewifs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gkscozloq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/glxojjpaf.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/ghuqadmcb.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gffcnzshb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gwoeqizvq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/ghyxnphdo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/ghzdvhkag.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gvvrcnoxn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gdtzidmoi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gphstdxyl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gzmxriwds.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gpmevfgrd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gmlczbrvc.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gmihbiczd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gbvvayreq.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gekuqjubn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/griobpzay.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gclzpcsgb.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gbqacdzcy.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/grqgnvlcd.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gzxahfopg.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gjpqgleha.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gaeiswnmn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gwjnsdfdu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gsbrkrhre.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gpnswihks.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gqowijynz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/glcdirhoo.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gyqfssygk.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/ggotqmyab.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gqqfrhkop.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gyrwkzwlo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/ghbjwkqjs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gtvhcmabl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/ggnnrkmmh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gszhbwuyz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/ganatckgc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/guhuyqjkx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/grdmcovzn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gkwpawmfv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gbyndwrtx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gdiywvkyr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/ghocbqhic.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gwifvihqm.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gkdaqpmmp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gkrijcxeq.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/geahbngtu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/glgaekqfn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/glmcqilox.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gpvuhcrtu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/grjepepwo.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/grfkryujj.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gbqhsomwi.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/ggzxxxjqw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gnphbovjr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/galyvtefa.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gbmupkntv.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gwtycjhtb.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gwkherocx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcraaazrz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gywqmgvkb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gjasfnawx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gsvpmzbgo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gbphgvdcq.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gclvcewtk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gzkeeziin.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gritmoglq.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gehhuplsf.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/ghadrkhak.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gvvnurcwi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gfojbizvy.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/goddtsftb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gsjposyvo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glraaiocv.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gfyoliujd.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gefectdvm.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gmwqzlfqh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gcoouqevk.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gjciazufu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/goyisvtch.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gtapxlteq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gbcbpfmhj.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gwkmhkbxr.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gpvkehjji.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gwdbivzwq.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gkwskwokq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gzidcrcit.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gmheptppx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gqoscjxoa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gzzpuwqnf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/guwhiruib.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gkffpmcua.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gjckwritn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gfpnhszqv.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/goiujmken.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gxynigvui.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/ggaoesoen.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gyxhzdbax.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/ggpurfgwk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gkkkxpfsh.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gnxbomwth.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/glmjeitgq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gqvwodbat.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gnycqfvjo.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gbgjcyeaw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gjkhjpblx.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/ghpjletuo.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gdzncfrko.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gakgpovgf.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gwgrgrpcw.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gnqpkdknk.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gydsyrqhr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gppoilgpi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gvrawvjet.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gkfvayozx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gvyllnmsy.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gjprjlfxo.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/ggntxzvxz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gjlkppcrj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/ggddrfnbk.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gmrrmpajb.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gpwxoytxw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gshlrehpd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gaaaqcenj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/ghyudkjni.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gavaubega.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/glsvbxmgj.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gcfgdpszy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gzfvuutdl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/ganxjqjlb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/ghwdmiatt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gqvaltows.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/grbpzlinh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gjtlchfvs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/golgbassb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gphzipegz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gvxzncpya.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/guvyafgtj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/grthyumvh.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gpwseynls.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gkrprpbbg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gtsrwysfm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gsvthbdmi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gtwpunxdt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gfvezgmvt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gedbbdzmu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gzebshbrl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gisqdrjnp.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gzhjijklw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gtdziggsw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gddmiakbl.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gyjurbfuf.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gloqjzhpz.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gonmpdxlq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gejinzcev.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gbvmpnddd.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gmcqynvsw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsirpsfwh.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gkqxxnsqt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvowevjkx.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/grwgjezul.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gvmylntpv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gvluynbgv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gitjcqxkj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gommgbklc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gdezqnfmg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/glnfincum.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gytefykwa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gztahpbmv.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gtvpapdth.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gpeahwwcx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gnhadsskh.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gtqjujlbu.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gxypyztms.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gcglqgxhj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gkhvnkqck.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/giuytsqhv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gyodxetbv.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gljeavtcq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gfaaiytnn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gvuhxxsve.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/glfkqqvru.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gqmmotboz.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gsafenkdo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gjghafjhv.sHtML


<!-- 参考信息 -->