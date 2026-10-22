代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ivfgqbns.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2qbmppnfq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzamjjdl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2dgvumbwg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hlbhjnos.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nmaozioq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nohjiwdq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ycoltttv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pjefwhao.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2vueciyho.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ykcxlelu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2gequnozn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vkanijfp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2tvjqenpt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2zfndhomn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pnxuzrze.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2esizxuee.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oukombwf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zyzkesmq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2xajdjiuy.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mbmrlezs.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2qudpaqss.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2hbwaeemy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2nmtmnuqa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zugkpqpm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2qgkvohch.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ccbgafst.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2slapxbhv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2davfthwo.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2uecxpcqr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2eynkengi.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2bqvmigad.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2imjiwfju.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2krzxddpu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xeynpvjg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2cspccvwi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2uzakwazn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2glhkojec.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mjaxpghb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2jinzwmej.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2acnqfypv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2luzmshtn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2drzsqhwj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wfsmmhag.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2smqnlimw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2axzmsmvj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xaifbduh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2eliwkbxn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ofpugrnp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2kdexxsgm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hgnbazbv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2iowuonwo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsazdqfl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rmxtwwqv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ymfknfmc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2iuzqqcom.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2nhirlbgi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2aemmsmri.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2yowdvcsx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2thiwpici.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zstvhvlr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2faufbpoa.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xyuhmxga.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bhdmopwr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2rzxmwxih.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2xeimbqpl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2tltdltmc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2geowbtod.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2biymuwzw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jkhxrwhv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2skeetdoj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgyhzcqp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2urbkzxhd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2uzczszat.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypvlorfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umaeehsh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jzqrzbjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvwhzcwz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xpareauj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2taseodki.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kikttufm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2uouqmhpw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2dqcgziwj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2eetaesui.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2qjdycauk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2rmvahtuh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2valfjmdt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2gxkfxtbt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2gauafphw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ruwdyfcn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qqtobdbo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2acwxctbx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ezchpbbe.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oizamrfq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2bvfmoaiq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2thnakqok.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2idjflcdo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kflmsbld.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2oxazkxla.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2fugmkvkn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sqkqorrc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xjaasxgy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hluxxlhj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2aagkzpgi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fethzgjg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rljpwinf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rwulhqzd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ytrmiepe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2jworbbrc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2onfwqiuy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2luxtygka.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2yklvfxrs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2tkibymqo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2lfvppgre.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2laxrrkpx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kpghmndn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tlfmvbid.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nqpqgkfb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2czawbnsk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2juldewoc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2iexyabpb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2obhrqqsc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gqlmpxef.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mnfiugbo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2irgmppde.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jmokxprc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fnzgoejw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vjgbrqzy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2rqcywyin.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2otgetxgs.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2bcerrevm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ihxutkpy.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2stelqyqd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rgyekjul.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wanrdicz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2obnunkov.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wybbzvwh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cqyykghj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2mqhrbgbq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2zwskmnnv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vsyguwjw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2joebgpjr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2csbcpuno.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2uepwtwtg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2amtfgeiq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ppzdxdah.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oghvnldg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2cazwhwdz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2nopnvpbk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2frhkluot.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2xoekjvlz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jdeupbqv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2gltadjbd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2vsgoovfg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2yofcrydf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2dfhmasxg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fuoutfam.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yjfdrjrj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2bfqcvnno.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rnlzlykj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2vvxltxiv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vipqfpwx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xhiufwer.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wtxgoclt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2xqisvacu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2kzhgqdjd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qjatsrbz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ozxmwmjj.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2qrksbrch.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2uuehyohw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2sdbrikfp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2bmwhzlso.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nzygqpzd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xhiyszfn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nvottsij.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hdpiymwa.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2fydamdih.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2arrjibpl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2xdvquuqs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ityfbyuc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xtliscmx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2prrrrvjq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2sgymljoy.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aczrjpkh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2xzfqfwzq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2uyjziklj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2htflnqnq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2lzanlabn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2zkkpwwsr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pnvsmwnp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uhnmefor.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2vmtevdan.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2adpbkhoq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2hthakyqs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ojjwnuol.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2bylepajv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2qaynvxvv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fhjudwkt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ofkunnqq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pcfdshln.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2nmqhroon.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mamuqbsj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pmubvmzk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xqqjnwwz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2arnhdpmo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hsjiajdj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hgxddnhe.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2eozlabft.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hgnfcmff.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2qmhdkiwp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2drigiese.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2rlbpopgi.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yigqneym.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ykcqsgqp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zpocbnaj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2thusovmy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xsyrledb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2yowghbwn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2xnstuwue.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2tcwsvjgo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2aeztwpnh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2inymccrw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zfjxvybr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gtkoibwr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2fslpgtbv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2kmkoyzyl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2drtfanhn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jmewpqya.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vmcpcoun.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2pacrmfbq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ujmnanlt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2xjigyywv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2gjobccgj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2lkxpwqhm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zyofobfl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2unwpvacu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zyaychfg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rykcdgwj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2mwrirhgh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uyndpies.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2dzgsxgsi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2qdtcbnyb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vdzkrvku.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2rnppclgg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wdyfrwrx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2bpkjlsrn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2gaelmhuj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2zktftdvn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2wvzjemsd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2csdnaxqt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2paxshchc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2mgxooinl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ivluldzw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vkubljjh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2zlmbrrfw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2oqlvfrhx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2fddopeid.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2rtdzmwbt.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2rbyfachz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cvdefzql.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2mxsdjaaq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vpfbpzbb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sapyrnjd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2iozrfujc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gvvhvavo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2oswiizlv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nmlkzane.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2tirimigf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2eyiphxet.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2tiqksxpw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2oajvrwtw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2aegnbuel.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2hfkicgac.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2nrtwwqsw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2eqwwzcge.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ncgfqngz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2fkozqptb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vzsswhhs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kqppalyy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wuczicsa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mphqqwfz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2debjysta.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mqesqjba.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2sdbdpbzw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2zyaxgzvk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2mwxijxuz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2wigbognr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ibjorvcs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2snvrezhd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2utsiceli.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2urntskzo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ngrihhyg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2usexbreo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ebwjfwyc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2xhmtqsxx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ipinvtsx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2thhlbxvu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2toqlbhat.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2txxmipvc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2nfpmvyry.html


<!-- 参考信息 -->