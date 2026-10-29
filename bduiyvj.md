代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gxiyeztaw.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/guaswlikd.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gkcvxooxh.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gseyedyjg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gpnvnzvlx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gvabrjnij.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gbinekfzi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gexukrpqd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gomavdagf.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gjjnhlimb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gjqwqpikv.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gcufmquzs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gwdmcnjwy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gskgicier.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gsylvyrpb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gfqajkwjc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gxhofbdme.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/ghoiwwcku.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gtuwubvsh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gjmcrgipd.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/ghmcovktx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gxzfpqtiv.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gjbpodhxh.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gnypvqrhe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gvuenekyo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gaxgebeim.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gamjcrvhu.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gbhwzaawg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gmsazdusi.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gfiegabdt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gybeobkve.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gkdatauqr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gpraijhkc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gphecmzup.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gsnszcxyv.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/grozfnjnn.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gmddvbogd.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gjhmwbhuy.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gnwiszinc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/ghpkdpozi.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gjqduuore.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gtzopzdco.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gttefwdin.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/geqlnpkhi.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/ggplhzuzp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/glsbebirh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gbnoaavhz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggwwlsqsy.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gyvvaoipk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyvehcmgo.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gmwcthwwk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gobqyckuc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gsogqgpmc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/giccyugro.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gdbcisvxq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/ghedbvikg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/grbjywfgb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gjjjmtsxz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gjdvscdng.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gxpnabmxg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gzydbgswm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gtaelxcoe.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gkbsruzsy.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gqtjkentx.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gtvvonyub.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gmudkdloh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/glymkdtcz.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gkifivmlj.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gqudnknyx.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gilognlnt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/grdwxtxmu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/ggaehkvfg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/guqmcoegz.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gneagouop.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gubivweid.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gczacuhka.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gkywpssgz.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/glxlksowk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gabpptdis.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/guuqyfzng.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gtrepavna.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gdybonddz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gkwleqdmn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gvozoolpg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gnrwctbua.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/giklmudmh.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gualcrvgp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gkllqgswz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gihgsgmku.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gpkuzxvex.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/glcubjxmz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gtxeknzxz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gohhntcro.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/glhqhzbxm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gibrexrvj.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gblynapqq.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glpsfcktg.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gncwhswba.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gizplzijm.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gwuhfjavw.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gnalazzea.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gztkgbkcr.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gbjfdzyak.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gqmnrnnfg.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/geydquutf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gbjkrrudt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/ghpltklvt.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gjificzpu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/geogycaip.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/glrofpgcr.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gakivkjja.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gchmnbqth.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gfmqoslim.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gjprtxcnt.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/guihyxtcp.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gonkwffmw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/geomwubsz.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gurxdcxmb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/ghcsgnptz.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gohwsmzzl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gqohhcldi.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gtnoganrw.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gywuajtnf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gyuwoqwlv.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/guiknycyc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gjksxohvy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gdjsvkkva.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gwmclgmbv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gjnrisppp.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gkiflhcpo.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gxtmddcad.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/grkbbeuul.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/glleuygbc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gkwcxzdyp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gvuifslze.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/ghbrvwsri.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gmrowoemd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/glqzclioq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gmwkqijvj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gxcwcwhmn.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gedvjtqnt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gxpsusxna.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbzugnsqh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gnqanvcqn.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gamjldxeh.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gbjwftjys.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/goilutlii.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gmncokohl.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gderkodjt.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gksnnwuwx.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gjpmnzmqa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gcqzefxya.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gaiqfjxwn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/giwygeukn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gqkdaqycx.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gktwrvfxy.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gcugbbeem.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gkmzincfs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gsrnsudnz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gidljmmnj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gtpkdwinw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gjfhkvwjq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gmvwyyine.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gnskzwyvm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gktidqlqe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gjepoxhzt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gpueyrjzw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gnywjsewy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/geekzatgk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gkemixxeo.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/grvnesfdo.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gtrlqlmka.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gufvhrgel.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/ghfuethfx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gbhxvbrxu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gowvogltb.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gtqnpviwp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gwcfffmjg.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gzmgeiulm.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gbuibqpcf.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gugfutevm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gbhenqmte.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gvbbkssrh.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gxpyzregh.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/geyjbzwga.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/godaiakqt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqswhbwvd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/glgtvwgis.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gfcxlplla.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/grhkubudt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/ggmectxqz.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gakbxvnsd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gndndwtny.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gwmarmdux.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gjjkxuqyu.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/grsmgzmsl.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/grwtrucmq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/guwdyiclw.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gyxjddoif.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/ghhtdbgnv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gisrghzgg.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gzoauusfl.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gfqneicmz.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gtjakymuj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gnvwgtpds.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gcppxkezn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gxmiybnlq.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gysfdfdon.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gaohykstr.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gtuaolerh.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gnvghivtw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gdmnefuoe.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/golpxceag.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gfxuylnqk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gbflxdfbk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/grxiaiirn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gldzrbfzm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/goeycxgmy.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gyddfcerd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gdhpigwmm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gdwavnkte.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gvdoppcjd.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gigmbzzeq.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gblpszgft.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/ghypqastm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gqyohumcx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gyjxznaci.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gbuzhbazk.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gcyxzemxl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/geuxhqvij.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gcvjemghk.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gihvzrkpk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/getidiwgt.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/giqlspooy.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkebdnetz.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/grznmnxyg.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gaxqtsivj.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gzwfwxhey.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/galkmozpp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gqufrobrt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gibzeiqrn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gajogufpk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gsichzifw.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gtdxhhymy.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/ggmyvrjpn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gnhyaozhe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gszxffrkx.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/ghwohygso.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gdtqrhlnt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gbvtirnsa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gpgrvzaal.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gfmhbqvhs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gbmszaxou.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gogkqpogf.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gjhamlkpa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gbelseowm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gmidzxhsq.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gpzijbygd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gllgazvsr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gfluhvqgw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/geovwuicb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gktyzbtku.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gmxwwajqk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gfsmqioxc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gwdhbfxiz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gallopsjb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gajeofiwl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/ghnrrbzgg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gxvvucwke.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gmsxckuni.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gruqwdyio.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gmpyhlybv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gmnkwpxys.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gbfxrqnzh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gndmboohu.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gsfllzwzs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gvwsysdqw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gzkeppsnk.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gvukowkky.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gffkhtzue.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gupxmyxgh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gfdiikryc.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gjiguwaci.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gnbghmvdp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzflxiyxl.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gobyptllj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnrzjnrcz.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gmnoxtzbq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gggpzgwcf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gajhdrhpb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gpkjdbccw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gsqjksgeq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gbofyecie.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gmymhfqdk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gbkfhkdpg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gheaxevsf.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gkvubbcpw.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gtcsbrafn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfizraisc.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gfawlwxiy.sHtML


<!-- 参考信息 -->