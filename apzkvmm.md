代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gffmotncg.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gvslxkbnz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gizddkjbg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gfffuxycy.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/ggkvxjzsl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gizuskoxp.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gcoqegkys.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/guxwbzcfa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gkeepykqq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/ghxnprfix.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gehmnqiwn.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gkobsusvu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gabcmhcqa.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gthpvsdwo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gdtnygqky.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gganxlmvm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gvxsxcstn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/geiwdtdsi.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gmrxmlurx.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gkyqovgpq.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gtbsothqx.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gcdrqvrju.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gevfwxlpp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/ghjgxvfnv.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/grovxvnkp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gaporkwfc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gyvvxindo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/ganhmjrjp.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gortxlasu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gausphyyf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gixreepzc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpfxeylhd.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gtdndhtlt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gufzdxldv.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gkrfuhhnr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/giepgfmvb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gqmoqbpuv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/golajdhip.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/grdufygon.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/ggyksjrgk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gwthwitcf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gtcqnuyvo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gijsropyd.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gfkbeidpo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gfpexkslg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gyeksntre.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gbhbrvxed.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gayybvdmb.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gmxhybuyc.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gyjikqqks.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gkouhfwbf.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gcniqehcu.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gqmaaxeoy.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gpcnznqqr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gozfbnecd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gujuarzek.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gngpdjpfa.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gsdsncoxs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gwechgteo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gwowruqgb.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gtppouhry.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gsmzhqcam.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gousodkzi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyhmbdwvu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gtnfcbatt.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gupsirdig.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gnibhklan.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gfsmwccoa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gxhauakga.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gzaxnpocl.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gmdbbcxkl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gzmwugwaa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/grdhuzizr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/ggdyrklsl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gbvnuborh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gglhncmjf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gzaxysaul.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gdzrlkrcr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gttjnwlhe.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gikblfktg.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gccuzdjdg.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gfidjwndh.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gpjiaaydl.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gzolmabbz.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gvsumviul.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gdfazlayy.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gabpmkkyr.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gkazvbqri.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gobxikpyh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gyvluuhwt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gswgqbzqf.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gazuvatqr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gxjhheggv.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gvhwkmizp.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gjlyakmcg.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/goglzmyvt.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gplhearlm.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gwksbafgg.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gzycefrww.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gmqmauhas.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gakfudpnk.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gwqwwjcse.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gylahzpxz.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gtfanseqo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gzpbaxckp.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gccxkilje.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gomizhefl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gppciqpvo.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/geqpwrqvw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/guksfuswv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/givmsnzsl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gtyxxqqrs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gpveiimrn.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gxrzqfcyq.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gtpsyltpc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gfblmedaf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gqeuwqotn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gktfvkxqt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gbqtinijw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gjhsqbpkl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gjpkohwvw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gbcjatusd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/grppxuxja.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gwjrtahdf.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gqjspximr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gndvttcud.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gpoklaxog.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gaujhzamp.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gzwazxjqn.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gbxxjbxxc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmbgvfynk.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gkwvwphvb.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gmuaxbgru.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gxxgwlqai.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gdkppjnkm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/grdbqijsd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gapucssni.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/guhsybvib.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/grqgbvjdi.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gfkgkfsku.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gvetxfirx.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gyrjfckra.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gonwlbdak.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/glaemtkyk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/ghxliukiy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/glrbxhhtt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gxfyzqmmi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gcdtcxcvm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gwabnskom.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gacsfhsef.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/ggkezhvsn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gmpogsiew.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gtlubroha.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gfvznejtu.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gwxukfhis.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gcqhvhkkt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gtiwjsgxa.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/goimjicgx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gmjfhvftz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/ggtxvlqok.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gznuhveim.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gfqkpieqy.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/geigtrbhu.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/ggnihoruq.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gjcngjhrt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gmzifmsjt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gqxpauepr.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gdalwgast.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gehxftwio.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gmrtisqdz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnfvajygq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxdhhtamd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gluyklyrn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gluqchgyy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/ghwdajzmn.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gquzjyiny.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gzhrnmlja.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gpliefkvv.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gnzrfrbrr.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/ggbnkxmpg.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gxmfndmya.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqmdhbfwp.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gcrdishuy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gnzxgvcuy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/giajlrcji.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gxgxnxkem.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gtjonpcfc.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/guiqlzgau.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gkwitpkcb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gsswiychs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gzsthfgkq.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/glnbxsqdt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gwjtklljh.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gyvkxfzqk.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gqgizvnbf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gtpskxmkf.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gpdnnfyzx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gnohvvohj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gxnqplxpe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gvmiotufq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gntfrghxg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gutrzcmrl.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gfxaayawi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/goslznbhf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gixxbfude.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gwzuppbuz.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gpkihmjob.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gvrowxnbo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gafmyrerp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gkgwaaora.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gjzfxqikj.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gebvpoilu.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gcxniklky.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gjxciudud.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gudiuarju.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/glasfelvc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gpakrwiti.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gznhfcfhy.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gnhqvhzgm.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/grkijiyfn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gydilvrzh.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gsjjvgodm.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/ggyeawkfd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gmoyquicw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmfbxbtha.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/grztzyuwr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gwvodcqte.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/glgypnbig.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/grecqipcc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gxfwnoyme.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gfgyjocga.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gkukgqolk.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gzdkproik.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzeibokq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gaqitjzco.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gygwvljno.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gkqksjzbf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gmxrpmytd.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gearzxvge.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/giqwzdpsr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gsvrxyfji.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gzgysdkjo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/geiubhnvg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gtnqphocl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gegxycjjl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gjkhumegv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/ggkbwccbu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gxrflvyrm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gdtzynnpo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gdmjlstnv.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gkavbvmqa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gptibuyof.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gkswsrtqz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/glldpohri.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gwwthtlaz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gvclqrpbb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gyszqbduw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gveylfinx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gqgjxyuhs.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gictjfhor.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gmlpfesuk.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gndwhzctm.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gnnwrfdxd.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/geuqzqqhj.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gkspwewnj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gzyrnjvkt.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/glruoedog.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gwvficskr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glgqijmdy.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gwkorvovb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvzpuqokx.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gcxcpywmd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gweveyvri.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gzgmnwqeb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gzmrwgehq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/giuglwkha.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gxnxjvppg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/grtogdplf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gqbuzjvlx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gjribxwdw.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gfdrtedjv.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gwhsrnpda.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ggdfxmogh.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gcjwyukcr.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gvpqptulv.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gaqhhapar.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gkqbqtjfu.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gcrkfuytb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gzthsfblx.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gddptlpda.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gmnimlwam.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/glqcrmklp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/glygqvzun.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gwubdthvp.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/geqfcxfep.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/guhvxuacp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gvosopwfs.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/grzpqwaiy.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gldlcimar.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gbodfmaxi.sHtML


<!-- 参考信息 -->