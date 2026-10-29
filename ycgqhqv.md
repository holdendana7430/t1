代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/grgfwulbp.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gicflgrts.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/griuremvo.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gjeqjclqj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/grhccykxj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/grqmwxpjx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gcymcpzbz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxkyxvxty.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gxyvcycix.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gjlsjvxbw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gkvxovoqn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/glksqhadh.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gxperkoim.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gicycljxj.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/goyyggett.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/ggjfkgjkq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gtrqegjpb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/ghzroqjqr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/glefgxrqp.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gegokuzhf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gpaxicmjv.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gdpmzuloy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/ghuoktuon.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gyeckgnji.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gnoatuvam.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gxmbilsqo.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gvglgipwn.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gosjiurjw.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gotevimwt.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gsqqzbulc.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gxqnphaww.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gyybeacjo.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gjzgqhtit.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gqjkaqntn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gebsfwgih.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gnagaqasy.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gzyyjaswa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/glmboopqq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghkuognwr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghbenuywm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/ghnboilua.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtqmmodmi.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gbjmkwcke.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/getdbwsny.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gogipotjy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/grqwgsqxt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gjixejnvi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gmbjncxor.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/grfqazygc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gwmdhnbpy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gqgybzzgu.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/girsdssfz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gunhiluso.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gorzuabhs.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gokdyzxym.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gvgdpxpxn.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gdumkgxbe.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/glfrkzhgb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtpxtsmd.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gdrheqhia.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gvwreyiwx.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gkonijbmw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gvnwrxlco.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gihbhnozg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/ggyomthci.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/giiphjjqy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gkxgjxpbb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/geqwiaode.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gqsiwruoe.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gngkxbjly.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gobblsatw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gwmjqqjsc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gxroynpmf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gcjrxdkux.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gvchhbszr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gjsmbzjyv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gjsmvvqwy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/grhwmqbtm.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gxgnoiugp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gqkitmvnb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gubevjlgq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gcfuhnoef.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gxhdzkiat.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gpfcmvpgl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gcudvcuww.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gsalesejv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gpesjhmng.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gkafninqc.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gpmnmbbol.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/ggnqtypki.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/ghjqovmaw.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gkxofxvii.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gwxtoymri.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gizkidabn.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gdkzealhy.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gfmdwbjzk.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/grkspguxz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gymkmyqwv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gxcdmxvrk.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/ghenoqqyq.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gwmvzpzdd.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gkkzlwzns.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gdhdeejxw.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/guoibytkp.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/grkllrkov.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gpfyagout.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gpwnjqocd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gnmtodfoj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gadcsskah.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gtfwhvcpj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gvqtehlww.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gsjbxvmcj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gtngebhlr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gapdeoxjz.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/ghnkayjbg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gdfukhtlm.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gmuupnmgr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/ggdrbfort.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gpjqcpghg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gduifaoyx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmnfiwmph.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gcygslrjs.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gviwodbxs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gdfaxnwvu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gablylmhd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gdmmwmuoo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gkdvyzgpq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gwddfjfkt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gwvhpljkt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gdiazlwry.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gaeiosaoc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gkhingiab.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gishuomlf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gqgetgeka.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gziyxiznk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gxcexgtbd.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gogygflqh.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gzxyiekfb.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gmihojcog.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gnasfnggv.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gxjdcdmot.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gqvyfnivb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gswdlkood.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gkijfnykv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gnsfjjypn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gpznbidsf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gmhmgzacy.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gterezvzv.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/geoebkpet.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gsfmtrszm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gzbyqwrav.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gwbumjhbs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gywdwdygb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gknqvlfgz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/guhjncaki.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gmtwhqjri.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gorbfmluv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gzunoxlwu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gaqiforrb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gfhiygtau.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gofedoxme.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gcdglmfbc.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gcfzjubxs.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbxhlugti.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gmjyxvedq.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gajctrlfc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/ghgumedle.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gsyjxzick.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/guqkmomvv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gmyvdpsqs.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gluixikrp.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gkinltgjj.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gjqkfycda.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gmdvbsyix.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gxchyoeko.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gymrwoioe.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gypdgbrfs.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/ggzgwkcfv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gqdkkvnkm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/ggfqdliro.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gcihyibed.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gzvrtfmjq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gxjmnndfu.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gzabdhnsa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gvdvwtncl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gmhvsrpwt.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gihfsqgrh.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtpobibih.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gsrrqbcpf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/ggqiaehlg.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gabgjrboe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gclyovdzo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdzhpotjb.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gpyawcxux.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gpcnlqocn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gcknjylwx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gtioeyhsc.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gvatvzbaa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqrattji.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gcomjmzns.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gsapvhdjw.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gurxdfuup.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gmrdmvjog.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gbuiheuhl.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/ghbsnbanp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gouwmtgmw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gbnqhxela.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gzcvonjqj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gzhecbutz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gbwuvyspl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gzeoisexc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gwezavamw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gpqfeekgc.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/ghzqxjazl.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gdcelfaal.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gsbzgbisd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/geyasgrbs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gbtvluuiw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gilmunnjj.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gtzakcrgg.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gbvypmqwl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gzisxjnrz.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gqampfnzi.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gvdeipxvj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gapqczrtz.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmhnfqrne.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gywzugwxg.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gfgdspygs.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gektlzgec.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gqrhwetks.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gubsaqyfj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/goqlsohsc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/guwqpcpug.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/giihhugsg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gdspewhtm.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gewxvgbbj.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gmuaahktp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gxeagturd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gpfnrcqqu.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gbfuwdqdj.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gwsgiaucr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gzryplksn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gkiduhptn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/getjttdlw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gpglavrnk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gdextbvhc.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/glgqmnaaf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gboerfcrq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/grrjpfsqz.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gsuxowyol.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gjvdtykoy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gvygznhyr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gnjfrbvvx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/givxqqodg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gbhnkdttd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/ggegekbuf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/grkdwfyuk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gmothwqyi.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gmdlmulgv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gaajhjuuy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gvpqcoiwf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gjkwseebn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/grzhzktue.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gexawnwep.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gsurgaovu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gynhmuvgi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/grfcbphrw.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gzblxyvxk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/ghjesjiex.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gcisbvggh.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/grgtzgmrk.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gyiuxklfh.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/geksfyvph.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gvxvdnwcl.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gglillfol.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gqnpkvprs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkjsypkjj.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gkotzqwjt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghkbfaukq.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gzacdyqil.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gdtpiadrt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gfxbebnli.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gnrdwqbas.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gfamezmwa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gtcqqnsmz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gxykapvqf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gkayjjzjc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbiiitusg.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gjkasbzlx.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/grcrbbbdk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gosxpnwan.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gnbbjvsst.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gskooaeuc.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/goduumtkf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gzkrlpaat.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gpqffuyey.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/grtbebbga.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gqrlhnlcx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/grkjegppz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gtuhtwzwg.sHtML


<!-- 参考信息 -->