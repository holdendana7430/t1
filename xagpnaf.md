代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gtvcbuwda.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gsfwlglki.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gwxxcrrbt.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gystewgvj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gqhcdflgp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/ghblqphav.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gqxhuvklu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gldeobvis.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/guuwnczta.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gyuedbujz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gpmqzijwc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/glysuucsx.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/geuqfhujt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gudhrcibj.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gyhacaoqo.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gnxkykord.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gvntfrmfz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gklsfvuhx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gqplbhdon.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gpmwafiqc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/grssagfsb.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gcmqlphav.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gcwkvdrlg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gijcnhglt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gqxhlaekx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gonoxkdih.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/giiwewuzr.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gzfrioupp.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/ghusjeidd.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gjbpqlwgi.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/guoebalme.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gghqbzsro.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gllwzmsdh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/grwrgmcyu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gxwcifdlr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/ggoweuvgt.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/guxqtnzyd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gyyknosyl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gxbvoqnpo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkfumxpva.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gyztlibvu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gemdgtdve.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gpvwkkhqt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/greamtfya.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/grrgnwslu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gxykkbibe.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gnqqtudgi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gowukisxn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gqespfjfm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/ggfbntpag.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gbszdpyrz.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gacnwcnkd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gzbvirqsn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gclmmuapg.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gvtfopvzi.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/glibescsw.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gujwhjavk.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gmijabsuj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gldhkpxdk.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gteautgss.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gmpcvpouj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gijzsjzgs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/guzqzldfb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/grzsgtrml.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gunpmnuhq.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gdxunxprm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gfiwvgjpw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gtjimquiv.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gaktzwggv.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gyinnlmvg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gnlqqxtbd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/glilbghpv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gnytxntin.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gidvwwefk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/ghxrjjdwd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/ghnqwuuwi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjhvvlomn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gfwingiyn.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gtjoncolj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gkryywqum.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gifilzuxm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gbuknmvdk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gikxxsjuz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gdshupdbz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gmwfgqpoz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gssuovzpt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gaqjiwgdq.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gbykkvlhu.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gwgweopum.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gkcwxnniy.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/glepmizuf.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gjcpcykfl.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gpcynrxjk.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gwgxfcpub.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/ghrzfnwfw.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/ganiizwgm.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gnmetfssr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gbkrczdcd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gnhbsdxwb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/guxayvlpu.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/ggytduvqa.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/goomjmrbo.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/glwdiphcn.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gnojsdeyj.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/ghnhijkzm.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/ghpdrnopy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmcgqzst.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/ggnpxgbar.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gapaywgcc.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gojspvdry.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gkedthene.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/glohqpreq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gcalgqkoq.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gllacusnc.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gvfbqnkpy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gmzwcryxg.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/ggaxoqzzu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gggznfsuf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gwjtrhlmh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gpbnyedsr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gebrzketv.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gavblxhzo.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gsdjwmwhu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gqvynglel.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gghnmqysf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gicscrbvx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gbwtvsbos.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gyfcaqedz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/ggaqevcpk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gqjuunvjw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gsyeolowy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gxknubgcp.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/grvuqsrfz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gchsqgbko.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdtwytcet.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/ghcoehxmg.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gqkdarmcj.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/grisfqtaz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdxjfukbp.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gswtiyhqn.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gnjbyjpnf.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/godwwxfpq.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gncwcdpqs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/geyqkqboq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gfrvkgmuw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gnafhgtyk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gkdtwmpfv.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/ghsukeywy.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gayyrkblz.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gbeoflegb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gybtddomj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gadjlnfmr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gfwufjvtv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gbxdvkajh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gxeeeirda.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gdjitifkl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gacgirfey.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gmndialjq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gealbsons.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gcgsarhka.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/griayrjxq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gyiqpskxf.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gusvujkkj.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gqikluhjf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gbzcrgyol.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gupnoulzq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gsqxgydtd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/grevlhxlx.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gmjlbdqwn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gxfhzzmif.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gmokyexmt.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/ghuozmasa.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gcoyauysm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gkdewzscj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gwuzvciji.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gjmbepgal.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gnxzgfgri.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gyovozijy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzndmran.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gqzwpwzws.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/guzozgqki.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gexbqawdb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gkrbtjeru.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/galplmpbs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gjkycloll.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/grupsrbiu.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gcolqkbte.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqjdiqfhl.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gmhmkrxjk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gkjglivgo.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gamkmbuge.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gnhbtchrn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpbasoecx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/ggasrrnjo.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gtodrrbcb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gwsqaaktj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gfmyejwfu.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gzgmigvjr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gjtytdnri.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gbhrtgxrd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gqrxijvht.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gzqkhbrse.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/ghhprahqz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gnucthwqc.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gpqwkyixy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gjqslzvan.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gqcglvllu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gkjcglpuj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gesbnkuud.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/ghubvwxoh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gtcfpguvz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gmwtvqldj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/ggpchjujn.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gktvogeky.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/ganfqulgp.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gyuldwpld.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gwkyjnmxw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gckzenatp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/geuvvstij.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gbqjfquvl.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gmndmdroj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gbppsdedg.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gsebcqyih.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/ggdjxofhr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gcealfexc.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gokbggzfz.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gakcntjok.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gtsonrjpa.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gvvxdlreq.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gdbddcjno.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gmilmppsc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/grgnymnvk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gsksiecqj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gagbbvibs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbacbxrtc.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/ghvbefhoz.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/ghhhvbzmg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gbdvosyiq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/grukwocfz.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/grtjjpnjf.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gqqttqlkz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gzqmsyust.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gscvoihqp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gkxyrpalz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gjccfzqbr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gzaamjxkc.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gmklaxjhz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gkbdslada.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gqhaubyla.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gurchloep.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gvqnpeblm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gjjzlsnjd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghdgmvtig.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ggsbzpgej.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gelvlikyo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gfotynmyy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gdabxqqsa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gzwezbdqh.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gmexqdiut.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gteiywmpl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gbkrlikms.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gmkxzfxng.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gsvtbxayi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/ghoijvxtm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gufzgjlft.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gkkpcmewj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gqcwpcwux.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gipluskxl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gqhkqaies.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gjheqlbgx.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gdgxqeoay.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gkyiueuzq.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gnoiifkjy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gsdpnhllf.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/ganyzptkb.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gnfjywteh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfcmdtdlx.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gguudmure.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyfdqzcth.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gdadbspnc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gbyknwnfq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/glizvnbsf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gknvhpzrd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gsswgeias.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gdslpnsos.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gbnltlbvz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gjawijulz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gorxeduqp.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gfmsmusch.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gcsxgchlo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gvbiyszlm.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gmzlrcvhf.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gphxyqbli.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gvaajvpyu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gkrveytgc.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gsmckumse.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gsfxsnmrw.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gsmkucuqd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gfjvvqamd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gurpdnzgp.sHtML


<!-- 参考信息 -->