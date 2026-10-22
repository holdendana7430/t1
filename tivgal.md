代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2nzjsddyx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2seqmzpdb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2uccsngeb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2rhdwlzgx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2khdfsdfb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2dpyknyps.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2djhuaqhh.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2sencppua.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2vsxwkbef.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tgcabymo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ywgqkbku.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qekumzpy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2mhdmzxxa.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2inphosai.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cpnzefou.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2rbfropil.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2xifuwfnr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwcifqlw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2vsjfbnfp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lxfynuyq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jukqiysw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2wahcpfca.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2raxmkzde.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2rnvccssg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2rlkalfxo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2jqnvyzaf.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vjpfsvhy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oxdwtwov.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohjkjbcb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehkbamar.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2eqtpnayt.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ivfrdgwu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2dmdpdabm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2fsjsfnud.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2dulviklk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2qdaoocfk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nrwtbvnp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnmomgql.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2piijhsyz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ihritsbz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2vghkyelu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vofapfec.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2dwcrlwev.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2whgsgsso.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2yghplhvt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2pvqxkwpz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2tmahmoqx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2riflzovn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2bcjhztlg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2kycajkbz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjwcdfyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rienztpl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2qhwfoxiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkelppga.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pvttdzmz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hbivalwl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iekixcwk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wvnkkjse.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2kaarnjap.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wpnhbsgj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2nexhvqgf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2pbunbjji.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2zfqthbst.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2yzlzluzo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ekgvtvup.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ynnzorni.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tzexowrs.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2knggayse.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2yjylzhvj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2xvzfwixq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2jlhdwqzd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ppslnrxe.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xzmbvyyn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wmeniqci.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2hlpixqvu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qxnqrfxj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2micddlcg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lmydsygo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gbxquqzv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2anjxanwz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2svhzfoxs.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zmgaxmcm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2innznduf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qpcdwsvh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2gqxbnbtz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hdgoofoe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wqemmbyz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2sjcsmpjl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2oenzoxfk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2huoiwxmr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vvudermg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qqmbcdua.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oowrasat.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kevsknad.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hftnlsbw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2cfefojbx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2caihvkmo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2crrbnxgj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lbmwnhgm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2evqitbjy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cnwvsyhj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2aynwzvci.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vcobuqaq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ujnxcshp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2dovmfekq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2prgfxhng.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ngtqdkur.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2juxmemwv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2wmzzhogn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2sdnfeomh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wjfhszbz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tlshopoj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2slkfmgal.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pvkdrphm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2egxwgbpc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2eenulvpj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rttfccfw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2rikmumhs.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qagokron.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2mhxixcny.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2smkqtfxc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2hrrnnccn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2aikirhuq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2wsfuczsv.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ybjuariu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pjzmupjs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2vvanglmz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hcnelclg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2skvnqpnz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jiltooad.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2dtnucxtp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2zmjprzjw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qejcarjk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kulwfrws.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ipzvgkfy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2xokwvhvu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2olzdohsh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qtqfghuc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qwqztxpa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2arpmazrd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2kzknagct.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2yoyncdsp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2cgxteglm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2wbsormak.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mzfmrvua.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xigcxate.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jnqpvqtd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2gyaeefyi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2gfpoifnc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ajblwofj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2wsjbdmjw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2dhupmkha.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ouneyyuz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2tokbjlsz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bhdiesxe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2znfkknqp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kjamzvkl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ifhysoou.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xeqzczgd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2islomaff.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2hnqtwwmb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2hmjsxdfg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ogatuomr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hexhdusf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2vbtvncoe.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2clhpyasl.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fgywbraa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ukketozr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2begmuemm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2saowcqee.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bbqmgxmw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2xccxcczd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2cgjpfpdd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aiyvzqyg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vpnjmanq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dwbhbtcw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sjkhicjn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bubgjxly.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qtosexpx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tjgtqhzs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rztkouxk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wjupswih.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jpbesvun.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gqoxtyey.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wdwfpbmq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2blfxokrl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2aygdvlpf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2mtccujjh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2zdzrjmoc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2bffpmbmp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hxkkouov.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qmuevire.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cnxlqtvp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vxeckdyd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2girolyop.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hwoiabxw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2poudrkmg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ioommqen.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ggwtgsua.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vaddgzph.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ccovhlpp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2rjwvjrmj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yxsgnrek.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dyeinyox.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2lytnpcdd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2pqooayui.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2pxseujga.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2lwoziyxp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2bhxrmbub.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2zfmmaadw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2fjhqnjzi.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2badzqfpw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2tyihfdmh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bbmcduhy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2rouovjuf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vtjuxnfo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2kgkpxmsj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ccosqjkc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2imbctkrb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2zbhrwftj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lucjudkw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2wbxlaocc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2hinkbgoo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2kwfnjqvj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2eicuqsvj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2fzalfmtx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xaaykssg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fbuxiciq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2yjqubfnw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tshfniqg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2zlzobqtv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2cefgpvmm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2rxeezbzs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2hzlufpyb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2abkjyniq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ezqbhdpt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2twjensyh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dacmrpqq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fdrwgncs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kimnsmik.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mauwpvae.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iiachnpi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2frajdile.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2gogyjypn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2satjeuwo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ozorvgfv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2nndegywg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2norkplve.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vjyndmpo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rceuiqaf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2zglkbgdt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sunowchu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2umdynoyu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2yrnhjipp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2hstkppbh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qnjienzf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vboqsjhn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2idupnuib.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2evwkjoft.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2txxrzdcc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2oazpdyqq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2qssudkuc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2rvzvpaxo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2kfglcexv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sukfopqm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fynvtuzh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uedostka.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ozlqcnje.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sitxkmae.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2sdmiaycv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hzozxgvr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2jkjnroqw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2iagsejeg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2bmligrni.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ertdxflh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ujkrsquw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2jonybxsg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2wtelcete.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xsejtvnb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2brvnrhar.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yiekfsvs.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rabkrsfw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2drisnrvr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tbukohuz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xmlmdodv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2usxucegr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sfjfwzxa.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mlckqxww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktxpetlu.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2flmdmgln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhfesoqf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kvfsclyb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2yimvqkjo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2vgmmkkdx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lxndslkf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zytwehia.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2htposdkd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2chcumjii.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2bwsdyffw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qeqkubfs.html


<!-- 参考信息 -->