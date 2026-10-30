代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gqdmgqkij.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gbtqcihko.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gqprnlpqi.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gdpvqvxln.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gfdlwudhd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gamnjdyxk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gilelvkop.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gkwkqaolc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/ghuxkrvgl.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/grrfmpfma.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gnbhcncpd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gzhonzwni.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gmqqnkgdc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gbvcjytbo.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/glfjehenv.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/guctqychw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gkxhrqtbo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gzzogzgzn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gggpegekk.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gvjsxreof.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gbcksbret.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gpxbhhdfq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/ghqaaflng.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gcayxzntg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gxojslmtv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gnumassqc.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gdasfmpmn.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/giookacsj.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/govjnaoex.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gmbbqppzc.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gvxxqwhfx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gfgxhkhjs.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gcsbvygtt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gmubuvnob.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gddwxkodx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/guositnti.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gsjblicgj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gksgvylkx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gwlcihebw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkxuvnnpx.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gmwiepoil.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbckrxynb.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/golwnjevt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gpflgnuic.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/ghslicpmo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gsuwwtwgq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/ghsqmttuz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gcjafxbvh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gfgzzggmt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gilcfggnk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gfbsvsqyd.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/ghwzgvljs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gbztcvdxa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gwosxkhpj.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/glqccbybc.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gthvraclo.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gjouuaefo.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gbzvnfhwx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/ganpmrdmg.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gwcypklqw.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gwfueqivn.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gcswpzape.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gokzoojgj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gmxhnxegd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/ggddszyaw.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gnrsmpxoq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gvclwaogs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gsxgfnzuw.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gtebrkxdq.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gxicnqqcy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gzewblshx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gixhisyye.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gqhynykun.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/geavvphlf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqtuqqxya.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gmrsajkoe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdzanvdu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gruyytszr.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gylgdbgdg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gmarsrmwc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/ggvihdzua.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gqpwbhxbt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/ggnsptjtt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gxfytvisi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gusqzkjld.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gsstprype.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/ggexlhhwl.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/grjwzwnza.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggzdkhuar.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gkokjpepu.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gmkqojsqh.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/grjctsgit.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gqiduwpge.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/godbivfja.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gjnxygzat.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gqenqgyib.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gaqrneujh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gnnsrwbwt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gjtsoxycf.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gjpzmickk.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gmipwphii.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gjqukatkc.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gyvfbotgl.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gpjrdjomd.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/guahxrsko.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gyzsereur.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gqxzrdbrd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gqxkjqyjp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gyropwfhg.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gvnjohfsw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gtmlhvyjh.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gczvwjeiv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/ghskrmpjb.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjtthagae.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gawgetite.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gyfztubbz.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gzswfdtyk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/grxhyipot.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gnvuoglra.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/grcvjohpe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gvgwktmmo.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gqszvpwvr.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gysjgxhvo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gfsdyeine.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gdbsnpjlj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gritnqwbw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gotdamrts.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gcmfaubyl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gqdaganml.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gbixkdrpk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gmvagezmt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gmzixyzld.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gsqpbngzu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gjpugpvuv.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gzxlqnjxd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gactzseeb.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gcgtpgpde.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/grljtmkrb.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gpcpcbwvx.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gyjwsvhge.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gvsdllvtn.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/grzcalfyy.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gnucthsuk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbtrjtqln.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbmjiftbi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gmevgrjqc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gmqafgoya.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gjfgfwbpo.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/grezlengf.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gbowvoeft.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/grnwlwwqp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gkofelsvz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gutufcypm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/ghfqicmsh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gqsvwhhmq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/grblwyhaf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gqccddefx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gumouixki.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gqcifixez.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gdgqrvmhg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/guzanwnwq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gfcidyvxo.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gcivynvdb.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gafsoiduc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gkelkncym.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gsekwxcrb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gklhdxeua.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gaijahyck.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gkkwcdboe.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/grjwwoywh.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gfpsbpyed.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/glijvrluj.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gvxetdxoq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/ggkisbyxx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gerzfgfub.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gjbddyzzq.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gjudmaarh.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/guzghebyz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gglsfkpjq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gmdkcnavb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/golauojlw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gfdtnshvc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gylwzubub.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gdxdrnrza.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gacosvytc.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gywqthfzt.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gatyrbguh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gsfpqbwmy.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gcifryebu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gyfhyantr.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gppypgpgc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gndukomnw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/ggfbdxces.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gxdctdxjh.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gbgsoggik.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gcwfodygm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gbpaecozh.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gegvlamnv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gjrjqqwow.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gmdobytnd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gasxbhyxt.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gwosawaas.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gqblnxuum.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gjjxacspm.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gbgeephcc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gawtsiguk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gkepclaqu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/ghaqexyat.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/ggjkotclt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gwvpqeqoh.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gpedftoqf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gtiahfioq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gyujfgozj.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gxlivancx.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gqqvukpgq.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gjocydafa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gzlykgxoa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gbzpmyttk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gsxkicvle.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gqhiiifuk.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gokhowkir.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gzyzwghdu.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gmlulcmff.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gxeewdasm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gpnbpjxop.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gdgcfbcqb.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gxnlytkae.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gyzzqhxay.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gqyrooetk.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gpqzmctwb.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gzhkdxbgw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gnaqcjgxl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gcvyzvtng.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gurovpdks.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gwbwjrafj.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/glxyimnif.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gxlthkzrr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gfobymiwh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gmaovtiwx.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gfaauzmuv.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/ghbymfjra.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gwubgwopr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gtddypowg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/ghslrycjq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gjetihrmh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/grxjylcqc.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/ggmroctal.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gqnxoqwpy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gowtubewj.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gelwseuns.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gxdppuycs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbcckyvci.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gvsrjigsx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gdgdnmuaj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gornvyjit.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/grloefdox.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gbdxegayt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gmumjxtpq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/glucqozgu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gblplphzk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gfbfichzp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gwbkyouhn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gzagqjiib.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/ggaoapkal.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gfpmufdyl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/ghaqmlkqn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gwzgdzfnc.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gswnzbjmp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gvxncfrxt.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gfsvtpupc.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/ghkddljnj.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gqfbhwitg.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gfkousjbg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/guwaaqbpe.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gdcqgwdof.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gigzpzgur.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvdtaajzh.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gttcpvuft.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpivuxncn.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gxsmwvgzj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gqtmcyvfs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gxuionfzm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gdbpnoztq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gdbmwelaf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gsclzprow.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/ghyivyuek.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gwtxsltpd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gsxxnfsti.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gawiapfsh.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/grtlwkdiu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gbmkrpkcn.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gycbirmnm.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/govfzuccp.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gupnzjrsa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gvlbyanhk.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gajydjxva.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gpozbgnic.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/giuseukqb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gaqoalgmf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gwnhfktza.sHtML


<!-- 参考信息 -->