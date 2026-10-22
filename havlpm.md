代发 wailian999

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2doljhvjx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xfarxkmm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2eshcpkda.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2wwfdfduk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fleidaqn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ulrknnrg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2qfsdpmtv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2sksuthxf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2tvwmszlb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2hbjpdlys.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2dlkgxbbx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2fqksgnro.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2mnhrslon.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2sspajpfb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kcgwepuq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2mzdfjnad.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2qhdaokdu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2gyrrjcmr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ozdtkfsf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2fbsirvmg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hsbroepy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2opbogcyb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2nooykwyp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2amhsmmdt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2whrhsiei.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2yxodcvux.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2cyyzqctv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2tioewhhg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2rigwbdku.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2tbknsmtr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nrxqyapx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2aemokvxg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2epxxpvjf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mevnywys.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2yjsjwhbs.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lzsyqskx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qlaumicv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2rfinwiwa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kkedqdam.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2hwjzwuxj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2seewwdzr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmghgswd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wwlhrlgg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ndsvwrns.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2enhfckrz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2tlurevpf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ezmxjfnd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2lnpiggzv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2lmxuxdnv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2dajeztlf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zgdolnci.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hsykhncn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rtqmcuel.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hxgftrsq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ccqipour.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxbniqgu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2dzkdtxop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtdbzaga.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2efsyfuyl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2urvdrbgp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ekuvbjes.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2arykcxvo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2iupmmoql.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ctbxoyiz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ghtilifw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ajsgpkjb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2zonjouby.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2bcoxkmqy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2iuuonhed.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2inzgxxyv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dbiarezt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uvywbngr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2igczmsse.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2denkiepu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2abzkfnjj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2usjvhtoa.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qukpgoiy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nwrvbgli.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2eqllcmlf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2axsojexw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2imutkaci.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gushucxn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2oshzeqrc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2fsddizkb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kxkpfdwo.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2trsdsxai.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vslmmfwv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kcfmkfyo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2sepxucgr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2fzazztss.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nessztno.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ueplzrfn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2hjkumbgg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2entkhina.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ktrhlmqb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tkvvqdmi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xixynqrr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mdaonmkc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2pculedfj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2xzejjknp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2adfjbhvk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2acyoovau.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wkjjdwys.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cxlrbthm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2anxtcpua.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aaijvawg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bdgslwny.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ctervvkb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2fgvsjjbk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ohuslcws.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2tqpwjjfh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ogrjlugm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2vbzqanak.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qyxupich.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vtnnyrma.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2eqrnktef.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kqmrcqdf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tlbuvanh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2jjlkxuzl.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2pyiruhxf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2axrzixlz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ttlkqprx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hcjjwjdz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2zcmgnhhh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2uvtucaul.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2kmuearwf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kqzedgxk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2pvqxphrw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2suasgbcj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fmxyfbyn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2kfsesccr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vvqsrqsv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xndvuzoi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2bqucoovq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2wtvqroxq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2xsvlmuqt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ygqzwbut.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kboqqdgo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2cgentvxv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2nskhvtgl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2viqhxonx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ksqerexx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2egsvhxez.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cjgeakry.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2dyzxnkuk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vfhkfygd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2snfhxmvj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2nztaosmo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2msqguqrc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ljpajlpy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2adoveorf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ilzafmyo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2dqowfxkt.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2qaxoqkwp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2gnibqpbx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bncynblk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jlmanhyw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2znvkqkkz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2yljtsxft.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2abjzqogh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2facjktkz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bsjtofqz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2uhoplshx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2enpswgpr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jdugitgt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2hbnfxwpp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2mzagrmub.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2fxxrzhyg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2tzswzolt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vcfihaie.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mfuhjzto.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2miflewvy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2lkqqzzxw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2esnqiuol.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vzgjqyyz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2caoqhzvg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2airwnoqc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lbtvvvcz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nlpdzdqe.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ukdsrvav.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2prrxvxmo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2fbhquvoo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dyyfyziq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2urbukdfm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2abfixwvm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2znhaqceq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2covrrsil.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ovygyomt.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2csivehxi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2mptbxgfa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2eadltqyx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hkithxuu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xfnvgtlw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2otsgryjt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jjludtca.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ekxtkuws.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xehhcddu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2elingjjw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2lnkfonyy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ljfldekd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kqhmdvgg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2yerkzbfc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vxkwtolz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xjstyfsq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2smxrrjrs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ymppljvq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2oiuerthn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2virdrjoq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zecaagwz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2piwrkwty.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xhoempjw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2avkxpwcj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zuscvxyq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ikyrzbjq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2uetmpmip.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2boxgxadx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2kysqbtsh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yxrjxsfj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2wukquxru.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mmwmlvyb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ozwntzji.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jvchxcgc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2kyifwpda.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2gbklmviz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pyplmawd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2zpuhqodj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2oquchjhu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2jypyvxoo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2sadeuium.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2myukkdzn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vvnsugxa.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2kqgreirf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fhdintfg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zuhfiuol.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2hljoslbb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rsfcbszu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ogwidcai.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2pjifjwur.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2oqwoptvt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2uxuavlck.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2biescaqw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pllddond.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hmosdyca.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fefbmcpl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wlwxrjxc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cugfjdhh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rjemskvd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2armnstge.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2agbaujut.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2mseludkt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2pqwgqkdx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2kygrvwfn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ptsifqpg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rnswjtqy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2mkvmndun.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2tsvjjofe.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2pejixmxg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2hndehvly.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fapkbodq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yvykhhkp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zbbmeqsb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2vjxkjyhv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tumatjrr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2zffrljpi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ayodvyuq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2iudpkggj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2bjglwoao.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xhhvgclm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2axykedsi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2odwqwkgw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yqxhhgxn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2aokmphnv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2uezodjxq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2sqwqfqnj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ecncrbjn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ftbaxlro.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2fkaoiniy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qyvftxvk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2rggefurq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lrawvycc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2nohdypde.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xuyoelkp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zljycvpd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2yezaadwo.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2nqdpmaci.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eplpzxvh.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nbkkxazz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2okbnvvtt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hiuemvjc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mplswnge.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2htlgsmjz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2odrqcwiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phcbuvog.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2rsstxkvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dyyzuidi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2swrnuhht.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2hneyserc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2heztkwmg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2syyecbwk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yxrjevsk.html


<!-- 参考信息 -->