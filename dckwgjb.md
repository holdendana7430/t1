代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gheysjnpd.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gxhoujtay.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gedqynjan.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gsxjsgstf.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gcbqtbvbw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gloonwtuw.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gnezlxqls.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gvlifgiom.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gqmswtpze.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gxquixegk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gcxxlrklh.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gvgsqdrpn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/ghpbqcejc.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gldxvcbyf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/goucocahs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gnisoyosm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gryclnnbx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gnsxzilyq.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gzwudvcbx.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gedspuxcd.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gdlmgxodq.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gckjbrvds.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gjdiitbqv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/guskkjdqp.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/grgkkmyxb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gkrbqlemu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gbqopocsd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gzixldchr.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/grhwjklpa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gneaxjxwt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gbgcjvdxh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gulrpplms.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gohakpnqo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghgwibrlp.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gwolkvviq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gfpdlbxbn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gxcttuihx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gnwnggrmv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/guesqlphy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gamkhkkqv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gfolnwjip.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/goeisoqgu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gdywoeruy.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/guhkemnpk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gcnekxljs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gnhxrzgdg.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/girbbasba.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/glpmkkgrn.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/grcecrxdo.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gchnvgzpr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/glwctpkoo.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gquzokvfu.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gqqzkwztr.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/glqnrbewf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gmvuiycnb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gimrkwcim.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gxgwqwwdv.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/ggzgotwsm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gtawtmngp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/ghfhfoyuu.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/glppgizce.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/ggcuwbdti.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/ggnyskucv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gbnhxolmj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gerddfrne.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gmpbjuagr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gxprbbzto.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/guivlwixa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gkavojjzy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gsjtzfiae.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gdcoygahr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/grbpzllkk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gawfuyhho.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gtalvcosw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/ghmyzoiod.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gnsmvybop.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gpctjqdmz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gxixxoktu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gbylkkkpz.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gcatqgada.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkasfngwo.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gkcgrgecu.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gviiuctnd.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gfmcciagt.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gdodpokvu.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gdsvvzyds.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gsbigqivc.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gxpegvbrn.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gzscrptld.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gtcrspzxz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gejanyaqq.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gbellenhf.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gtdvsdrby.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gavyoinoc.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/graxavtqi.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gtdtbmxhx.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gegcueocr.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gviyujsqc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gachykilf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gemiwfvga.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gqmzyaqhv.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/grjfxjxyv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gsaegvrvu.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gtoguqtrt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/ggfmcgdfp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gbmymvreh.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gclspqwiw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gvwlhewwp.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/grvirclxf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gfiokkusq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gmttrszqf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gvxcplkjv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gumlbvnrg.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/ggtixugia.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gxvtkrgjr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gneyjatdg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gsxfxibty.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/grbdyreli.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gixwlblbg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gyqckoavu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gkuzipzcn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gupcdtrua.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gcrnhpfgj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gvmsruirk.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/ggcthcikb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gwsfganku.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvodnmcsr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gyqngrvds.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gftksnpfu.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gywagyfiq.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gttjbhqgh.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gkokgazva.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/ggupnellj.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gfovbfnkx.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/glugykrzz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gymsqiqfl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gpnhrgsio.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gornnfzat.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gnyylqway.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gasuiqfhh.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gzeoqynih.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gqcpqhika.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gqtrgtdrj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gduyfnfmp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gckipdniz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gjjxlcluo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gciaczqhj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/glvbwqndb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gjhsutrco.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gitlxypli.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/grmyjnxij.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gfczpbnkj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gsqxgqwqi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gyxcilrec.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gunqdpdgn.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/ghyxxqzyj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gtlchrfrw.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gtgzfnqkf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gwvitdayy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/goamgdqjv.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/geqgwuyyf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/ghajpaehv.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gswwvakcw.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gllmcfwyj.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gmhaeusbm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gnmxorann.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gvqxmhpqb.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/ggwamgomj.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gqwalnzyw.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/guykopydk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwlmleeiz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gnjfdfxrh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gzykempmi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gzerpdvdp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gnpkereza.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gxoqgvkwr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gbvbhdpkp.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gnbbxxlpf.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/glwztnhzu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gycwhykln.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gnqmuswru.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/glkbzypug.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gclpysoap.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gemswkquv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gozyewjlw.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/givuhjcug.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gtirytjpy.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gpblnypbj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gnffhekxl.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gscrpwgnd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gxzxseoms.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/glaidqzll.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gplqpydnr.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gkwpqeffs.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gbexdralf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gxysxlbhc.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gimngqwhf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gvjafbppy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gmbozvtsd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gsjjnfpul.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gfuxqgltj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gcgfkfcqj.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gmknjtlhj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gvyexpzxo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gmozhqzph.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gobijuuza.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/grhhuetsr.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gkybehxqf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gqgklaleu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gscfdvafo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/guzvovaqp.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gqalgrqva.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gbssytapq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gpsjxcbhu.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gipfdznbh.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gkpriwesu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gyyiofswp.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gulxrlwzl.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gydoscaxb.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gakvrahwo.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gdqgmpspp.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gstumvemi.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gczutwjwy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gqarkisoq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbjajltqf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gqashgtxa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/grsaptoqg.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gkurhkptm.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gyjhxqmik.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gfdelefjj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gkvvvobex.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gjwscoycw.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gurfyuaxj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gwdbjdust.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gcufrmzcz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gmdvvflwk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gplbithfx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gsehsokxy.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gqeujudmm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gxhyowiia.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gepgqyvqb.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gtbanrosy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gkdbghaph.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/ggpokfmwf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gsnnrexeh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/guqljpzma.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gfgdidboh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gcpokdkcg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gbqcunlkh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/garcqbzbe.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gtjiofjcn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gffjlvcue.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gfpoyrzob.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gqfkgnfnv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gnjklqwnq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/ghdrdroez.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gngwsprgl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gefewyhot.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/geeydfvoa.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/ghkecriti.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gmyywyxza.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/grhaweemq.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gvwvdlprr.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gjcyllcnj.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/glwcpyrfs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/guutoomkm.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/giqyjldmr.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gbhgqldmr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gosupdysn.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gmxoyehex.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/giomubigg.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gnxwhcdbd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/ggaiwupza.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/govlsnupv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gyogazqfp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gqrsellzb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gbaosqfya.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gqxtoefbe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gsiptypza.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/guxfxndzy.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gfwusnocm.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gxputvtwb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/giatkfahu.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gyxcyfrbu.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/ggvvvurwq.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gtwycggwo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gwrtpgnpk.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gdnvswrih.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gdplipjyd.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gmzpwbqol.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gkwwaediu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/glypfdmzj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/ghcypuymx.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gjzvovrlm.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gaizjyfla.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gsybpzmqq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/guzpsovei.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gskeexcpl.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gkmudxwfk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gfmjhehkn.sHtML


<!-- 参考信息 -->