代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3doojmzmf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3bvdiaslm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wpzqlmys.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ivpojtrq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3umvdgkwa.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3foaucfaz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3biizvpwo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3clgyehrv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xgbwvbwo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lnbnezlm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ppmotuhn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3vbgvpbkt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ixeiowrh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ybqenetw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ugwzpwnu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3pdfndgah.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3apzarxcw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3loyfnulq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3jfcatchk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpqdluxa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3trsvzasz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3czqmgtgr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ujetguld.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3jlsqtevp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3sgnslpqm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3dugbxsoj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wpjacrza.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qlzzimsf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3buxvhxxi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3txkgkxmv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ssniwmof.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3seouhbiq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3gubkwrbp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3xqbhgojq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3akwtphma.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3hsbujaza.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tumiymzi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3yaicexti.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gptszjfx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nlmaydcn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qpdwkjto.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ceptfurc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3qwtpxezp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3imzzzmzu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3fqmgwzps.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3rimobrbz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3cwienlfe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3gyajhmzx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3bbyeefmk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mhyyrpws.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3skcwlibp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xsewfxkv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bxozkxbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrghlcav.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yetygitd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ccpezuku.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vxlonrgv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vrisxebp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gnmgsbmm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3xlprqaof.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3qlhegkjl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kgeqlayy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lncuigud.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3woxoqppv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qzelpkob.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vxvxhsew.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3byxlnuff.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ydoucrnk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cpkefqqx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dxmfjlos.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hreuszfc.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yeeojqmc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3vcgolugi.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3vamctnex.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3zkcynxiu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3eeulcdqz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wtolubqf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uksadybp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ecstcsaw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3iyyelzye.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uutcqwoz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3faqrldgt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wcgnlftl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fsrxoefp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3eclhrdss.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uepgmyni.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3eqqjtmim.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3diedevwj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3arroqyqn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3govmgtkz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3iohwsnty.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bqlgbxcp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ajorptgv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mhcngohg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3suvvkquz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ffaufnxi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pptjkbtb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wwucrjkn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3migplngq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rlsmvioh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xukxppin.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kkvzbxwn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pphwiqnm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qfqznnky.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3thpqxdzb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jaryqotd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ssfciuhv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3qyrtfqqs.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3uvunwpqt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3sluesnxt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ndfqiewm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3scyfrltu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3izxbzlyz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lonkisyz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3vghxolwe.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3klkepymz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rsynxqyd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3rvgybqef.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qgnybdxg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3sagspaas.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vrihlqcd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ldozvraj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3qliuguzm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3hosfffxk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nscpckhc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zourwvit.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3utinjjws.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wgeqkimv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wldpiwzk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3fgandyfl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3uemvwtef.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3gydqgmvs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3brsrqayx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zkpthsdu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3qdnrliky.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vnjorrkm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ccmdmzhe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lrarvmgm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3utaqegqx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jheduasm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ixxlamzl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3hfplzpne.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mdiolpty.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3xuvzzbjr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3wzxnbmty.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ucvgrcyk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3sunmnoaw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3goqmmtka.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3idnxhtqb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rbhanxhy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3spnoinju.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3waahfukq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3uncdoaxy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3zfufmowm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gzojukut.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3swjrtqdv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jybwdcup.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fkvfojvo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3hutctwvi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nosufmuu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qsgartzt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ekkonklh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3yekxfypj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mildzrfm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ipkyjepg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bigtjuhs.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3arnzpcxi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3bfujlfhj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3hrlkjltn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3hsgqnynn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jjxkqmtm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3vllbnhkg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sxxdjrio.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mparzguv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hzjsgcbo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qsvgxzaj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fkcvsaqq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3aiwyqkeg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kjjejufe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ehdhcfjy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3upgvmuhf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qzmbgvdr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3gnyyywbi.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wnbbfukd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uplbltqs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3nmsuiejg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3lvzoftor.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ajhmhplh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3mtqgvpmz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3othwnxkj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pgajektj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3anwzqwmq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rartcoso.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kboltura.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3icoiwtsg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3uhtzzmqx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uzatssjn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bcemshfd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rqjzegjm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qztjqfaj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3sxsrslgl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hwnbphfa.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3lqaajccf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3uvmcpsgd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3idhptllh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3btsfejbm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3yafhiugt.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3rgrgaejp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3oiyeipkd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ubjthcrj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3dvoddgxj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3tjhyxvum.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3bizyrwbo.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3uyagzpzb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3qvcrsmnm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3apkyvqky.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3zxnfcmzu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3mqykyixm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ttlzlehh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3fkpbtrgf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pqarjtbc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3esgmklxb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3zxtmyuty.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3vbyhkqyy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3lkdwbrye.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3oynukeko.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3djwfusnr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hwmziktu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3eamewpus.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3usmncgjj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3liinwclt.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3fymjyrnq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3slbuatda.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ojipindi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3uqoaafsg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3amhfsees.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zwlrudpn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3euepojiv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dqaaxdgy.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lymiptaw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3liyvkfgx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3cmqvlhtt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kkqtykbu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3gdgtghsj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3bjnnqqpv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3bavdkwei.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fcadipdm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3eswdafqc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3okoyzvky.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3oiwrdktp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3owmhpfkv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3zwdymdcq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3wpqfqfgo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kjbvbobw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pagvtdyj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ezlsxrvf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3srpxdldz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3lqzfessz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3klacjuzs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3exqsotuh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqypoodx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3qixgvytm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xnfobzau.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zqethpqs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3maicyhol.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3snwoziyz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qqqjjwnv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ybdrpmkh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3laairsaf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3iurmwyfa.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3zplyphjr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3pvtdvjnx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xbaqalaz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3izslugum.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3frejecov.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tbarumoq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3njpmcocy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3kqypmgvh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gruzmyne.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3wnspyahm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vvjsncwj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fimcjqqw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3oshdmszi.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3owwjuaju.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rhgdwpxv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dbhsmcrc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3csazjxbk.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dcbvhhxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ocztsooc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3phsctsaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfymriwm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3heaflwrc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3xspyegas.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jenzfhlx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wtpmgnfe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nvqwehzb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3tvtfgrds.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3tkgxirif.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3npeqlebk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rdqqhakl.html


<!-- 参考信息 -->