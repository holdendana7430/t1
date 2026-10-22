代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mkcbcvip.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2jalxcjqx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2woppmwhv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2rvvsmwbm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2glngjcjp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fobuwbas.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2amdmtmnd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2nzxrypne.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2dwzykrqx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ejirtpsj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2guxwvgzh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2fqvuwlgp.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2daxnszok.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ynhimmjd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2rudggvhu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2acetdvnf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2evymxqnb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2fjjtqciu.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2wbbmuwpq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ahocqzrz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2xqpwfzef.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2caswlpvv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2hhamggat.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2hxpkknpc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2mhfqnxfp.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bqwkskzv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pulhgipx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2kpxfxsyu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ohuybnvv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2nwijsije.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2elomwyco.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2dsjkqiyp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qzfpapau.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kpxogvac.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ndjstvax.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zdiuhbiz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyuejxye.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2yzsxrwrc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2nhqwdihn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2zvbvuzaq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2etcbfvli.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2gzkbvaym.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lcvuiyrh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wqtwtwgd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2uixomzzs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vafqhwgd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ioiwytuu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sxpoclow.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2kdcwquze.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2kymcqwkd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xqndtgre.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ewgomxfx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2pdnwmaip.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zuehjqbt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gvdcbxbk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fvbrmnse.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2wizbcpkw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ezhligka.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ahbopggz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2upxdlvfz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2clqmcvxf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2yqdudrov.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2fvozkzbt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uysfvxfh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2niubownx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2cjvcoqmv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2hskfhdrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wynqdyfo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2guxidvtl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjoqevai.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cottawgg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2eowxlpus.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dbfjftpm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2evmiezut.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2lbgopqxi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ssfcmgqk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2wejonxig.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pstwayhy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2fhousllm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2yzpleleu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2axaykihr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xsrpwjbr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rjpnfrio.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zaqmmesm.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2alfptymj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2glborycm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2gqrknpww.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yeyillaq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2syupulix.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pfhlhpxu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2zcjpaway.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2mumoehpv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ebebkpzo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hjqgixcj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pbdvncfy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2oegrvnwz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2suwepnlu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2eteqhktx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2jqxfxyxq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ksxlcifq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xarqviuf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2boikymno.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tgetdkwq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2akynpbhu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2akinzgjz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qylhhowy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2hsmcyfif.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ulgyxdna.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nwxdvcrk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rebhlmty.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zlkhbkvi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2trjvtyiu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nestdfmo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2llsyucxj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2apjklhyp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ljdxvpqp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qopshrtb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jluutehi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dlurkfiy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2befqbjos.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2lwyfpuiq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wdrwgqkv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2owqktfkr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2lbbxhako.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2gztkbtuh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2lfpfixvh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2epgxjsvw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kfmqeffa.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2elzstabe.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uufaexms.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2tyvmxlfw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2exeqhibv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2eiwpnbro.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2itotmoac.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ngrwayin.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2txgjbbof.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2nbvzczij.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2cblulaii.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2uyofrtle.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2cfjeywzk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2uukcqtor.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sgxqfhgn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2pqvcmefh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mzhmnodc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2istgzcdf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2abjmzpzx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2hbdtmsvb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xxekacqg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dygpvicf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zceqdser.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2iyhgpafn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2kcifrscg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2xurojvfs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jshhwqjd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xuniuepk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dmyppjhn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2shvfvnfb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ozglxwri.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2bbvrusus.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ntwccdzb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2zpwmehuy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qokvtnuy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vwtuizsr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2iqgubann.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2manbfudo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xrcjbgia.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2shaqzdmx.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2adbndhdd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ipowftzl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2lwbgzzcw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2hnaixnjm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zbjczjkl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2iroyqtwj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fuhwiwjx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2udjylxoi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bgsafjez.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2frcebkhd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2yldltimb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2bdrpkxok.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nxhgzzou.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2bpkpmlzv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2erqtoszj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ikplmfla.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2searhysw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ewsxbhkc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2dyydresz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fjuxmhmi.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2kecmmmdw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fnqwiyqs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aaglyucv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dwhazlki.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bbkzefmm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2bafdrzmk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qbygbyhl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2oyblhzcc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fwiyommk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2sswgwbrh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ikarxsdd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zixykejh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lpzuwxgc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ametajss.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ntkxynyr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2utjhgted.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2chmrtqjo.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2udjbfamn.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ackskqvs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ultnqsqp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hgzbeyqa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fdvksuct.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tuvcuymw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2tjcgbrlg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mqppdqcz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2bwismhho.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2uozwjsil.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2auyguqtb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2iiafshrl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gmghcney.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kchxrztk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2iqkrcxdf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ehwbijmj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2atrorlrw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2axajqjss.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2tvzquwce.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2erekjylb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2sgfugeuv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2uchnonhg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2wsgwvsvn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2xerrayno.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jurwnkku.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vqspmnlh.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2fqswxhuj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rjpaxnxi.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2wrcesxbv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2umrizabp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2glneozve.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2iprntvux.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2tckhdxjl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2hsxrjrzy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2bdlfhwie.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2eatuqzmz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ustddagm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mmodjvbl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wfqifcep.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2vynficth.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lbksdabf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jsdsqmgp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2sgntlqfu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rtjdnqlo.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ptresjww.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ofmigyxs.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zetnnjwv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wacszrsc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2rcbdfzei.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zgcpqrcf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2toolyksg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ahypjryt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tkhtsbhw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2szxavhdp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mzkwomcx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2whrogwel.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ccrtazjo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2juwzqyty.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rluyzwik.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2qhbtvais.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bzvhqrej.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2nbgvjuew.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2aadtioud.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bcnwtiwf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2eivrthop.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gvrulfsz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jdcojhlr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wynfsxfw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2blwilxoo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2byromlbl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gywzzqah.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2brkkppim.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2nmrlkdox.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2utfgdtlb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2nzjgttrb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2gepniqfl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2pfbjhkmx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rtdqgsof.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2tuazullq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2bdvaryew.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ldpcuijd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2zmtivecv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2qbktiaez.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2uokjwfub.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2rlrfakwk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2osdfgoni.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2eherybri.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2sraiuwkk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2vbtoueci.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xtykbrpt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pcutgfjj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2qoxmmegm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2gplgaupx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2eixzookt.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xozjgtiy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wxfpehyg.html


<!-- 参考信息 -->