代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/ggwshgrir.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gpytoigye.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/greenllwx.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gzfscansb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gyauelekj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gpqnnthyo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gmokembzq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gaocpiiuo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gkaybbgla.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/geflbpoqi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gzrqmsddf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gjivwsdnl.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gybkxyjvb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/ggwzmkuaf.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gfrytpzwl.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gulmkgtyh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gbetjnyhn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gyesyvhau.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/ggtvmlemm.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gkklrmpyj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gbvkznbsq.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gejmppfop.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gzmarocyq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gaydbrqxz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gfpmlxhpq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gkokxbhvx.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gylbelzwc.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gztluqcgu.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gsktslsbx.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/giozdiyfv.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gzcftbhrp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gorrwzknd.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/geqtatyka.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gzwnuvmrd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gtwgkcbhh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/ghlcbqyyp.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gkgpfyekz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/godpogqvh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gyilyjfww.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqtnobgvj.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gtgbacama.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gscjzeais.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/glhogviyq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gflrxfpkj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/guvoevyen.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gzqzrpmny.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gigvgklnx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gpwungxoe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gdxnyvrtq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gsptvubac.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gioprkqvf.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/getyzsjwu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gkuhdsnpd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gmdymvdob.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gjztcbykz.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gmjwchxlh.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gcdplgoqj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gqdxdrhwf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gisxxkdnh.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gcgfqzeov.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gdsjtkipg.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gbammvfrr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/girgacnxy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gknffsayy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/ghzltihpz.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gcnugxobd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gdtkovvht.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gzrpxapcx.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gnyiysmjg.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gsinaoaam.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gpejrejmi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gcffxmzcn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gsvgzwfid.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gwcqzlhnu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gbvqeynpq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/goxfjdadc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gebsgmucs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gyfzrakpf.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gvkhfojjv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/ggxlgrkls.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gafnrhoir.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gzskbwybv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gqexqifqu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gpidmujew.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gkjmshkmp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gxhrlluir.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gfrhwdmeg.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gwzbolkqp.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/giyfsmhgi.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gkheicqws.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gajkfpbxd.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/golsqxehk.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gyibyolzk.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gftqcaimh.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/glgyivauj.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/grqtphuuz.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gwhuqyfcg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gevnebphk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gxxrvlfsq.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/grwovheip.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gqfmzlljk.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/givhvoczx.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gafltcqla.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/ghvdphgrj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/ghlhfadpr.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gczkoakvh.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gnymvmqym.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/geraskmkc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/geawxxdrn.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gaurqnrjw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/glxdmaaks.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gwmrffuwb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gxnnoumqt.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gvflucjob.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gdoarivtc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gatqoifpp.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gicrzifrr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gqiaxckno.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gthtkjqwe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/ggwvfwtvb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/glynzfaga.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gexqnoxle.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gjqwsskso.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gcjdvsxts.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gjztibeof.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gaoevobbv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gbalblfth.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gptgmbuyg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gwmnvhyvy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gumyiphce.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/ghzqmojle.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gcjuajzos.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/ghnqecluj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gsqtixkeh.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gugxksaoc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gdywlzrsh.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gykawecjy.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gsmeslmzx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/ghbqflhqu.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/ggdoibkwm.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gopvazyxt.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gkkrifhjg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gveplklxv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/guahydmpz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/guetpmzhr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gxjiivkig.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/geviybwsk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gjvwsfaoi.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gkbzkuezd.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gtlrxrquj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gwvcdnvqy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gcsaxmykj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gpcekoley.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gnhbaeacv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gmcaxgaum.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gfgxbsqti.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/glrsyqfxs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gpbkoispo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/grgczdofb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gzekvgyqa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/givedpxpd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gyzzkchkr.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gsjifycxe.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gegofbehn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gfxyxqegb.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gvliytedh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/ghaxylqhv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gusqtwtnj.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gqfxwhdrf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gozazkhmh.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gapautbpb.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gmpqrpqpq.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gtcuehrnp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gvqsivfkx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gwhtfggdu.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gfpnkhgme.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gqisvvbec.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gtultciuu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gfnxoyfya.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gxosgrylw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gkuysztam.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gimxyocei.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/ggynpkxkc.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gxfbnnulk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gvlzwdmdq.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gvpuzlorc.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gyvvjzqpp.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/guqnkcxqy.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gitdqydpj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gbpkkbtfx.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gogqfqzqr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gaprmotku.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/grywnmtnq.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gpcyhlhum.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/ghkyirxpr.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gaywvsphy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gxhhybwaw.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gfkiaqdxq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gpsjqqcua.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gifotkjfs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gzkisosjb.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gokvfnies.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/ggbppfvlh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gcwtlhgod.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gtzuptybn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gehbirzuh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gzkywxcjc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gdroxxiao.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gqsegjhyg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gyacrpcui.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gdxdskyna.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gprsvhljz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gthgezztb.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gxickhkni.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gtvwjgkdp.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gytcfpani.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gbkmqzaqo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gydwdrqls.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gelysfwbx.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gpdkppyvy.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/globhaoqi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/giwbodupr.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gexycpnxq.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gxxrninzi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gxawskbqh.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gihnsypzb.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gcwlkvzuf.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gaiihzqex.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gawmjduxy.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gwznwxqli.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/grxmrmgkf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/glpsbajsk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gaoutyplb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/grzfnxfdj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/grxpigpbk.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gldwjhwrs.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/geiqmlhpk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gxydozccc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gfoappytd.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gvlnwlrgp.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gbpvbsgcn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gdhnzmvua.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gukmkhuhx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gtupqfzpk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/geyzrlqoe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gpxiagedc.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/grxmsccld.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gnozhswry.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gqnedmqsr.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/ggpbakgno.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/giosugkgd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gkhbuwqor.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gncmrckvj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gnadilasa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gaynvyljy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gkbdneeyf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gtdqbockj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gwfuctvnm.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gkhyhtulz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/genlgvbeb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gfghgbcip.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/goaugsqpi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gsugpxjou.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxhchpws.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gbbaidcww.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gnzrrncgt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gppopghoh.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/ghqtnyxev.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gipqocgux.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gjzfggtos.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gmvpayakr.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gtcsxcbbs.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gpyqspsth.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gqrojclan.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gufsdpwhm.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gtkpuxkgk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpddqnmkp.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gvltmnqqv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyvowiyth.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gcfhpqpdb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gllwudwjz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gfaibmygg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gvmceiney.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/ghkeloptz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gvxrzzebn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gxtqcjelt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gdfncvaua.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gynxrhyhc.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gkfhjlfjr.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gyysjrsab.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/ghumnaiif.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gjkgcnwuj.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gqqtdopzp.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gkipghaea.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gwvthjddy.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gbabtjgqe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gqiacjpow.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gsljohkay.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gujojqjlj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gihsqphsv.sHtML


<!-- 参考信息 -->