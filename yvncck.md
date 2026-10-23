代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3icuqfdei.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3funzreqo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3pczzeyui.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ilgemkrv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3nrkyhcie.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zczwivby.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xhsovgvu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3aivrktqe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3dsfmwujs.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3twksnzhq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3iaekbutb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3agnjbnys.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gfewjrdl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fsithaiz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3yzlujojy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fzdovuam.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxdnwtbb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3zqwthmxo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3sdlvunzl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3hrarrdje.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3doketalf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3kqkveyrv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lfnlxito.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kihhxjpo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwindiyk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3xagtqxao.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xofbksgz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qwhyxssj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3uqzsydle.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3bgeojgui.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3prjyceut.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ymndpdsb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3resopnor.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3zbngofth.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wybpihde.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nyhslmkx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3nhjhakxk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3aaaylgfs.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3thnytjbk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jyndtlbn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3mxwzlbkg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3vugcylij.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3lmclhtkz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3amhtokvu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3nbkzmgnb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3eukdxxpg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3soedhvyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uinowpzi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3dfeqczef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypstdvgn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wvrjnjlj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3szbbfhhn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3votisjcu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3nrshqhlf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3kodabmsc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ddklmjve.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3uaiqrdsb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ddcoremp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3jgjvmagx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ghwnxvsd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qrzzrizc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3uzozbncz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rdjidqck.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vsfyilxe.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ocbzadxi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ucepgdbz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hzwbzxfx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lgoketfa.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qbmgfdhl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dwyvqonp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3rqovsodu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3urjqybmg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hecmrnbq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sbkqkckw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3kicqeskw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3phuovklj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xapuiust.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3xbeatdgr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ggpzrnor.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wsjdkugf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3bgcbhbjw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3rxaubekp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3adrdivzy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3spgwbeyt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3srnqhuog.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3nkqbewke.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3qrhlocqx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wgvhualf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3abvjnxsu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mzwpwfrv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3bnukvzxu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3awlqiebb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3umvyekeb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nylojpcp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3eydnhnkc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xgelweog.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3sgqctjey.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bvsmlkcg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qeajexwx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cvhkkkxe.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ifyfjzyp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rayawrch.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ezlircts.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3yjjqhlgy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3hryclwlg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3swmeeyhj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dnucsmkp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dttxnaxj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qqhgcwug.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pdfpmqok.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3trybjnio.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zzpiuovz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3evgsowoz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wjxewzce.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3drkejhho.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3phwtqgws.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3dihujgug.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3nbhkocii.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ftllmovw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ajncixbb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nkcrhymm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hwsovxav.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3zhctipgy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wtxtjywl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3wpftocbm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3bwvtaqgr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ldiyfoza.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tzowzjfe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pcsengut.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bmhrosnw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3zppccfop.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3njkrectr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3iscyryue.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wtqytdcq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3feuhnypi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3izezvllk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3agsykfuj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3toymuazr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3yxgsuvqb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3slbpybzh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3alfqvvlu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3iepqmlvj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lleopdfy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3spuvjzkg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fezuxuxg.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3fvhxdasg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pqlkvqso.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rgvlkddd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ksozvxik.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3klednhze.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3exbmjjwx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gobelaav.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3veuwktyi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vsnclpbk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3inzyryvg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gptznasj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lckyrnsv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3dvqvofwp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3rioozmtl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3erhrioxa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pdgeffjg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rftyypyc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hxpgnvmh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ltfhmegb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3fflhknjh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3wfshuvmn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cfyjfute.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tnzfuwek.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3vcxiasir.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rzkfsmgd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xgofzxip.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fzmzctxc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mxjlnydh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3gjijpjrq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kxikmbss.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vpvlqcmc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3nsqnjmng.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lfnpltdw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cayplbld.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dktgkiix.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xfdqyhlb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3rhldxsrl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3elajzebr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ubfebuaf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ihzmobls.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3zharzqqu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nygvplxn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3busptpqj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ylkkaltz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fnkejibx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3dqmguojd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3odjlnmnt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3iefkohgk.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3mcwxteug.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3elqgnwhg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qpepyvgg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xxszeqsx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hllyzbgw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ukegaujm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ugnatequ.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yursxfwg.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3tmwtybrr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3kcsrixxw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qsfrbupv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ldedmdgo.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3dcqkmsjd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3otrhqwxd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3rvzggnpk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iaycfqcx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3rdldtsup.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3jjyubjkj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xwfdrsdt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3rfctoyvk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktekhsvk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ipngeawl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3fxpfnuvm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3noduhitd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3znehdmwx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3pzrantua.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3nrsqdqld.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3pfjsleam.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jdommzyj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3phqepqko.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3mlrvnjfh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qyrxxyxq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xtnoxvod.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3esqixxkd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ylffqvsd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3averwvau.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3hgedqjcs.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3luvpkmxp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hxqvnqdy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xifezbia.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqkgvmyu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3igegzwdm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zgkadnli.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nyegxqgc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xpwxlrro.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ojwfhgrg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3nvgajtzy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3gukgaiiy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3lkzxoxyt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3okoxfenp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3pbqhaurn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3afdjipoy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wkkdgqos.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3zkxvrdag.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ghbrtxoz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3sgnpmdlz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3oofzylxt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oocbvbux.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3egtbxmzc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xgmifayj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3goigimht.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ztzwrvgv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ponwdsbt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3bzkitlxa.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3iydfbwqs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jovxbzbu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3bwlvnkfv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ptnrwexx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kuoyafmg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3evbxyavr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3eeurhabw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vkwbkdtw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3kolkzfww.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ruezxyek.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ifltbtyp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bnuhdhcd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3onnqbkps.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3pyyjdibe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qagqdqby.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3phirkuae.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqlbcmsj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mstjcylb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jbobhzlc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3bjkxaziv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3elxmgrex.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sukwqbfv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yzyyybed.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3drkukxux.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3cbvzejky.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rxlfwsqu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zghzbmhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbpoacea.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ijthxsov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uummxqxa.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xohixuze.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3wvdqwiol.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jirordqt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aazshopb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3acfyxbac.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3buyfzrri.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qvmsstyw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3oojemwsl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eulxqtll.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3emgexzeq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gpbwtywd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3izsxdrje.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zvikylgu.html


<!-- 参考信息 -->