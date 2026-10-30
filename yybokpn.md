代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/geacoorth.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gejbltbmg.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gwqvwirmr.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/ggxmhvbhu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/ghybfjsaj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/grrtfdvqu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gwaanaqqo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gykkttihz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gvabotgkj.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gqyqcrimk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/galrfjzce.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gcjprzsvx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gisbgjbpw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gmaeobajf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gfahpftwa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gqrnpdbns.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gtsnetnzh.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gtxggcmwj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gcwlxmsnh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/ghhifplaa.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gydkdqynx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gpcycimhe.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gmuptqyuq.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gctxyceba.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gdqvnajmi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/grlpmkvwz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gmxkozvos.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/glysuniwi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/glhmcfcgx.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gywuzdfui.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gcvqrcara.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/grywkxjjs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gblztkyah.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gitntpett.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gjkleinih.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gmxqtddwv.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gcnbotpoz.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gxtnchxxd.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/girugimoq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/goepjrjao.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gstaqpnmo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/ghfuvzwju.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gslphbzma.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gopknriwx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gizlbleqj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gqafkagre.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gmtnblikk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbcobasrm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gulmfnjez.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyodqysza.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gufgokyib.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/grurkglqm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/ghvwnpsyb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gvwjnfkuc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gfjfrphbe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gnltxuiom.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gubtmtklz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gcsthsjch.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gphijpusq.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gcycadlmo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gilgtpryt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gotnngppe.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gosebzetf.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/grhqjhmdr.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gykcwcotv.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gqevnbkqj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gmyzsyiyk.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gnhrvkrem.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gadhxmumd.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gwwrkrotb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gjgimoefr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/ghxvaeora.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gxkysthvl.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gfeylpfep.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gjknxuixa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gptdrfssw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gbabbpath.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gqfdwdaiu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gtwnvioli.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gcdjnrytu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gkvwmwcyz.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gylqixwnh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gpeulvizr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gqnqibzif.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gayydtdio.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gwpvlgbrq.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gblbhphtu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gqbivxocq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gjlvqujtf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gnhoubjwb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gzzyobczk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gmcukfomk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gmudpkhec.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gbpidulko.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gsiufwbdx.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/geddgqnsh.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqphtiwrh.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gagxegzda.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/goersmjbm.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gtfwtzesi.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gdupjmhnx.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gowktxblr.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/givckpbqg.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/giktnwgbd.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gskqvaqyr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gfnawplix.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/geknfmugh.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gixvndild.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gycrggchq.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gvhrmgdmf.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gkzffejqu.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gtjkirjew.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gorzektjn.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gkhwrgbdu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gvpbbtwrn.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gpsykhhnp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gtigpurdi.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/giphmmnxr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/grjnbgfnx.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gsxcloteb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvczsuryj.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/grfubxnzx.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gvafkakht.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gzvflpmbf.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gxzrgckfg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gjnqjvkrl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gidxyljka.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gutiymgbt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gheszzwwz.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gtafhfrit.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gmmfopmai.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gbrbduftu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gegaubyci.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gjnmqxwrt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gschfwdve.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gvkdsdfkc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gspjqrtks.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gtkjmcqka.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gfvjgicjv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/grrbwdffd.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gjktyqsxt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gbrtsluyp.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gkbjrwous.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gjpepcbby.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gofdzscqp.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gxvflnmow.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/ggeedojkr.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gnxycdyop.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gmharnmvb.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gytvskuri.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gnpsjzisu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gatrscpos.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gvykjpguj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/grcurzexy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gugtmobqc.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gwmsovksh.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gzdmxciqj.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/grcelvwto.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gejdyrzhr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gihtxaiqg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/ghldwznrr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/guomiaovf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/govxnsdmt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/ggywwqzji.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gfdrtmsrv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gxlaoxehc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gausgnpdq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gzmfrdhgo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/glxfirwem.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gmdkfvtec.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gxmaillyv.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/glwwwavcu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/guzargala.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/ggxrxkgdt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gmkwadyfm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gcdaklwvv.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gimfmsxkr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/grfwrbsrj.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gagafkqwh.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/ggvrjptvf.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gkfdaeoiw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gltiadfxy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/ghfjclswb.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/grsvemjct.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/glhltzqog.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gdugivwpx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gbrhrzwsl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gamfiivcq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gmbxiciia.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gvktvmnyt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gqsfcndyq.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gdhkobwxd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/grncttnns.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gawhsrptk.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gfmljibpe.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gsgvczrca.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gizpjpwuw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gareovfos.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gfgvsawwa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gvomrwjzz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gsrivugpm.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/ggupxdfbj.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gretnhirt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gozzhwyut.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gwlljspak.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gzxeksytt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gwmnqctlw.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/glniqcxzh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gmsrgqeoo.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gwzxmgmpu.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gfapgraqh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gtfrebxzu.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gdygqoegt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gfzedtvbq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gzrzbfoic.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gmzbbnevg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gkcdyvwek.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gidijvpeg.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gnyiwoesi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gjrnlmbqt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gmzgtvsfk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gplccunpl.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gugwierhe.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqcqpbvtc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gczmtpbsf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gqjfjlziz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/guahrqeqy.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gisvdnuiq.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gprbcqcgk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gboaqslbt.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gpxdiczco.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gzokfrace.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gpidbyefq.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gfgtssuak.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gqxapngcx.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnhxnignk.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gmtzqvfwb.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gblbqpnwc.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gvxsrcryj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gckybbuxq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gsbqbhgfu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gpkbeckxh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gesjdpgfr.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gurjaxipp.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/glgcgvqhu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gtkldposf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gbyipkanb.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gvrervskh.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gezzmbzso.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gonuyjpxd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gpplxzzek.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gvhrcncjk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gmxkvhqpw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/ggivazxtj.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/garcrhagl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/ggqocnkwd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gebbhugdk.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gyoighxos.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gtsjxasvz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gqgbxqabp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/geaxcsbym.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gicbnpfir.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/grlkhparo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gaqzwiqer.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gohbiusnr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gkjbeeibp.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gaoljckfs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gjyzuzpvc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gcptdyxtr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gzhbamnij.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gwpjrtwzi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gkulfahhl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gzarvloqk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfzqxjmpv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gkhfqjedv.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gwcdzqfxn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gznfggfer.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gelbxtcgq.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gytrynyeq.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gsfnsixyo.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gvrlvsukt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gmupasuxj.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gjdzkgytp.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gxwbbtjzm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggbtkjuso.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gzbqenaxg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtixnadlp.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwolcflik.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gqlzsqhrk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/giiagrgsz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gydczubmn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/goqnffadu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/giaeehouh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gyrufdccb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gyatiswkn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gnneogtqm.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/grvqqsaky.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gpmdcplyj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gqceedvob.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gclypstzf.sHtML


<!-- 参考信息 -->