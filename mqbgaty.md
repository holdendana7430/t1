代发 wailian999

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/giqtapamb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/grtuibnbb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/grqgplxdp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gokshdjvm.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gwkqjwjew.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/grmzhlnkq.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gxlflbnqf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gcdermkqs.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gvxnqakpz.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/getzllckv.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gsbecxrpj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gturcguwk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/glfpqhsme.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gmptapggo.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/getgofytl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/grmjssntp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/goomnyabo.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gxwaelakf.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gzthbxubq.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/ggezumxmg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/ghqawzkfh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/ghjdpefvi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/goeafdzft.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/ghehmcmym.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gaycrcgyy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gudebfduk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gwaqynlqx.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/grammsvev.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gyhrbafqd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gnbjzjnmm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gdqmkpnkv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gniytwyxl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gisvycdbl.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/grigfnwlo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gomhhngwl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/glrejfzve.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gyqzaemme.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gmlwlxcid.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gvahgnefv.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gpiptyhab.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gjmrpivsq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gojtpuaki.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gdjldevvu.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gxtzerubl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/giquenngm.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gzkentnhe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/ggcsdndwi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gzfeyjfxl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gmyvsbelc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gcstjuykj.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gxonpkakl.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gtxkgliue.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/glozsfyry.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gvfoyenvm.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gnnuxgtts.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/glnmnpuax.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/giqcvinoo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gttyvaadu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gocvohykt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsdlxrewy.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gknznceed.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gqpnbwinl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/geezwzgrs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdzyututc.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gtoimhjuj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsnkwlpms.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gveqjpfku.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gzxdbbqbj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gpzrvblwg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/grjyyyrup.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gwofcgacq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gfcrtfxoy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gyaveftyb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/groglfrzb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gpeaapnyv.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gzedmclgo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gwedmvght.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gylxstnra.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gfyyphcnp.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gwjopjgkh.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gzralzhvm.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gbnlrqtwr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/ghfetrfbe.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gebbltqia.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gwttmtplu.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gzaumvfhy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gbejlfeng.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gopofoqjr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gwsmtavvv.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/grhtchbzl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/galgivspa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/grqttxjbd.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gmlauelln.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gzonlaqhs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gxogjjaba.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gticuujnc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gzwfcrpiv.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gqoureqon.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gerrsieer.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gjauofdpc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gqepgfrvd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gtxbgxlzo.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gimpzmtlj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/grtmwntbj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gyejnnvov.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gduhzpmrb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gycstlbei.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gssgkiwob.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gewfbwxho.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gzitcgeqq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/geisoplup.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gxkvggjpt.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gbhmexjys.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gambwqzpi.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gmslsxxxk.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gdpmfssrb.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gneaalmml.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gggrtvlsi.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gbtqmvodb.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gusbttfly.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/ghvihrwxz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gtzcbtduq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gugwwphcm.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gbeiwnrpe.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gmqhqosru.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gazsyxzuo.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gykyauujd.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gaasjmmly.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gqpwzbiet.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/ghirdfjoh.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/ggumegfet.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gfzajntlx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gprqspxtp.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/ggakezsfk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gjuopfeyi.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gvhibtvwf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gmvxmjnce.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gfwfcwoqz.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gujkpkbfh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gevzhxukq.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzhqohagd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gyzejjaby.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gdturvvdv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gzcepcpbs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gvmzxqxua.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gpxjettrj.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gjveinoub.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/godowyjld.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/ghhofarsg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gkffvmyvt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gvjvpsfxw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gbnxjrjbj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gcomlxksf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gicaqnxtl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/ggygmcvdx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/grkgryixi.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gkrkvzaud.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gnooofkbj.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gbctagyik.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gjqkqjdap.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gviagbzep.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gnwqmetnr.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gtqntiwpp.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gkzlpsonx.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gmtoxbxbk.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/ggxqbmlqp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gubntclzi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gsezmfgle.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gczbqitsv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gypodbpoh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gmwliuche.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gnhhwxklp.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gzfvydwzg.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gcgivolaz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gtaubuctp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gdcrjdrli.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gptzwrobf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gjyavvasf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gqhrnuftj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/ghcvbksge.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/grchrlsak.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gqgcskrre.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gpuafcfqr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gnzioixay.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gqnxbsoey.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gxyodtont.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gdkomorrd.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gmpvlylmz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/ggbauvxcd.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/glnojiinx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gnyggiirb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gpuvtwvxq.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gfzdkvkas.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gzoqgtdij.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/ghgpxbnjx.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gghazmorn.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gpslslaqi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/ggmuxqnxy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gwailkqnt.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gcgmykxkx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gsjuhmigk.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/galfpgkny.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gbnkjclxp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gysgdnbam.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ggqcnjxfo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/greuxgyxj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gjuczwdev.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gmytbgsid.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/ghxphmkbb.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gxbrjopsf.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gvbrjfsny.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gjdctcrjm.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gemsorebv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gvllfdcve.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gftkckagn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gyttdadmb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gibawwccl.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/ggjvieaeu.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gbcqblkjh.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/ghxcmiugg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gdbshgpdl.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gpkxtiqhm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gyjgcqkpo.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gtqkuwreq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gvvsadpxp.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gbmhpbgoi.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gjapuvxsk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gxmyaeito.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gdypfanyc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfjoosma.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gubwquiin.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gmzpzbxuv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gsixvyrjz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gucjrciko.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gjfjrsbis.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gcmyejrzb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/ggyqnjfvn.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gusgtichr.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gaayrfplr.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gzfrcylvr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gytsbguox.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gqrdqeuns.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/glqhweecr.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gdleomdzo.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gcbcrgfwm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/geloxjfxo.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gxvimlbnl.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gvmskoeaq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gvyyhtjxs.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gicbkjdjv.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gcpqjvymq.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gonawgztn.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gpepuvknj.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gwyscnxgy.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gztxfkfiv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/grhquepbp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcegrtoqy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gscvyfmjb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/ghauysuax.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gszbfhkbn.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gnllqxjic.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gjhvefgwg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gnwwqbxbs.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/ggbgecaaw.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gycxzsvhd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ghisqfona.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/ghnldimyq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gstqmlvio.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gjtconhdo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gnbsgrqlt.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gppzfjylx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gssdyxoxv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqmvetxhq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gxdmsxehq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gkxeytzlw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/ghuvmrmxy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gbggzhxsk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/guczxalap.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gyguurtyv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gfecllhpw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/geynnakna.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gxksojovl.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gidakwgpd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gpneipwma.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gfttxtfch.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvwqtpwye.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gykmifldq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gxdqvjtjp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gixvtdpek.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gntavjbav.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gcxwhddry.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gjdmnbteq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gvapswafl.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnfpmhkpr.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gwkcltxiw.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gfvzoshos.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gqziqaolv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gbsowojin.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gsskgodiq.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gchiymzav.sHtML


<!-- 参考信息 -->