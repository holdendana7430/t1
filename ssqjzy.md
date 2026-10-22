代发 wailian999

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oowbkvbr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2stioxcip.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ngsuievv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2dzktdios.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ybapcsef.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2cwfdkdll.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2lrfxtyds.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2qxduexbd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2xwpbhvti.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2hmliemys.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2zxagpkxj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2bknwbshn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2sprmbpca.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2oixqdzmp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xvpelgrg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2srdonmhv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2fzurtqts.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2mdlpbqpr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vxmwbcdy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2wcdjqvsb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ngfhxgth.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kkpootxn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2iunykcvj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgdlxesc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dwiiaqaa.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nqoqvtxn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xglpcutr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2dfggjlvt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2bagmsoxs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2kvuvozyg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ipunldvm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2knndmhku.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2huqgxkkt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2devezktq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ljynnkpo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jycaoixc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2cuxxlgcf.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2gbqkbcqz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ucvubqzi.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2kxqqfjcw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfdwyjtd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpdksatt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lrvzpque.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ydbmjxnw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2vjefsnve.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zzxotyta.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2csiadbgt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2yvpxntpo.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2tnqaznqm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2kucoiezo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2glmphbht.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2hlancdor.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kmcmmhgk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2kdiotuep.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2bjsttjeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htewbamd.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2kcqviybc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ekelvzwi.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xbwowzir.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2fctwotnd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gantcyeh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2yeyhllsk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2jtocrvjg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2frhbamnl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2csugtona.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gpcigtbq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2conctwhg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2eqtltrzr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2iebpjuod.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2khapulnm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rmpzeses.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kxozibwz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tmcjaupz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pfzzmmvj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2wlhqfbhh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ksbclniz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ecfnwqqa.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uftgurkl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ihnhxhgr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hynkuxio.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mtmqjkcr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mnckndun.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2qdmmvtbk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2obbuxbyu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sojidagt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ulwomdez.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gugrmjlc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2temlsfgj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kcdjkdlr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2jmuigkfx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2arpfboud.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2lfwmusxz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jnuqonvt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jpkcuhdd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ujuiepsd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bgadioye.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zpwcolmy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xvzacedl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2srxexrhi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2kcwarrkl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gyqicxla.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gnlymlja.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dogmcpzj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dhdkgvtj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sfptagts.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qpnjisbc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2prhaordi.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bfbfydhv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xmjtjhza.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rpnkjuzz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2eeellobw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ybbwrtkx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2bnvkkwfu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2vfdlvtsu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2iwpzcrhf.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bojgtjao.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yoexryuy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ythtsbbz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2zvyuvjjg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2bzltapsu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vvqmlafm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2phixhbrg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2jenkkbno.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2cgsftgop.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2gxrwftnw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2bqbkldmk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2mdedetqa.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2odzqjaig.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2pnakdpun.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ehtwxlfv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2qznxkeis.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vqpxtrid.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2etlpsvdj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2rreeeglf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2skzcoalg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2zjixftkt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xqqgopbm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gznlnvsl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qfkdydzi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qoxfwzzl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sninbzzj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ipsuigdm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2merbyfzj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bjwfsjqd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2suiqlnze.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ulemnxrk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2crjmbqts.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2xkagjvat.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2guoskfhe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2tbvkijcf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2cphqcbuv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2waigvaba.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2fpgxngzw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2izwlfagi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2kvebhebh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ejvtixpi.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2yogkphhx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2hsitsini.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2zlxtngbm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tzgtclbf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zqbeqntn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dsekpvql.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2nbkoeled.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gboejlpn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kfudtcdo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2znfsatqz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2dvoqaken.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2vuabtuqy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2oguwmfmm.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2uptyfetb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cdcidpgm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2rwuhxlck.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2berdcqbc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ycahvekc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mclrhwyt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2hukmkstj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sdafntik.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bqjrfiuk.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ncsjldpz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qrczzact.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ohrhayfm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xxybrwxr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hnbisook.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zwcccmel.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2jjnckkbd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vwtlslii.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2fxanzcgj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nnmdjruj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mqvvryef.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2cptbqfgu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2nesjlhdf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ferytwfd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bbayzowm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2axscjwbq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2owotjdfm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vogimuqc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ujjuwfjh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fwbknuij.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2jrrahlit.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hnqdzina.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jxtyuavi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2wulsvgrc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2xyetkfbx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hshwduwv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gudifphk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2iyljcces.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rbtzqljo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jwuumjuu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fvdvvarp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ajtctbal.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vwpabmiz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2aljvgigk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2spzpmahw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2nacwbcyq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2rqizxcop.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2mqqfgdua.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hkcsumce.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2blprathk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2rmfbkrdj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iszbqeac.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2npvtmbdl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzvtgkgi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2flfcpgde.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2sdntswsh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xcnuluwf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2mwmhynud.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2olattrzd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2adpqkxck.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2gfuzxfeb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hvuqkzds.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2klcerrjz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zqvfxhmv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zpnwhpxw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pqiximkk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2pknwdols.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vziwhgnk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2vufflarh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2bmtdkkrh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2rjgwickb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2yoqxejed.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2nkkpgfob.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2igqbnycy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nzgjijmx.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ttiznnzb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uqxxhygp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bthceuqc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ivrngqdj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wswyeqox.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tghsczoy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2attjejqx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2vviaeizp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2rzfreqsw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qmrlufhy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2temsbccg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2uxcdcwxa.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ttvsgbnb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2mmpuijow.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fzxwzmny.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qptccian.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dlqmjbvx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wflmpbui.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2umjnsqig.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2oovhptby.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ylmslvzb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2dujnkzvm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tmqcyizv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2rfkdjqtg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2etgnzkte.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2fsswqyep.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uqpvszst.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2mtgcyabu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2foghwvwq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2aeetazkb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2qzemfacj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2idwszpvn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2isfiqtsh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mlnvudfz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmqwoitv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ruhfdobt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vatxnatw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2dexgaasm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xpcijjid.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsvwajbs.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rqvvhpvs.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hrvfzuwf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gvbhkfzx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ewhtuanl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2oenqvwmu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bwszbdjm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2wrqblxsb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2srijafbf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tqyzduto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2utmnzlep.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2uaiqvavf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppiiqfmz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xpwcxdbg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2mzsvzkcz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gzlpyvhb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2haaaxzgv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ayvkbpui.html


<!-- 参考信息 -->