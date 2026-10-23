代发 wailian999

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eozsjqed.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3mftztaiu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3wfnjsbks.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nqgxzeif.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mkpvearm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hqucgsrp.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3lujfvxhj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3tifcvrrb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3auzqkkey.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3grbbcmpd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3vefquzle.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3yqjfmvri.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3hiwlhnby.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3otnfueoh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3azzzwcqc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3freczeme.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3aivwzjpp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3caoajkma.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3twqpfwrj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3xgpbeqcl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ohcvxfva.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vvahfeza.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3wiinsrcu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvqmyibv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3exyxofyc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3kkrjoucc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3cueffgew.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3nzqpimbe.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3pqijfitu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3bbufcmih.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nnjryvsz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ndxtortk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yogkpyhc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynorrcsy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3figvgwqk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bwqfnoth.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bbzoyzai.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3mttlpjuy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3zycgqkns.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zwfbearq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngwrvump.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3higqwolr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dnijhmeg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3aukewput.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ivhrhntw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3txnqkzky.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3hhxavuie.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hhpupmto.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3efwrsjzr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3bauqpaqe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3lcuutocx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ygwumnyc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3zcpiqpxm.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3zfbdjplk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3uspvqihe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3driwkdjm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3yqgarcmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rauhldmp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3abqeohtb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3kjfkfoxx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rgyinllt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mldfkpuh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3xcmeshsg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3kapynnzt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3qyljfgdt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3timbrdec.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3giblckfr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3repnussf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ccncgnqx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pbafhvdl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dszsrmmy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pctluiil.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3mhhusdtu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iniyukxb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3iqxavxdh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ltvkeufn.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3vybssyjq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3altoqqzg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3aprmfnti.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ufwkdcst.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3woufzhfe.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pzmesyui.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3hzdalzmd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3hsmymgbu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mggbvtbq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3yspymyge.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3btxwhwrn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3easswsyl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3rcdqwblg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lrbjcdcq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zmplmzgy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3lovvtraf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3peicnhdi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3fymvfylw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ilpsrown.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qdzrrezj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nhlkkwjy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vwcxfiqy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3nwmafwjp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vsqfuyds.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3amifcegn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dbcnagmw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3trcczppp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3yvestmru.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uxygmjzs.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jdjwrhyx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jvakrdeg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3emzzknnw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3aarbjxxi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3drkmmjar.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3pvdgjdge.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3dvlicxsf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3tdpelftr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3secrrsoc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sgtmfmaz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xbssprrl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hqrqexkw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xuexgxkk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3rzbpgykh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3udtkyyhg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xnfpdmlb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3tgqshndm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3janusgco.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3cqssynka.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3jeadywtd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3grqqsvwj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3zvxhjrwu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3yrhgbgmi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3znylpfcg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3plrkiuth.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mfmwyvnz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cebbddod.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3istefwsm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3wycjnegi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3geqwsmgy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3loeeugcs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fcdsrdze.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xegximau.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3owqfvfyp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qdmzxoyf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3witxljzx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3srenerir.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lgpugbhy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yhvhkwnh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3iiwlvoqg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3lwvorpfa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3tpjjvtnu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ykvekkqy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ylxnmlyg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3koqjrvvb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3opeqjjkr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ekcujiab.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3evytdvny.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oqsxxyyy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zjgkcqme.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3rhegaxib.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3txvbdhbw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rpmeyinc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3faxkwlpk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zeddjmzy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ailrnwwr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3odosclsl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3prcneecs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fartqghf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3avbenxhd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3alagnbqm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3xpttjmbl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3xevosyto.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3onorwqgc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ppaxwdwd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3whgsvnlp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tvtcabmc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ylqidzyw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3czmahfhk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qkvienva.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3unsfvaqt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3uhgfluvy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lyresgun.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ybginmqv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wshzemxh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ozljubbd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bdpweyfb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fsdmeear.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3izzlsstu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3glpgnaqo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3auucdpzv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rxwuajxd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qypjkrod.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zuavwzgc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3fvbrkshr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3rxaqcpru.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3usmxdlhd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cgqnjcrr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3lwnharzd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mrotusqq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ogmfzamg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cddznjtw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jjvocwcl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3buetkuvy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vaaoeidp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kfzgkdsu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3vvibshfg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dqjfrgps.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lrzqbkmg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mcuryzml.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qcaawiau.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dwqsntio.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jjvqhdco.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3yfdzkhid.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kiqornff.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3urucpvab.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rvbtohhq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3jiyleeso.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3inizybun.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3pjulwsfi.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ejtbnrfi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zagykleu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3puvdvznr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3bciobjjg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iwuwywwt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xwnburbj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eobycyjw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3oepgdcrw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3dfmziecn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ommibvxn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3bqnzfjli.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3tzuwmtoa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3dnlflwio.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3wsvpincm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ngccgihv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3byapilfb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3odyabcvt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bmemrasj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qimdouvj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3fdjwdlld.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vizonxle.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3zzfznyqh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3fodjfpkf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zxelnsew.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3jrvghkij.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3omtzaoma.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3knjuhkru.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wrruzxjc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3utyyofhn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bgqhkpkx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jnjdttfm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zfdgcztx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3huvkbfuk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vjpaxsrv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3dhirswyu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3exrkgvao.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xmmvonbb.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ikfoamiq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3bzrnayam.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gdojxlgu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3qsntdxdz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3afvkenam.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3srouvdxk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3whwvjfrj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qjsoebgn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mkgbuypl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3msxphljn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rxonpeyy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3dovmgpik.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3uqrpfhzl.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3lxkcyjga.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3gyxvkcrv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zlccsbbc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3oltqwvrx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bkpqfryj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qzpsvdga.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3gnpelmew.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kxisztqd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3hwqsjjgs.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3nlfxkoft.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3fnoyqcxh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3votxdmug.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xlugewxz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ihwwoitl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3txjkdche.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ozkmfeok.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hbfnhjfq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wjzicwxm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gucntlzd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vztasoxr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zkkvbvtr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qmragxoz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ucijjvck.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wdilfipy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3yyttcpth.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kwvzdlia.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gtzpsvdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aezgvqrl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ekjrnguk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybejxqmc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3oiwnruhu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3vjzqilrx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3gpwenaps.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3yenglile.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3parttyls.html


<!-- 参考信息 -->