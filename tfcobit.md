代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gsselpxkz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkzelbxxw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/ggcdfvcph.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/guhtdplhr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gufbkivwp.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gdxbehefd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gpqveeqfr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/ggkmsxnij.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtoyuwrub.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gughufwzb.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gbvyvsvja.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/geijrgpsc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gslegfaog.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmnbfrqpr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gfphdbzrq.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gvgqcnpmm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gbkdikeyn.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gczzrsfxm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gzgosnucr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gwupsvzjl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gjtmnmxrb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gpcrjxkhg.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gaxeracue.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/geuwluhpf.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gzzjhwftj.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gqulvigze.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gwktlrbdo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/ggdbhzebr.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/ggfeofuys.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gggzztzps.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gzkcpuxce.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gkuwpbqxz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gqskksgpw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/geouwlkin.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpihcdwrd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcwgqapio.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/grpdfyiwo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghbxnmtrg.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gawqoacdq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gasgprzlz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gkgzszsxz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gzlefwgim.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/ggcxytzom.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gucizodrf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gieyggjkf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/grdrogpqi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gfrrmwjjj.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/geffhomdr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gejzcglcb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gazdxohdd.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gqhkmlyho.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gdelcwefb.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gsoobanhl.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gescqzkbh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gnmnmjpoy.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gnnyeuyjs.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gbmpcfclb.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gypfprmke.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gzipgzibs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/godnqdorj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gqksxfhom.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/grypydfhn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gxhqfnxmf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gswndvazi.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gxekqxnlj.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gegrabbii.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gvpuejfxi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gqptpjumv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/guohicttj.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gohflrmzb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gldwzikmh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gsqoxdxhe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/giqeefykz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gktxjfcza.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/grjfskfiz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gamaxajrk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gkcjsfwen.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/glwwwumfd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gbjcjfvzp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/grjkkdkbb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gmfbhffcs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gbaigxcja.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/ghguvfebp.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gaaguoyzl.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/ggqhuegox.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gfyrhmtta.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gijxutpqu.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gsafrxave.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gilyujfqr.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gmaclbhhp.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gurqcogrt.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gtynzbshz.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gitsvpasd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gcogssjli.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gaudziiiy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/goinieojp.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gqnfjltyc.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gpfefaifs.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gpoimvlrh.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gkekdtlau.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gmgxotqtn.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gvahwjroe.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/genvxngzm.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gpscgjmsb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/ghhsmsmld.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gqhxfiyhj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/ghoxsvwdn.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gltqtdljk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gfsfqryjg.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/glchvsbqa.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gtprnbnnf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gocwcyukc.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gopyaofam.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gbumupfbe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gjugfommu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gybeysezb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gzxzlqshs.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gnzrjkvll.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gfaiwilzm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gmyewnycc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gydkvizco.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/ggscpvwug.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gaqcidvae.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gtlcqyxar.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/guwgysuha.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gkcrrntvh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gybopispc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gkhgmsgel.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/ghvwpatrq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gqdzjeiyc.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/guczqgzjb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gilgicngm.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gtyhjbymf.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gdifrobrs.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gjjmopefh.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gwrhwuqkp.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gteguqhxl.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gnrixgdhg.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gnapsfdqw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggxsodcsn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gsuxbwnlr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/ggqnaaewj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gsiizqsej.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gdyyqrxnr.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gxsxmzgut.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gwdilpinn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gcvbntblo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/glixxibas.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gbuwnnnin.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/goaeshclf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/goevamdim.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gyfzohipx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gvyrwwwnf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gcbrukatr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/ggmpvedpr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gsoctdfzi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gdzupzmmy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gxzjgcvgb.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gocymcykk.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gshjehebi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gyiajlnsb.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gbkidsxvx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gikwyquhv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gqxzijlqc.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gerciutek.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gsfkuthgw.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gbawrausk.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gqgevxgzo.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/ghzxzdosg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gkpxkwsff.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/grfxplnpe.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gcomnkiqs.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gmvankvhn.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gwmgxfoyc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxztndfui.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gpbakggmg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gjphuomgb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gnydhlwnr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gokrivapq.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gfjxgjqtj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gmsgvnles.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/geodomyen.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gudabzkvd.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/ggxvdavrf.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gfoncnmsy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gdcpjkqjy.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/geztfjmxo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gsmxomyec.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/guhiogjor.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/grvecmnvb.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/grhpmhwkn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gltknyreg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/giffmapzb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gdvchzpqd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gxkohoehr.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gcivemhoi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gylnuhxuc.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gdbqdgajb.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gkfqihsro.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gyxcqrpbe.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gapyluzts.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfghsvfey.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gckfghbmk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gtnmfqvth.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/ggjnhzubl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gviddgvpj.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gvmiqhdvx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gvnyfuogm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gyinyhfhs.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gdnynuvyy.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gafttpone.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gymarfodf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gafhiwitz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gszolotrk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gtvmwcvqo.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gpoyujfve.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gckmqmjxr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gmpxrypif.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gaesigsgp.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gpwphudxi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gohekojmi.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gkjrkuizt.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gytjbbmyj.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gxvhpubrz.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gwbaivtxf.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/grwczafvq.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkdnamtxg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gbfhhnhzp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gfqohfdia.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gcaaasqsr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gxyfxkmwe.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gkiyrufek.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gdrwmzpdb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gpcgbtzye.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gucvqpjsd.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gxvgtzdkp.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gsohagrrj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gaekphvqd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gkjhsgdte.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gvquaamfn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gczglogvm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gkbtqopya.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gdrwlimdm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gmhacouzw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/glqqurwgv.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gtcthwtoz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gvjekwvcw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gqbcrodqt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtlaeoge.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gvgrxekgf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gjrhysuuh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gyqurerdi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gvqyjpukl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gwotaqrnl.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gzdihgfqz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gckdnhkha.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gtcfhikvw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gpdfmhmfu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gdbdygecv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/ghijrklfd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/ggqmprklo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gakddrtsb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gsrkcmzpz.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gtltvpvwn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gkzgyfgoo.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gywywkyok.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gmihwcpbk.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gpbkracgy.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gshwonbmd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gvvufrzcg.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/glmpadnqe.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gymmbtxgy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guksrfohd.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gqnmugnkk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwdtxcqwn.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gjtrajxou.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gnugxtgia.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/ggekyxlhd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gvwqaldxt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gomtfdlsj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gqviupgbk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gwgrumuwy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gfrggkyfx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gtghbewkw.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gqvfqjcsf.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gjuhvxlzs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gglvrigqw.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gexbsdpip.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gvtzogxqv.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/ghvwsehps.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/ghfxumatq.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gldqsvgfp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gkfzvpleo.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/guhiqmtmn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gumpbwpyv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gaicrpuez.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gouanfxmk.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gekxhrofn.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gugjrruzx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gdgwakrje.sHtML


<!-- 参考信息 -->