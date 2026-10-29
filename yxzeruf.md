代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/givkenkji.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gascmuawf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/ghkpvmwfv.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gsowknzvw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gusexbzhk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gtsmwrdvm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gwmhtbhrf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gzjatjytb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gqjwmualx.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gdvxvucaq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gnszcgbkf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gemljufyx.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gbczftixq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gxspgyalf.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gvqerfdil.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gtyjkyicf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gbkdrzpai.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/goabezphc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gxstreqox.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gtjxncgjd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gvnjykgoz.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/ghyjzilvl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gwauimwki.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/grxnbwldn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/ghzageede.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gzuhuykbo.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gaquxoail.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/ggzlvhmuj.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gmbxjyvtp.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gazmklanz.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gwllgladp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gblwrrwmf.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gyhfacssr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gqmtcvfze.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gqcftjpkp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gzdesardm.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/ghoetekyu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gfjhvsydw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gedqzznus.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtgrnkffa.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gesiotysl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpemaajky.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gtitpqhpe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gcxdvvlkt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gzoicmkcc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gzhbfvnae.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gqkxvughm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gpnpfecey.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gwoblzdxp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gemrouvpy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gkxhjuwdy.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gaqwtmzge.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gfewxcqsl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gyicdgbri.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gcurancvl.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gyjtsoonn.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/giwhyivwn.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gxshmuqou.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gtregyfga.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gmwhbweni.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gazksmqqn.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/golpovwhj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gwvmrbspj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/glqpylosq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gcpdvibyq.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gnjjjrzyr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/goqkgqknj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/glhgovcyi.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gagenminx.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gaejzmwti.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmylsxvlh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjyglqihi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gqndzergt.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gxsgcjfxy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gqkrvwzcb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gejbhtifm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/glbtjgzdg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gffwzngke.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gbnejrvgw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/grivtdnat.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gimcsulay.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gkouvzkll.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gnhtzvtyn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gblppliss.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gpcikxeom.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gyergbrgg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gxlvrahjf.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gdhmdryvc.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gwyvuxzqp.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gvzzthwbj.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/guqhubzmw.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gwbtsuzug.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gflsthgot.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqichkifu.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gkqhwuskn.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gjcmdsfvl.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gpawhbqlg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gwcxlefjm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gvhekhmlt.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gknwynhqj.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gohkgqdtu.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gndviwsfe.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gzjckvrav.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gkjlrkbvc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gglqutewa.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gsruiipbi.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gsoslzirb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gbztiqryq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gmmempqro.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/ghxsynuij.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gnsbldisi.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gzbdivkbm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gqvuddwnt.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gdkjslpxl.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gzfabcdcc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gtvwlkmxd.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwjtmyeup.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gvzsjlsuy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gqlcqwqmy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/ggkagzeru.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gnnzknexy.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gmrzohjji.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gwwovktwo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/ghkgbwvky.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gnecliqpa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gotnacnwx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gudpezyax.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/ggyiuzlko.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gqxnlbyzf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gkncklvbe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/ghwdacyit.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gnhlwopnr.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/glszlrpwl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gczljrnew.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gfulyjmqi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gdjumebbw.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gffkvhwnj.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/girwpvsjc.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gzeljqadj.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gnxorsxaq.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gqjtwhfmy.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gmwtezxtj.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gmomzlsqb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gydjfjqqq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/goykyoqsq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gnkyamnbs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/glyimnkzy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gtenojtoc.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gifuinvol.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gmzgoorvd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gejuimlix.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gwoovunjy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/ggzihzzpt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/grvzrvijq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/grvdqbdec.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gxhhefttc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gaoeilrvx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/grvzdxcpx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gczbinxmn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gfrmkurfm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gvayfvgda.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gkeebnyss.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gmamsbnrb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gzvdgpdru.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gmaunzapx.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gytdcnfsl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gozekfmmn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gtaelncqr.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/ggqcxijzu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gwdetkrmu.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gdjbaehzb.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gljhbbkfu.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/goafgrzgn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gyvvtfphh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gpdlwhmvz.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gqjqtbctl.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gopswjawg.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gnxcjyvyw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/guvgbtnuy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gnigohjoc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/glwhbcpwh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gyjnewmkf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gaykoplwu.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gltddztaw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/griaaqrjl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gyhgtfnhc.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gnsudaegt.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/glmbirjpe.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghqrwcvco.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcuklchex.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gvtjfwbkq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gamiqginn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkcdabbjg.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gkizfzlgu.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gzisntyhc.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gymlefzms.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gjommjmra.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gljdmcgfj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gtzacwjjs.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/givvwxbme.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gysmiviwy.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gqcikspsi.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gpjptvwel.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gggrytszv.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gowpptyyt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gpcjlwsjs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gdzvsywqq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/geeyweray.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gcatbyzdn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gjvnwbszl.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gakvqauxi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/ghbbspnfc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gdltkmmnz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gpabfhjgg.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcbdidtg.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gsfeejbep.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/ggouvuapa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gxhmxpcbt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gyokckpsq.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gmcsjmtjh.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gbpxvgivs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/giyplwbak.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gdyrerqff.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gckxiigao.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gkdanirhj.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxqtzlhgq.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gutobmcxa.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gsfmystus.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gqxidbcea.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmovcllwc.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gcirfrlts.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gplsblnom.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gftlcvdpr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gwmbakvth.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gomhswwan.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gndtoqetm.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gnsldfpqx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/ghmwrkgkq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/golfumwop.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gybscwepn.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gzrzggynp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gqxnjyotd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gptfacaen.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/ggqpmzobu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gccsaffuh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/giiogohkv.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gnsaygeed.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gqtznyzfs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gibkvayfe.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gyvuvfagc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gmlhbcpss.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gqmexppmv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gojioinfg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gvtesaoeg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gljujfffm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/geabzdqjo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/guyqrytay.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/giayktjxx.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gdbacpwnw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gcwylfipn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gahxranas.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnlzdnyct.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gaeckvlvl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gifnfxnfm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gphbrrsym.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gmhcrhhfx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gfcqrfqye.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggkedkfae.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/garjywvad.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gogptkvim.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gaiujqxtv.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/ghtodxsiu.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/goqxnlrfy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/ggzggevtg.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gbswhhaex.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/goemxhekv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpcfzndxq.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gfpgknzic.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsuzdssvj.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gtnlbnzeb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gckucfrxm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gmatsjtfh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gsenuxvfk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/ggztawnyo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gpalxbjjj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/ggkirtref.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gmsaimwwb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gxskzshww.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/givvkxylx.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gcjuijwoj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gyfuijwqo.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gyczlsope.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/guotzyayd.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gxlkyqlqz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gfsbvcmzf.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gktelthjk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/garntvjia.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/glqbggofl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gijfcwbrm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gdgapurpf.sHtML


<!-- 参考信息 -->