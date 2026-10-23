代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3cgtzloei.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3fjkcqadh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3sgeedjsp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3pgwqzyjj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3wtluyfga.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fldatlbi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3khzxugfh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3jskulcak.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3kdwjtduw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3jhwmabhv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3pmtorsqf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3pufjvylj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3cfsornpj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhgoqgop.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3cxctziuw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rxyvbjzl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xvdkhvni.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3bpmbhkfj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3fmkabbzc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3zshnfhqy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3hgedqfnx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3uxyvzkmv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gtwttbdh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oqmaojas.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3bheensdi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3kyhfbxcr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3rshjskoz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mjfshugf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tgrzrpbw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vlnbwerr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3rueafkmn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3envadpgz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tafdkpqy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ncdrpena.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3daarhoyt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mlzfrdox.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3mrbjfujs.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3svvqjpfv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ltztbrcw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3aupuefkb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ilijfdsw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3mpzuqgsk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3gaqeeuuu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnzukjgi.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3oioktcra.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3dgabxizl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3klotrcdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gioukohw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3gyclgmdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmgjnnvi.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ufkeieen.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3eswwgwez.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ocbvelqj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3lhgkxelw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3arplxqez.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3tocksxif.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3oqphpmch.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3apzifhuy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3kocnbvix.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bftcalpx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3pgukkwos.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3lojnnfvv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mxzarwwm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jibrihth.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yqrutlvv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3nyvdsfnx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3mewdlfjh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sgnekwhd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xcxebrwv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3hmiwkclg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hnbmmcvh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3rrnggdsa.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3eaoaqnnw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fgxewaor.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3uowiidbx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3wergwuch.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kcgobkbd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rbgcldja.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bukmewjt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dltayjgb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ykhqedvg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3szsnmaho.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nbwfvzfo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3gzkssleh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dozabtgq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3imhpfquo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3xazkiavv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3sifgrzzm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lfuxlyzo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3egrtwkfw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3myhzxrig.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3aqxijkmm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xdxnvnad.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3curpllbb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mpskabua.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rkoqyhle.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lbhnuzvs.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jtlxgsow.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kkkktler.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fqgtpcaw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3rrsoroqv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ifbbsczu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3kbkgahwk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3wxiepfym.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3nmyaewvz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ofouervg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vdvgotng.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3obxalcmo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pasuifjb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lwxwcfsi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3rvkdeque.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3kswflkaj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3eobdstiu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3xiyihbiv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3tmxktfor.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3rgageecq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3aqhhokff.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ryxxtlij.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pvwhlmin.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3mzzeziwe.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fiujteea.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nyiezmdo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3jqjdwvtp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yezdysyp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ywywnewr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3uwrnktbn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3gtfylywx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3svnoyzwf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ggiqoczk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lcnbyzso.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3yeylhhnw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qxmyapoj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3amyaywxw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3seubojec.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zpjjpshh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tdkzbawl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3orabtlwx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3smcoxqwa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3iaabqnhs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3zzzlvrgo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ifqbkviw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3uhkoxnwz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aiteuvug.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3sikuskuz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3gaovmnto.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xtoslfbd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3tgmokwhc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ybdwgvfa.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lavlxmmp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3mifzkdmu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3opczkkjq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jefhywha.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ffsfnsjz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3yullttuv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3oxyxjluz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xhncgihp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tczcohyf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3iwsagvih.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3zqurustc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3unclkhvu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hcnfltxr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qkebarps.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zuiidadg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ygnuxdxw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3tfynqdvp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3owvuruhn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wkfmiuie.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3lofazhjb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3sqlghdjp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3enabzzte.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3whytggkh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qhvqikpv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qamqpflv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zqveepzb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gontvobs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3brmumhja.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ybxkhbbb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3btsaeoiy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yyoihcvz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qbiycjvo.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rgrhqnag.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3gxkrmynb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3bkvblnpp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3fbweftfw.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iijquvfu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3fillfeke.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nelpmszk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qrbyydmy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dqddinyf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3avnbacmu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3zjjumrvq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3dtkcpgex.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3femfrpwp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3dsqtbwrp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3oxvymdxp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rowvwbac.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ambptnrb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ipaerauq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3venvpxqn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3jcgtfgvf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3akttpbku.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3dfztlreg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3uutrmzqc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rzhlvzdd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rxxawpad.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3zobmpwgx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3fowlpwea.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3idkbgyei.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3bqwxiusk.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xozdeveh.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ymrbwqtr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tykvlcxp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3lelpookk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3hgyheaek.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3zuhmxqbi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3uahpvpzb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3sxpldymi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3omppwzsf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3oqkudxow.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ltzgqxcs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3brvgvejn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kxuekxat.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3njsyrnfl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3fiqnpvde.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3laxmqglv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ikuupenr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3xmbqbwli.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3nhaacamh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3mdqaxueh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3wvtwnwob.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3yuxtvwfn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3vsrrawec.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ezlkjywi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wokorsli.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ymwpduay.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bvncailw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3phvgeqwd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3euwasxot.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vbvwepxt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ousqhvgq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3nacmzvdc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3esvbjzbo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3dfchgmdo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xipomoyl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3vboejooa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3sthqsqzq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3olyqhagn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3xcajrxpe.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3zolwczpl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3vntbuqkc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3abitmwjp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ekuacqxz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uquwtsdd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3wlmeyfge.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fsvxbjra.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3hnrnyhbr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3oygrnrbk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3tdfeohdg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ledxghcn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zcnldluj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ihqxzwob.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3echnpotu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3htivgjbd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3nlwfaait.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3juglbnvl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3vurphlzu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3mfqkqgoc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3rkbkxvth.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3goartgec.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3mcjnkrgo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3obuvnyyn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3srtmthzf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3raibtibh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3vklzynri.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jggadzun.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3bbxypunq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3rcewpxpx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kswwxqwf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gqrubcwy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3neowkhcy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3btolvmld.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3zjuictwl.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bdcaoshy.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rtlljnfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvxsrdnh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3rayjyxxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmdfkklr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wxbujzab.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3djkvrimo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3zbyguppc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zyqdjogt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zzbnbxxx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3rmifhduo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vbtuwwhx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3sezwjhzi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bnehwahx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3gllpwszw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xayzadtx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3erwybmwq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3goobxibk.html


<!-- 参考信息 -->