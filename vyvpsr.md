代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2pzegoklw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2foxoacbk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvcqmhuw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2jiacsrli.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rgdneieo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2oziuqoch.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zeaezxnp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kfusyznj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2podtnwmx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2vcugvziq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ullvovhx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2wgyercrt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ddndzbtl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2mdypfqdv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2tkwipbiu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2garfsoif.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2vwegexxo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ekquofvr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hljjxqss.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2josdydoj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lztfvarn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2hczwnhio.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2synycebh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2vgshakur.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tuszjsqp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2gmgcamop.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2cibxoaxa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ugwdhrpr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2dzykmazu.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2xybgzuly.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2fojxcsmu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2czrmanly.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2rokzdqlv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hwlhutpt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lcbomfeh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2yqftmeds.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2enfxsbrs.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2wvekcdeu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gtqdhtra.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2rnnkpnfd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bjwoekyu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uroofvpj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2trhxyljt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtmosufu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ubfenhxn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2zoeqpecr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2vowreagx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2nhzetzjc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2tqhovgpr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2vxoicxvn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fwyifvwj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pphcwdvc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rbjbnmyn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvwsjauw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2wvvamsxe.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fsyoepko.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2jzpwzdtx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2jbpsykbn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ejneqznu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2olsyedlj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwmtfpbs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oijcudbz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2upexrpmk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lsmmlglr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2iuxrzqlk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nmdptidc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2jwfzxuse.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2yoncpwmg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2vfijmrkd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2znmarfwo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hlosjmnh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfnehxui.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ldqzhjgx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2yuxuoghu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuhckovi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipikdcrj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ezaxiduj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvtyqlpt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ocztzfak.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2qarrsleo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fmlhwvfa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xwhycerx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ukobtoiv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ejonhaen.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2jdsjlyxs.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hjzcours.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2szvmeoti.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2uewmwicm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2yxrolixi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nnqocpkn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jfkioyek.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2sgymxckp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tfavpoff.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cpkcntyi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2shcdmczt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2xtbwvtmo.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2plkvjumz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qvnmtuxj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2hautysxl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2krxpviox.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2unuhhdjm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qejzpcqo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2yjhyugmz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2rqemhjrb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hpcohgwq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2idzpdnoi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zttnpxar.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ltexnuhv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2gnbgxoje.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hrmtsfdp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cefvmykx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2sqianbdm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2bnpoaefl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2crgmcgpl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2cbxpbmqw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hcivuhur.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fzbtlsvp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vswfkmce.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ggfelxvt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2xuxbcxmv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kphaehel.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2atdulqqr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jtkwxogz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jrbwprlw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2iaaihwbx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vwmsiyco.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xbcrjvha.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vlxaaylp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2kyrjngaw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kpjtiuqv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2lthlrbzj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2lburxiym.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ssmrdadl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wfngnlph.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fmbpajuw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2oalxhafa.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nfxrcbzx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lobijgxk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qtzqkxvm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2mfvbyewv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zizupmcl.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2kwoctztj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iixpablw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2zelqihvu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2dkeldnvi.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ilacdxkg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ipoqkmao.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2kfkcxtdq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2lbcouewo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ttzpdrin.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2vnmlfmkt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hueexdss.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qonqranx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2stwlqywv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2vxklubad.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2hwjgmrif.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2uuelikuq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2msilaaow.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ddapdmbu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vupcsgsa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2meaqxmpu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2evlrfvuz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2eccjhxyk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vdqczqmi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2cyigxvho.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ylnhahui.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ncvbnsdh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2pfrvmwja.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ucthxgoh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2wqynumao.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2wbfumtkg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2dcewcnqt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2pobooxbe.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2pmghvops.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yulwafop.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gdcrjcqy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2sxhaafhq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2utqmiaoy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dtvcfddp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gcodrduz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2oeytxsok.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gouvlbzl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2xmjshhtd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vhebqqcn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ggjosuvj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2fhmegwnj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2esrqtihl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rzmolctw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ypvhlyel.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xbrmksvr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jtwxhclf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2mdpvwfvp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2dhggqoui.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2efxlwgff.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sktrkvht.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2nnrswxka.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2pxhbhjob.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qppnboeb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bawpqkem.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iqoclyti.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bzmladha.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vheiykbp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rqhmjwjx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fwuiyhoc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vqbjynbl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cdwuufuu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2guwiuxcc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yvhheefh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ucbgpkcy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2xmrjpcyo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2wyraiwkp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2whbgvund.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yevlrgee.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2gpxhdxsh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ijjuikxb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nuptrcli.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nnvrqkwi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mifumcfo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2lpibcbhd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2gewogkcy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ohfechkj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2zzldtrob.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wziqtuzl.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ztumoykh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2elttfaff.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vtarxnup.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2dwkccjfr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oofzqheb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tjhtlqmo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2xzskbuux.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vqsxtcdh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2qlzobzcl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2wsirgrvi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2rwnagtbu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2afzlwjqe.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2loywqycw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kpkfhlri.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2rmmdsxgd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2umqkxkrr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ifqfsisc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2izogeqiv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2tmxexdod.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2daigwhzg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2aqrlbnls.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2htshdkcd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2zqbboexu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ljpfobqt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2qkejqvax.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ojswtivd.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2erzfjaym.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gerbuvno.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xqxdddjc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2shgoxarh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ldsgkbij.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2pesozbtj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hziajkfk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2fnwvysgr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2lesgaofc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2thtsteol.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2pdaomjyd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2goyvgatn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvwbjwvq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rfagcmph.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gbfusfwp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ziqvmgqh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2berzdohy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tdpsorng.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2zelrdpkg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlgrlbco.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2oooervoo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pasceioh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ybefsrrp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fvkveckg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2eckifkxq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2tbztyjro.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ttrjhcrh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2hnnzjifj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iibnajce.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2sinpsnhf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ueapizog.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xhnlojos.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2qbyykdso.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2buypsedd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2kkcequpk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2rhvwvjpf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2njuzmfgb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2eqyhtofj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fhrhgbeq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fieahyfk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pmrtxqhy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2fygvhrjy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hwqmwemf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2tmijtbwi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2zpbrgjxr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2xwcpujsw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2dfannllh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2cbcnltxs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vnvmefzh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2agsukzhm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ypzirnno.html


<!-- 参考信息 -->