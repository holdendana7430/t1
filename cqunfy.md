代发 wailian999

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rfalmmac.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3uxykzrur.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3zxkervaj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3biikchym.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3pfervngv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bbxacmnn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kckrqfrl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3wbraxnsn.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mikwqwgw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3gdfvhdmm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3sotgrfmh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3bwvauqdw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dmzcsgbl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3djkyflof.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3mgorsohx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3dwhwgvim.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3nefxcdch.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3cgbktrfr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3vazcddbp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3fguqrjrx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3dizglfqs.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zsyhxber.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3emfstvdb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3qviejwva.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3lauhptho.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3egjkixxc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3famhelcy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3pgyyldam.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3iujujvaj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoenoxon.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ipaoxwdu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wptnrpnh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtbowwze.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fxqedobp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3piepawcc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fzgpywvy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gtrxsoky.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3tzwwwdvi.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gxqjxcdt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jnydwimu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3igfvkaag.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbzgeloc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3edmxlklt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ytsuqknb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3habbnzgx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ejqyrzgr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3hvthhupz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3hwsnqhhx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ylqhfyny.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwieckcr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xujhccua.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3isruvyvg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3xmgvtmis.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3lyuhmemm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3jsvggfjr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rjatusjh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3yapfkeex.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3tguyarnm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ukkuthxx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3gzscngwu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ulhtwkcx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ccwkvyri.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3glbazquz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhfspfsa.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3upwozwor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrwmykye.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fuxvymts.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3suicwmmh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bvwoxnir.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qvbnbqne.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3owqqrwes.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3bgxtzbuh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3hezfsnnc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3qayscsvt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3dclbgoxf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3qcxqbela.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3fysdesuj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3kugrhvcu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jrbgbclq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3purrbfnz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jzmzboyd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qlfygjsm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3owntiubm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3reqnhhdl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3pxokntqc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pswrcpnz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3mtpwgvbp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3dcknagyy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jrsmgtvb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jqpxzzqz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3yvqmabks.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fvzosplc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fcbtoyhj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3esfzpsrs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3eujebohw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vcpoftfg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3sdezbbvs.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xstnatet.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vdczpywm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ymckrkeu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dthohqxq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ohonaddi.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ividedqf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mcumikre.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hzkaavst.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3slgcqgbd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3yszlwgrl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3nduulqmx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3arexiodu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jswzxpcr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3npdazsfg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tzixabme.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fuospcam.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3udvufwdv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hgjkzjud.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ynhwqxdu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ayqoobev.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oypzqpdv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bxxpwhob.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3wkebgafe.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3izoymqbn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vizqqywc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ebtlcwlo.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bjcdeaeo.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nvqnxccs.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wmubkbhr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3nksktvyz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zykwjwsb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vvwqlmmh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wtjfapnw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3txkjnolz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hpficwvc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ezlgevxn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hgalwicr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3rceysxqn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3gtduqnnp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3yrxmziti.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cfufwujn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3rlwxlwvz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pgbmabhu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3durjjxad.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3gjqohzlo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3nbwtbojm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rxlugbzv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3aubzgklc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ihpvwaqi.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jrudivir.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3fkqpoznq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3obepmesl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3aeuvbhcr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vvgkfpvj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rzqhmmqu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3yzusjrop.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3kryuvihc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3hvofspwe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ktvfbzek.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3nuouaufk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3njfohzbz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3zxfbhbey.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3wuvtyebc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3likfkqqb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3rxagmscw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xiczthfp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ebnqazxi.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xuzmxten.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3czchgzkl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ktqpoeyd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wrrhulyd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3izmstxhv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hhocwjnh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3gwcpbkdq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3emdmkxdm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ftjadtlp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3lfvkmrna.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3asbogivu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nlpivsib.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yfppgqix.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3joncbhqw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ebpuqcwp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kqgrsquh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3omrblfml.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xjskkiju.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zkwjfive.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3gkxhdizz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3wyphpvab.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3avtmetjf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pksnbilp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ydbntvwz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3uqerzaxm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3iqekszzp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3znoujeri.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3shzgmsah.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3cyrdhlso.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3bnzcwpqg.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gdimtyet.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nouawlxa.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bufhblqd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3nmsjuvxj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3cyvpxcrk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3lfssxaov.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ejfboeln.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3moynmflt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hatgckpy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3iodemdxd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gifilsvl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zkikgdht.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3brdjxxvy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3gaehhnbf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jffnwete.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ahzhfdgz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3owrbtucp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cdwkzhnn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3otonaixu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3czaclgji.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3snsfrxcs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xjbukwby.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ehzugeit.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3lmnlfksg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3poinhatx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qysgapgk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3akjoxlsv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3goxsngyz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3jxdcrige.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ytgjyvnt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3rtsohiec.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mbilkatq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3trnhdaut.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3udgbnprs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3kikscxlk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwwxgrtw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3noifbtuv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3pcmalovz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vfczoabl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3pyhhjcdc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3adpikdxk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3bjeiholh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fckzdoub.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3npmqgqlc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rwpybfyy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wuseqfyx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3szvuezns.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3infihzfp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3rcdpqhey.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3dunwslys.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3zbqdnllt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3maflgenq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ndmeekzc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3edlhftid.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bjzfmgkv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wemkscxi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3unfgjajl.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dadfybpa.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3awtjsbmn.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3spiwrdrk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sniepiex.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3pzdwrulq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lyldqwkg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3svdfdfzw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3vdbhmpps.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3librxctn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3jbuglpqc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3lgybjpvp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3bhwzllnn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3jdthhsym.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3mpkketxf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hvoenadw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fftiqixx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3aiaccobp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uxhsucka.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3iffhpmqn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3tgmbosxj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3lakkmnqn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3byvkottf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3crtpmidc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3dmgfdmzl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cieuipxe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zilgnkev.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nfpcksrl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3wgucufsg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jkypynof.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3tmbudcdu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3iunnsugx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3qitbuzvy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ehmlkkog.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hmyiuayw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3rwroxjib.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ivaphfja.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mbeexhur.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3msatykpi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3odobgorl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nrtipdqn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fyljgziu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zzdajdzc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bzgbdlxf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fytqqolr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ljicpykr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tfdztuid.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ylwicctf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ycnionxo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ayohyasr.html


<!-- 参考信息 -->