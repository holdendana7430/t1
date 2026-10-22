代发 wailian999

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2zslcvgsl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2rchvhswu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2qcgcbgxw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lejqwvgh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yxfhbont.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2isfeafyi.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wqrkaeqs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2oxifxopz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tkdcoeqo.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2wrlabxpq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2wynydmzg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2lehqgiza.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ftvqzuls.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2mgmxfkhl.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2rnwhmqaf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2dnqpvmkj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2xplvhmdr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2glppjizh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jyttpfch.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2icpvlxkv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2peuynwud.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bverxivr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gbuojcun.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2asppqyyz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2cnvwybps.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2omefykbt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gdnawylk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2atszhnxa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xfqahywh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mycmuwwh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wktkjkae.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmxjsvki.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxwmkjai.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2sefvcgox.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2gkqjrdkx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2larsgdxg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2vxydycrv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2mztquxki.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fobduxvc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2scmemtzh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ykvssdxi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2axfpozhs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2cgukopsi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2envetfdg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2dtxgcrzb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2aguyaetv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2rjlnvjzf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ddvvcazl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ljkpfqlb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2edzmzdnm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ciqsqubk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vcfgalls.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qoxwzpta.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xisifohl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2sikznikm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2biagcejv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2nhanmuvm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ljthdjon.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2teuygurw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2onxcnwxw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2uwzmxzzb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zscmatbh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2hunzymnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvciffil.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2iswgsknd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2inrylssc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zlcrutub.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2dgyazqhe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zejsjnlz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gxwwoiyc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2cuxpohxj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ullxxlfg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2umrbpskf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hbfhmpxi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2qrnjhlhy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2xmmlpkim.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ybpvwgwz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2diyfkglv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wnqcqjvc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cprihpkt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vypfxnlk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vpfcyoha.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2lihabrcq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2akzligss.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2peztxxln.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2anzelcad.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xorrnres.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2fouavawk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2queahios.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mdakbejq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2slblqkkc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2sbwoprfr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zrmvjktp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2yizoeous.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2auznywow.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zojukwlz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2glmndjrq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2crnhxkfo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2eprhtcky.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2dijqqwwl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ldsnwvmz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2cdzjzbhe.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qpkejtat.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2goljmbsf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bneoanva.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rlureqth.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2huupjugb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ufgjdzua.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ocexjpyb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wtsxvbhh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2catixauy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qzlwkqqp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2repiurbj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2abckjgmh.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hvuouctf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hxaovgri.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zbgngfxo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vwuwuypm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mjmrtqko.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2sibkskqk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2nsyemfnz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2kgxfypqz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cosnyzaa.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lmdigdgh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zmeislgb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sqgcpsrv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2upgbklhm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ykzvbgzq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2igbcbiyi.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2qwewbbyx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lnwdnltg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2amcgpotz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2rkhwsyky.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2wpqcqudq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kxgvhxgv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2xbacccce.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mpouywlj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xnjjljde.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ebrtllmq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2byuhbqsw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hadyjmjq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2vbaizkcv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2azgdpmiu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2skwymbrm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bxyyuvmr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2txworzrg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2tiipcnos.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2phqobzwd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2yxwwchss.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2thdexaex.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vjxbvdss.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xigqsaxd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2bjtfsudu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ognidqxq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2behafibf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ayzffkuf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2iyoeaybz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2lnhfsgab.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2pkrdgzze.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2sqercmdu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2hwssavth.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xufutxtc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xiuwivvo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iniykcbf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hsurmqdx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2oeounair.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mscvfayk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2eprehxsn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nluumaog.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dvlpyumm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2dgincqcn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lzfgvvfc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lfyqhqgq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2luzgdwzh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2pqjnicok.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vdvgkfec.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2siutkckl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xijcmtfz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zhhfxebd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2syntkkix.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2zrsazkyq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2nchtkqkb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jweksrif.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2zqafrmtd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2sidwkegy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lsjpvwix.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ecazfusp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2drgtaiya.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2yabrgvtm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mvuppigo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uqtlsheq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2prwqgfjm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2oxpkgbkc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ymdfasyn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mywxslnx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ajepvuzw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2irnmurog.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2aextuuid.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2gympzkbh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hypcobek.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2axjpqimq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2kjxbqfrj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jtnauiel.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wnmobmrv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2agmsjgxh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xhjjcrnv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ggqrwadt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ebunilus.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2lvetgmmx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2wlnxbcgg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2mxhytpfq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ganzhizz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2pgdugapz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vozhvawn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2njjcvguv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aemvrsym.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2avrtrerq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2davfnwlo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ibeuwijx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2fhyonlcr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2tbmpzwrh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2dhxwoujj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mdwcgsyx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2oolfoafc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2wosvrfxi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ewkoelud.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2miunlync.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2abpiijia.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fsehyfup.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2rhwuzsrf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2fdsqpgeh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2qvzwarro.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zdswquim.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2incskcqn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wyjsrgwo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2xsrgkfia.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2bjqyjrnf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rhtrhxjh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ofqptefy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2evbeybmo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kbevauvs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2yncgmgut.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2nzahkuub.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2reqvhwry.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2vqobyzjy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2wwloruhv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ctbkmwej.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2dhafnjya.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mvfllobn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ojkljssm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ftnfqkel.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xohhtqkb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zofxtpks.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2olhoucdp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zvvbwetm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2vspjforj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2adqpcfob.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2axgaorta.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2oeydkart.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2miduzept.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ikksepmt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2sxedcrqc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2punoldda.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rudwynhr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2pnrfqusi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tfkuehhh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vnsxzslg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2agufxcrk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aczdjous.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2zrqnpjbx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nzpukvuw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ueeichms.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2inmfgqif.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2movebxgq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2okmrjpzl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2hwvyvevk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdxeahai.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sjidtvqo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pjmqenvw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2krzwebej.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2otfupmca.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2oftnclcw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ojxkrqdf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2inseriit.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lhurfntk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pkensccy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2evgnoysf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjqukpzh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2pntiwagh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2rtgrgyny.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2eaizpdrl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2holauaoc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hebescvz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fzyxykxa.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hhmqdhmp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ctamskgi.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xrxtayqt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2unzzwysc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zxkjlqot.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2cbptxkld.html


<!-- 参考信息 -->