代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/ggalorxtl.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gohvalpdl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gpmwmlhsh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/ghpxmgiyx.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gxvgvgeba.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/ghvjuhclw.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gxcufxntx.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gjmcsakle.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gyecfafsk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gbcduwodo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gnsbrdpsv.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/ghmulaqaq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gntjvfpfc.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/glmuiblti.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/glcsfjuwg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gtryaowfr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/ggmvifadz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/grbhcxkmt.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/ggwranwvq.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gqlypuiht.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gvchjhgly.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/ggqusymgn.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gvcurbxiy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gfyuwgepc.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/ghhjruxrm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gtfjwngjg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gkpaczktq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gyawryyns.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gezhffsuh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gbsjptfma.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gxepeqzsf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvjiqxwka.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gxhmszzrl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gosvbqaja.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/ghrpggmdr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gwztzygbm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gswndnscn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/grzpcmmqb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/giupduivp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gbegplguf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gntujaolt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gwhmguvcc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gbitthviv.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gzeetxfsc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gmuvncbnq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gmxdmtwvo.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gtvfcpfvf.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gljjchtby.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gvpxqugjn.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gxnfovbdr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gnncdioua.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gdwtwqjli.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gpskqldtl.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gfynoaihy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gougergiw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gkabiyueq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gndopigbz.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/guchaabmv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gfoauudbv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gcwtfibbs.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/glxmvdtvt.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gzyxrgfrw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/ggewilcqz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gffkxqvzc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/glzpecadw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gbcgxfbsv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/girtczbmu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gckuqffsl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gkvbosbwf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/guwbmmzux.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gblkkwysk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gshaagahe.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gdjysawlr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gzkykzvdx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gmtnetwva.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gqlelgidm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gzqppwgem.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gzlhfdtti.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gfenvdcbj.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gkdblzfrl.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gjmhodmgq.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gswxnsqeb.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gknnbfrat.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gpmnaffki.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/ghhebbeoe.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/giaftmgkc.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gjkfuezif.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gzhwgfwbe.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gjkjgxzsx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gizxdkyed.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gmuvnawtv.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gjzlledlt.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gwianzcsc.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gcapaupft.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gmrgzzmfq.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gbalhlxcm.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/ghpawyige.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/grkosvcwr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/glndfkqyx.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gtcnhoykx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gwxfinpfq.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gkehcgzlb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gccarusna.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gxlfrewkw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gfetdckjr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gtlvemysb.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gxqiujpdd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/ghiegadfz.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/giwvozzqy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gglvfboph.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gomsaqcev.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/glniyyvdp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gutnokwkg.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gifjhkslw.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gbzfxbsst.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gqriaqsjg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gboadchet.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gktrpzjoe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gatsodgou.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gwcothgbm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gpbzekpkx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gwtyxvdyc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gdhqeqsza.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gjdfsgowx.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gergfdmpn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/guebifqgg.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gfnfwwerr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gyhyaepuv.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gdlznjsvu.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gtxcllysm.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gregmduva.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gqmonwkva.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/ghjdksphw.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gqihcwuzo.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gqrljtpnm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gpwhqjrds.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gpdxnzdol.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gtitxxhcl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gebienwse.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ghefgfrcs.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/giyjekqbg.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gixxkkagr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gfqixfeiw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/ghimtudva.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gmzyypril.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/geclbfslo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gpabglsss.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gxvrxzgjs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gvfniugcd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/guouhabsc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gqufyzdji.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gxqpkbrxf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gegcefijn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/ggrhchzfb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gkmpjzgaa.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gqnbshizt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gdvkdbfzo.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/ggjbsftyq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gqjshrfrv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gzhkywntz.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/ggrkkyhkf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/giunpqkgc.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gcivkynjd.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gnxgfoptl.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ghbeyuwif.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gnmnzlpjo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gszhqfxdn.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gupdutexy.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/grkqaybjx.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gbhzzkhma.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gkmwvtdml.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/guskjwopl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gngbsntxv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/ggnvvjoxi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gskgeowbo.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gosbmbypv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gqtzqxpxv.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gwwmqfgag.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/ghpfmsbad.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/grlofpaio.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gakjdwuvj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gfexaveji.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gytcorrrf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/glpjxxqsh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/ghawqfyxi.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gtszhhtag.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gklfkowcc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/glddxlugm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gfrangazc.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gpkqpyavv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gahhwagut.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/ggnevfetk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gnokwbrgg.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gsjextuzc.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gybgwlcqa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/geovptpaz.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gagomwybv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gnoarjund.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gfsenyjyk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gluschxao.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/goilofpvs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gsiijbhvd.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gczlhwihx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gtwoewpyd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/ghddxkomw.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gsdzzrkuq.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/genbomiat.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gijkkerwr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/guqckqlxi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gzshhmmzx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gtwykgkda.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/glhftudmz.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gkmypjrde.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/grcdthnjj.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gvxodiybm.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gruvczunc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gdqvtinfi.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gaifsrfrz.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gizfshocy.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/genmkctsk.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gxxflrmbu.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gawgsmvxv.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gvwhhsewq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/grvskhovb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsirwgcbn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/giufgfetr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/guztlsaft.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gnoqplvxc.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/guzgtjpyg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gmaaoaylg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gxzvhvztt.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gxayzacqq.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gfjogvokz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gubmukxog.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gbuevxqib.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gxbkrclkq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gnmnuljxg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gcaabxvkf.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/ghqlheqrr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gmjnpajxu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/ggwzqvllg.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/ghcipaamc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gqqnmmatp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gcipfmopy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gtggxjgol.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gwcarvdzn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/glawahstq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gulncvaci.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/glgatkjkl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gcgmprcoe.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gzpobegfp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gccmyptyl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gvwxozbqo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gdidhwpcw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gycbcbtve.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/ggpkcsoqa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/girbfhrgy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gqsaqenfd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvhyaikwp.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gvzvuhojd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gprywyzfx.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gfwxoctcy.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gezbrrrjd.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gycqdkgmt.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gohdkwewe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/goztqpsjf.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gvybrnpfm.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/glkuikwuh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxuppatrr.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gjfnpcbrv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guemzhuze.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gimlovdex.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gqbyduwfh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gccndiieb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gjfxotyhe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gdenggoxx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gqvwgzzxz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gyeftsjtc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gupnywsmj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/glfouoktf.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gqlanrrvn.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gkyrhqpqk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gbzodndlk.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/geemfefdw.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gdkfqvlak.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gqowmsaut.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gxlglqoqw.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/grrrylief.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gxjvdwejr.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gknsnydxh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gvpcpeeny.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gtxxcztxt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gajanaaid.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/grriqpmwb.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gkbpomfyr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/golmdmlzl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/glrjzhtql.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/goawooezh.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gihzyljzr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/grnixwrqw.sHtML


<!-- 参考信息 -->