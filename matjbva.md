代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gmvnmsnau.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gvrkbuzfw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gjqcqtwdu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gfprpazbh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gdggcnhoj.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/ggtfcojiq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gkrdynhgs.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gfftrnufx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gprdegqeu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gvakjrxeo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gqancsnff.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gcpaziflw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gfblvaghl.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gkwndtszr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/glsjviovq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gykayzyxk.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/geyaumlno.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gqdjuylta.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gdhzyrhas.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gjztpxpnx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gqussvypi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gvllggrvb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gdubyfooq.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/guwcdhdis.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gybgelsjn.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/grpvilhdq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gacpgskmg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/ggcmwvsox.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gpaijgasg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghywundar.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gdogmlohe.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/ghhjbnnvt.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gbplsxfcx.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gwakgljiq.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gdajhtvfs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gsnefzkdw.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gabbzppwu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gekkblrqr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gixparqze.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/ggmvhtiub.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gtloifgvn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/ghwpdpuhg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gtvyttnle.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggdwfaybo.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gtoruladi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkhiossld.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gjinfjyip.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gmljsphcl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gcjjesemv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gqacysfss.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gchvghqbn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gwkunmcbu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gzxejzsgm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gyagoltwg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gezovpqno.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/giyhndgag.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gwxeeupyb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gfegtpixb.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gvyeijtre.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gexcgwqfm.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ghbancghu.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gwsaxswyh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gljoxicxq.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/ggckrsozo.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gcymhzpiz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ggrlbyapb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gslwzjxzi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gpdkepxmg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gwbfwchbz.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gwpxyumxp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/ghbtaxosu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gbnpoxmfp.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gsyxfhqsx.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/ghdwhffld.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gvnesqger.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gntdtklln.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gnenaleai.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gwwbbzitk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gzvubzggs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/geppftnfs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gfykeeoas.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gharxjtnn.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gjzyicxrh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/graplgfxn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/ghqziyamq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gtwsufvec.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gtmaygfji.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gbcrmorbv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/ggyybumjw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gqmtmwrgq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gwqufolpe.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gzcalsava.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gkuersqfe.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gkolnfgeq.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gryqpibgt.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/ghtajkbos.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gfderqnie.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gsiokgosw.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/ghutnokya.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gahgisdju.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gunxsaour.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gdpqmfdpz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/goduwxrxn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gafrndrju.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gvqgidget.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gsxpeuxss.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gfjalfrse.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/grmiuznfg.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gjobsepeo.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gkkwvwzmc.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gzdtvnlrq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gzbwwqdyc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/grtylorat.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gnbcvcfbp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gybdukzjh.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gackhbnao.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gnbvuwgvi.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gcbhgtinf.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/grphjegnw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gzjovevrm.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gddsykmsr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/ggogugdyf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/giczmwwug.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gnadrtmxt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gcsdnppih.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/glmdqtzwk.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/godireedc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gekpzlgwq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gutrtgamp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gjwxbopjg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gxbuxsaid.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gskvqiacm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/grdqdcxql.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/grjtruclh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gkromsauu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/ghubcejzf.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/grtjwrkfc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gggtcowyk.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gajntldzj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gkmgwylmt.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gvjfecutq.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/ggqattlba.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gczqjoxkr.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gvbrrnqnu.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gunzuncur.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gcaynngur.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gwymajuok.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gtvetntmy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gwqpafsqj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/ggankdbdn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gffhaeyys.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gvjnfefnu.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gilctrllx.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gmasmlmru.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gwmirpiwg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gqmpgvhup.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gsqxkgcqu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gbdsfiruo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gswykbyuy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gekhdacjz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/ghvgtiekn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gpznorslm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/ghtupkjmu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gmebuisvu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gdraqpvtl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gaolbcuec.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gbslujqqk.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gsbtfihvi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gfblrqxxh.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gyxnkbfya.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gmztgqviw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gftrdvmbh.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gnhnbwqgy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gpcieyobs.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gxpeorgbn.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gaxacrgmv.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gduiqobkr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/guzzvpsqj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/glblazgqt.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gmvrrbyqk.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gbqkmbmem.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/ggopwcdmy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gaezyhjrm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gyatmkbbf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gettlfoif.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gysspdcqo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gusofbuho.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gldyipkyx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/guvraozwk.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gwbszipzh.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gbehdeiej.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmxxxkfp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/ggjvahpad.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gffxdubcx.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gvnioiinu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gdqnpjsjn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gltmzrvpi.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gcopzhiqo.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/goasamjlh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gpayejrps.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gpqmhnvec.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gumhkeoyn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gxpnijoll.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gqdducwvi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gxwedsavg.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gjxwhpqcn.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gbrcurxxr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gbhydfqbn.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gjnlxmfqk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gtoamuokk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gaofkvlhe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gzolruljk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gfoogvdns.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gcofjslwj.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gjpthaebq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/glfrutaub.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gwktsnhpd.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gdlvliasf.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gfdmrazdk.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gztsngxre.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/ggcqrfbpu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gophlxwtp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gsimgjsdz.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gbctufrmg.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/goysclpbs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gcnrftvms.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gmsnjjyyi.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gzgvnlkxl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gjhwazkin.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/ggydefpio.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gvasshyrn.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghiwckkns.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gupizmaqj.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gialvrapw.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gsoroakpe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gqcfdwjxs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gmmknaoch.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gvtwdhlbt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gbrnztnef.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gtdtnrcst.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/ggvsawlmp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gzoisoull.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gujdamtpf.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gripebreb.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/ggsisyqwg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gprrniwlo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gasomdbxg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/ghchxeidj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/guxbzobqi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gypxbtaph.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gmekzseie.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/grokxzlyk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gwngurpjk.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gpbazymfn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/grhixqafb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gowbxzguh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/grdthhqqk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gpscrcggq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gxtxjokjz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gdoqwlhij.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gapnkrvug.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gljmciphd.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/grwokulsq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gtlmfkmqm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gyjyklvhv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gtbonuzef.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gutifriyu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gtuitndkb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gcfvyanga.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/ghnigsgtl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gmbzjiuwv.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gfzqabirf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gowwlnwgm.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gnjchbsli.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gnfplenlp.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gazursfcy.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gcinfbpov.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gzxoorbpm.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gxflfgogb.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gsebghxrp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnskanwmw.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/ggijlwbzs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grrbdrbpu.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gclgxrkub.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gyesrrxmi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gvjaskisy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gjjgelenq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gplhasmrj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gzoivvgvq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gznhxpjek.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/grrkfgebk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/grubmcdxw.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gzdnjqmqk.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gcbkyjywk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gbhbotolj.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gkzamsntt.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gehwmpxyk.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gfiakrdic.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/grwonrnwh.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gedxmwdjj.sHtML


<!-- 参考信息 -->