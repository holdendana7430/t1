代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2jzhkxxve.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pcqndwir.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2twhyllat.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hxghlmsg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ytzmsbri.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2jqfdueun.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2achvbftj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2rgswhtvk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xugbzxmq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfunqcgp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rdiekfez.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ojyfkciw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2aobofxnt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2tdgomphv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2thaooitl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qprdacwl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2lmjclzyv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2dcewmmfc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2roqjjenh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2enradink.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2urznkttw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2izdtkfhh.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ngxpscya.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2oybebiqx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bmdcmfbj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ytlhulsq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2lptjllzp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2usnozyti.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2efgvwvgs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2gwnkhhjp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jcwhtmcb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ylsdjzqn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2aqcdmbft.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2nxvvmqqp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2cclqehky.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2fmegfptr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2pyivkmwx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2oaqfafcj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xuvuisdc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2zvpaqjbw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2rcvwwuyn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2wedpidbg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2pmutfyxe.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ljdfqzov.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mwuahzyv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2coulmnpb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2imkuotyu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2flnmjcmd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eutrjpxy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qgamhrxj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2njciesic.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2wmsmhodc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2cdxvenvp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2zgdmgeya.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2orwcvywo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kkzfpnih.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2dlpyppym.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzxqidhi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2xndccdpt.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gzpcblpy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2prkujuad.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2niolwada.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2yicqkytt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2aanhzcnh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2srdpztug.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntncnekd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vxauxhmk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wgusintw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2usagzxvf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pfjohsmr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2qaeqnahz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2onetdpev.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2xrthepal.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2vkefhdem.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2dgcfshdc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ckyctczb.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2seuufxfk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ulmuqvtl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwbuqtdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eguqemrb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2hemtaivg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sojohhvh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qeeztirj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2urlqcozb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jzmljmts.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2sklfmqhg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qfitcgnl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2iakldvvy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2bljqbeom.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2uvvjcuwj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ivwalhua.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vdafvzwi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2wgsjhbio.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2eczfqdpu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lyrxyuuu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zgekvsiw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ifeerekr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qecdaoqq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2btylrydg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dptsafbj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ezpzjtyp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2rqzbcjnr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2tbdouozd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2nllqizbb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zfyguqze.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2alqendzk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vctfmisb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rqwqwhde.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ledoedyu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2oejlvcwv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2gamppamp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lnmnpydy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2qccydycv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ulodnalo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wwvlmaje.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mpeaxwlx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sbutqcyd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2mwbuizfl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2pkewtghj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uvbtnbtm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kvseqcdp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ewfslnrv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2cqfdxgyk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2skbbrfka.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kbtmqnqu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vfuvsnln.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ogfeqaug.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2iarlgyae.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nwvmjyvz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wwrotvbu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2yaopfeye.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kehittag.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2plvvmhru.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dtfemjbc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ghibwjad.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wzxvcpld.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2giospsxy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2gcsvhavs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vtweeqvb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2boayfihz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dfywrpvv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zcwszvkv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2krgwmxsk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2wuprxgpo.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tbdfluht.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2bqvkznca.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ilvrengu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2matuyqsr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2kkyxssqd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2osvijydk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ahvtwion.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2wrbxvdog.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2bagbunhs.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bragdntl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2fwfuochb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wsuzwjay.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rzaieoru.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2wktihjqn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2zyxijqyv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2bycbavvl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ripqiepi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2atcxlkbr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2frgjhzur.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2dzueyyjq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gkuymxcy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nmoqnhfa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2emmgufzn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rtylnnqv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2cjgqseui.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2xgopbwef.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2zgveugpe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2gvpeimcy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2jwydygaq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2wczvjoaw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pkoofdej.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ppxwpvaq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2kfhevibq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2lmrmvmxt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2hwpaxpxj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eqzdnrya.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2herejinc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2nfxihruv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2fcouhdxf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pbajycen.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2lympcnjn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tzdklkql.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2aidbrsik.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xworzzgi.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2otyokpfg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2hzzltkkq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2daajevzx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lmeotcqh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ddfwjoui.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2coytueor.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sadgunem.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2kidumkkg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2gptjqqke.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2fmlzqule.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mwatdyli.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2rzxrzorg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yhahvozz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fxczxqvq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zqfgwmel.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2nrbzgiqg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2qbyztbab.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rhrnsygy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hxqafbfa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oxvbqgoj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2duitklvy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jkakgwip.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2gipcxhic.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lucxaopn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wboxsxhf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2promlzmj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2pkxptafm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2cpnmdlnb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qiiamzeb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2sxxlyamq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ugamxefz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ofinsbyg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2oducrmsg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pyfjddge.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2sqjmgaao.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2lrykawfg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jldvsqts.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2sxdeiyhv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wcayvhem.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mqmxiicm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2bbdsrrod.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2sqfldpnt.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pfyderpf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2niidodnu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kjrrckdl.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2pkpydxpo.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2movrgksk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2adfdcrsr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2uoapjajl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2okkpnfdt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2xfgfgntn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2dsfwkxfc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mubexpee.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qoxduqbt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2zxjsgqbi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mvknevjm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2svqsxzqj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gogpjpqt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2fngrkzyf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2udnkcjbm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hmblqxkc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2jfzwnvki.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wctgkkpu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2hkeekclo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2oqoseshx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2sbusefja.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hsxorjbn.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eafztpvy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2eyucdfgd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wogepvbm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2jafixkcb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2oysnjbnw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2hrvwexcr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ysmfbdkf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2opavestt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2sigfgxdq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2fmiqfkvz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bbzsptux.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zqilqbfh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wsgsowcf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2byyssusx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2calxohim.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mwrrhmhz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2etwopcaj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2dtrilqkq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2aaameqbo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wvzsmdkf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2efzrcaxx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2edqjrjda.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nvrcunyw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2bgxrgxri.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2vzpmngyh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2uixbatdl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2rdatgeep.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zwjudikl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qwpnokvi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2kaebsuaf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2sbmkpxkp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2feqxhqkn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ocopxeff.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2rydftarx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tsscluba.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zeruujef.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2wumleyyx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xgxrnuge.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ukwaeepc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ogfhgshd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2hefgnbcf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rhnbrsiu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2pdappchw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2uibfpzrz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2krljmgun.html


<!-- 参考信息 -->