代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3meecegkr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ynnjpbkv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qfkinqfy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3lxpptfuy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3esfeywvc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ouxdijct.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3liptvpyj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3qxttsbzi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3sujibeaq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bocccftx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ldysalno.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wxykklba.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3eqtycxda.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3eigukvlz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qoxtghtk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jnxltxyd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3uzarghvg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hsmirthv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3nazaxgtj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhkradaf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kxrhvqum.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3wgtmfgvo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wlqpourj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3eyqfzozm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3shhmlbzd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3shuwwlnj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ylyiuyhc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qgobyidw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3okslsmte.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzxxxmox.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3uiguwpdc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3erfdyzwk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3avimloev.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3kzgcxdua.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xmlmgldp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xwxtkshc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3aqeydlfw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qpyfubbv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3chfrlnxc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jrxutawy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3dwbbihsv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3dgsfaksy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3xmwjxjdd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mskucair.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qhdmhtkb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3iushoxpz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3iwwykybs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3sowdxnau.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3uuihgtts.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3amoywzlq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sanwcpgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xtapoyop.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3srbfimie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ucjzmdwc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3itmbvgun.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3dvefthat.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vyhtiotu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zpfrbwso.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3spwkyqyq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3aptsjltb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3plmrdndb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3dxfjxjkm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3crjimpvk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ydefjjwi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3mifwfvhb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ouagrwxa.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hxisehbn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uantedxb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3zbgwzbok.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3foscbgeo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3yenvwcky.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qbejiaba.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3xdhakorq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xtkxwdoc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ehjvbrhe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3lreraxzl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hzpiqnqt.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wvznntjj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hvbzktbp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3iekmbikx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3heufebey.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kgacuaxr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cxgyyqia.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xplszwnd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3xtbpbkso.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vmctyzyf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3rfdblold.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3bxjvqncs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3azxanudi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3qiabufeg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3qesmpbqt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jvfvdvwg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jwgwytuf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gyvbwdce.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ubetkvme.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3cxctgubo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ghxdeavc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3uvzzlgzb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xqrddtwu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xtuorgpy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rtngqwpn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vwpksxlk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dwnugtoo.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dlqmohet.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3iuctcrof.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fkwstpfi.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3bfzdamwg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hwbipemy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ojfepwav.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3wpfemxxm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tnvdwppm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qtoznfnd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yeilswic.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wcmjojrc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3kapmxwts.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nenjtbua.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3aqxcukbu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3klocxael.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vvmcpcpe.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3tdrsqgss.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3alhxscdc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3aldilhwu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3rjrizmfg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3puainjow.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ohzjvygg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ikzuvbka.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3palkmerj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oiscrdfo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vjnvdhcg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3tvubrczs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3hfmbcqqp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ngyqnwqo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lxnffrpb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3spgbtrxq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3qkyiqysy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3jsrfldup.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3aesvsaun.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3chneqetf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pntuqwqr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3yeibzseg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3xmzvetqq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3lnvdpuso.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3lymjuckd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qfftyjcn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3rbhegsul.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3sgzqszzt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cruyugmb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3sbnbjaqj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3crjpizfy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3spqtpoxw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mfxzdstf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3svycrjns.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3becfzxmu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3gdmdgqqt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3zyohydnc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dvyuhnxu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vutkwzhs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nbxvtdgf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3qixlytgg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fscnmtsd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3npmjvcbw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ljjiajbp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3yqynssbt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zqqwewsr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xrcgavek.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zqbfsbef.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jybsclpz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mkonxppf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3qhvafbxx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ivihhcgt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hyrzgget.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3solixhvj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3oypwindj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cpljqvvv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3esinmxbf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mwcbzrja.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rbijronm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3caubbjlv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3iarfhjed.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ummoiace.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3vzlkmfun.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3emrmbtnj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3gbrjlijt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kkrmmabx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nrpitoum.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3mmctaymn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3aqdzibdc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3sqyodkdm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eglazqzk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3lggkzvke.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zwtwmoik.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ogbrowdr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dmpkuxba.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rbzyfqgr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3dvrxdbqw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3wmzwbhny.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3otphyxhi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3rfsvcedv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ioigfuer.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3akwwwzfk.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3extjryto.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3heitxqje.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qcocmzom.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3mpeafixo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gbjhfcwo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3rzzqeotn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3pxaxyyhx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3gbbheclj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3bjipupzx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3kkzfxdgu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3nphoelrx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3dmvuhfui.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3edidnixk.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dmefdcxs.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3jwdhirsl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bzefxgll.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ditauvyt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3izxdunez.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qvqeusfy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3upnuzakj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jjmdwplz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3asoztwli.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3wtnlcqmb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3edmogicm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3lxymyeep.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3keggxcuw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nlzxbvdh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3nckaaclr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kgshbyur.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jpgtnoiw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3auzzsyai.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3eibnsokd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3wrxvlrma.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zeauhosd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3sjkoqvky.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3iciqnnbm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3pphftkzb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uyvmdqgv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3obaqubma.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mfkirfuz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kaxryfta.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ifitbtpw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pjiorooh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3gqhjhrhy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ycrxzohq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qiubaydz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tfzrsivr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jjyohkbn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3gzyyldyk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3znavjwhw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3oycvcroj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3evatbnul.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3uswwophb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zthlufar.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sizhynle.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3sovwmvza.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3huymjufh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3qoodvltn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yjoypigr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ryiwflpr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zkjjwvji.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3zldcbegg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rkmtitkw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jzdftirv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3agyamtpg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3coyrksyt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zrzogcvp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3bynysrwy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3njgnesii.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3sdpdwtna.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3hjftoqss.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3yoyrorvt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3adrzszaf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ydwiimqb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3hunccnhm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xtabwfjx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3twcilxtm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tndnqcow.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3npzvuxql.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3xhvjsvmw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3baxbszlo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tnbietqf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3eajnibji.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bsphnhbh.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cydqmkbr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3aummfuih.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uuvlhtpu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3edvewfwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ritfcbtm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3wvenarzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwmjjlsi.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cptyzruc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3okjqnrnr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3srcdgwfp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3roypucwo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uhchmrkb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3kqwfnqvz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3herulbpk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3fxktketc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rigzoegx.html


<!-- 参考信息 -->