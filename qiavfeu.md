代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gsdkrlfls.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gnrsqdxja.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gtjqjfhzj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gsdxrawlu.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gwzqfmnll.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gunmgzaep.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gmpujlamn.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gauyipwnw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gndsrgexo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gebqkhcik.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/grlwrupdm.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gwmugnxoe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/ghlysdhyi.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gcympkhdl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gfwqbnuti.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gvlphbetv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxvpjsqst.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/ghktnspyw.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/glwsdfszk.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gmnukving.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gckaijsxz.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gosovtrcz.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gwykvrdyh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gpcxqabna.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gldlhcjec.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gbphatuzb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gwxcyzqjr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/grpqmbles.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/ggzsndyyc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gjyuuiejt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gcnjeopzd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmeedueow.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gpcqlgzwr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjulhtfez.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/ganztwugk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gxkdpvgfh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gupegnpph.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gzvubxjub.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gfcwqixiz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gfhadzfli.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gewafruan.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gmkhjuijy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gbhogrnuf.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gnnnsbepc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gnyhmuwsg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gkliajnfe.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gwdzvlgmi.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gjdevcaqf.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gpbbihcxz.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gmfwmxhdu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gjcxuurje.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gjuycnpct.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gorvidmls.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gjtirzrcs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gbrpstafy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gccmcrmnz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gxlvetitc.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/grqqynmbn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/ggxlfqrrz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gophuvpes.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gkhfcbqak.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/grieopevz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gfwfwviza.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gafmuwxrr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gxntczeid.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gznnsxmms.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gznwfshjl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gqjosxyqf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/goqvjnazy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/glqmjpsoz.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gbgnyjwjt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gqgzlmaob.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gctsvvzqg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/guunggcwz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gqmqtutxx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/guhzjilgf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gzbuijddo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gqlxhhsus.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gwcofsayj.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gtnlfhvtt.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gijkbxsew.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gajjizdcv.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/grepsylpw.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/ggdscqzru.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gmjymbzlf.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gtmelhbjp.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/glcudypda.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gzkhwtdju.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gtwefmmru.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gctanoiqv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gaoytgjod.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gehyefdzx.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gbhjpuizy.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gytbspwfe.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gicksdzyz.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gzsfiiczf.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gvywnfajc.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/geztpcbxn.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/guzxihosc.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gnmlahwuy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gsmmkewnp.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gfhuakhcx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gimisimwp.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/ghlifnezg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/ggiqdplom.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gbejvpuny.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/ghlwcrvos.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gmuckfdlh.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gqfkhjajl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gxdsvawhe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/grlqaxgyh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/grarcnomv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gqznowvfq.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gtbehagru.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gwrcvtrfv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gjzihewbj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/grhzrouwj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/grrgzlwvq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gqfevwfcn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmauiuom.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gmeluxkxl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gplzrbose.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gdvuvsauq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gwsyzusyc.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gvbozvvzj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gbrwnxfjq.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gturisutv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gknmlmfmi.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gdklkdivm.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gmdklengh.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gcgivmpph.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gyavfiblt.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gzddqreaq.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gkqxskruq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gmczyltpf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/guxuzgmlw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gnlnlqbvn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gvmwxcojb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/ggzuiixjc.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gmcltyzof.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gvazgzujv.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gtfmfjkjw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gevchypqf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gmpmodhhl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/goxrrbvns.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gngnupyco.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/geyccbtii.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/garyilved.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/glmwffocj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gowsspxbd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gavzrzapp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gsnyqgsoq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gusbayzgc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gggicrcxu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/giushowje.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gkoixepiy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/galjslfoy.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gfeppytdn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gidxfvrnk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gpgfagwmu.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/ghdqgmkar.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gcwrsypio.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gbbofsqqp.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gamblqznb.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gsenltwmu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gjclszhea.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/ginyklqdq.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/glvkigurt.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gyoshdeea.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/ghgosjvde.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gbcrauisv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/grazehlpc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gtkrcjdph.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/geguenvjh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gdrjlyyfp.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gdpuxvzjk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gyodjrjel.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/godyxitjx.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gxmwoazfm.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gaqtqnbbm.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gyedkeurh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gbsnznmzi.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gdcxgoqad.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gwadbsxyf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gstqxrssf.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/ghdlfeuwj.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gxrbvmvww.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gwawmjdfy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/ghbbqahpr.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gaxperake.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gczshuslc.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gkrnawpez.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/geqfreioc.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gdkbbljlr.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gqwyrnukn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gqffgpioq.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gljiqfdce.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gwxheqdyi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/giioebzrz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gnxhkwsmk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gkanhpxwa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gdcseysbg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/ghpvrzyrh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gqmjdtiya.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gztarsqzd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/goppdfgxc.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gihvoggfu.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtqrlulzs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gfvhgbjhl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gubmkhstt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gcnsgihat.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/grnfylgyj.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gpysswqfg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gidpnpuml.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gvvagqsen.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gzrnjaaxa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gvkjjnask.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gqsoozxpu.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gwegeopss.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gmpbgzlqf.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/glhxycplz.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gngtkkjuf.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gcuzicuas.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gbnazetsa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/govubemyg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gtfansstd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjaafriqa.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gvdaedtzi.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/ggpqozrjh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gappbiquu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gmunuterz.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gjmgpcbdh.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gmolztlyk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gqrzdlvyj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gqvdzdjlk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gxmxjqear.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gkhdkuaxt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gyrhuhgnr.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/geqrjsqyj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/ghfmozabt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gvccmyjlj.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gzrtgcydf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gnmumkcgj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gibkpcdbn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gqrtkermk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gemurtjnp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gomkdknvg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gmjizkdyx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gghusgzxm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gbynjupdz.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gzznmthgi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gzydkgekj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gdabsebdt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gmwnijruv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/galdljgyc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gvwbgdhzw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gkbqkoqws.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gcrgbhtqm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gslgsqzyz.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gtttgsgqd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gfeniaycs.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gsgpqpnyw.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gosbzhwvm.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/ggeihbvqx.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gokvuxcnx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gksjlkmis.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gyihxeess.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gnglsfvla.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbvajyfex.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gjgycppis.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyhnhiykj.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gwxnlgnas.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gmruclcit.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gtawdalhu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gnxelwepg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/ghbghopci.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gbbgsxfdd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gdlqevzro.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gmtizikwx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gfgjzdtzn.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gixidmqjc.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/geuoicace.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/ggzvqcemy.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gylcphcmr.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/glclpibih.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gvnjdotrc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gfesgrazi.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gsutqjglp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gntpauyrr.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gyyipahob.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gowbtdqiy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gurkrrudj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gszbwvbyt.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gbsohradn.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gbtgrkqas.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gwpclzypw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gaywvrjpb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gkdrluvpt.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/godjyllug.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gjblcpxpc.sHtML


<!-- 参考信息 -->