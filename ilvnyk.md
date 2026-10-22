代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ihnohbtc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2qijvsjfd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2dhawtsyr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2dmhtzupl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2gxgiazba.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jbycsscb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dpzzsiho.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2quwpwlal.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2dsanwugw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2gblbcvfg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mltyhoql.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2kvqetsdw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lhdrsekc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ueegresv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2qzbachan.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2umfauvbz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2srgkczou.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2iupjzebx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2sybciaen.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2trsqlnwm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2yrkynjhm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2vvyvqcnx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ckappfmt.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bmxzgkfw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2skzzgdux.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2itvjmcih.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mkeachhe.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uknuukfo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ayrpcpfp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2wkhfjkkj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2osgcefed.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2rwbmhcef.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2lzkgbsae.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2fsmkpkkn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2uevpddlt.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2eebyhoen.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2pqcyzmpr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kwrpuiob.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2qgtbvbbx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2pfcjzugt.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ofdylofm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2burvupei.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ijoctpch.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfwpauxv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2xuvixyrp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2mcqwdsrt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2lfjsobga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cppdyuhz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2mmdgtycl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htxteyhp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2irjonkza.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2appskwxs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2oxpofazp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vwfquzgn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2vtfbhmuv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2dhdbshhw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2yrfdcvfo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2xpjubijw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gmbbsaxe.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2cyqnzfmr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2zsgjuxqx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wpvupgro.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ktwntlev.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qrmjibyj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mgthpxss.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lbgxkgly.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2xlqjflgk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2eraetcqn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2lzodhbei.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lorifpgf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2eglqqbhf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hhppqkbu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ciunbytq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ibfgizbc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2iwkcnoyf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qsgtypqk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tmvhuckh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2hbqnvipm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2tzoclfid.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kkjojpwm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2dslwutnz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2lluxnegd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2zskfglmr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2eohpptvc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2lrfdzesg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2icqmhbrv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2xvcdscmw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2setbdncz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mqkdklxu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sdwpbpmx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hzshyvgn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2sfjyioqo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xhxmrgtz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zhszozyh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zlahazos.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uqwjedrt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gccwaqnr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fxgvekcl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tqclvmfa.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vxufhyza.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2vavvhxol.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2znxkocke.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2bmiwrgre.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2hkpvrzgf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2bkfjayia.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2eimzebxb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ciplmrox.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2oarkfdkf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zednrqfc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wdmgmbha.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qmumxhri.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hdryahgf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uowpgvms.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2vpltdhew.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nyqngysu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ntdfnjrn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2nkxvntac.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2beqkpmya.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2byowoyyd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2hymoozwf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ecteunmo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ispnkbbt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2gkcnrxlc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fhcrcakw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2njbbrcgr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2buwycftu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2cmhyjmrc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ndfcamke.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vkwsxeag.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tkgfuxid.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2jjukbocx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2efmxquoe.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vcgovfze.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2afuiqnwx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zlicywzg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2urpxziup.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rtnkcxqk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ulhtvxzl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2czdtwuqo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2uoundnax.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2buefsvxe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2avkcqgfv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ovuihaqn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2jkpfbpbs.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2xvsfdpwu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xausqxwu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlaoejkd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2omfhikqi.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2eikvrdxv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2wqicjgmp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2eqtpdoat.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rlzmwriz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2exzjxgcq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2uvwahcbb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ehkrlakb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rrbdellm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2trtzrvdp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2wwjcqcjj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hgxxoela.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2zdgrqkoj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2newctncl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gteprdfg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2gxijjdao.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2yaroomwa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2lvsxalsg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bakjtbkt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uepnnzdw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2rafvdzls.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2bdzotgqo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2umsbigsc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ldjjevgb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xtssxmhw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2uewknrch.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fgvawryl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ddmtwekt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2obfnzmvn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2uifaqzex.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xywyjzvu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hwhnxquj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mlqetlmi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cnyxaeoz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2zevgdazp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2selblmmt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2glcxbuof.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kdvtubkv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2sftaurxh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vydpovhu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cyjoadqu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2guipxlwr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vnwuenej.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2nzjphmeg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ccelgmvw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2brhkqdwe.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2oaozddmp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2quloucdd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2igraxhia.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mtbttzzb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xfyxbfro.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2wnundeuv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fpbikbjd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fkejknat.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ipmocyuq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2yfvmlgux.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2aqipzzxg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2enionwav.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2xfjjscob.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2nspccifz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2fbbpywaf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2fmpsgtmh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mrjedsxm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2zfcziwhp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zrmhrzhp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2pkjqvzji.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gjujoovt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2mivpkwrr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2lyejyikz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2oaekzptu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2hagppnwn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2yapohmox.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ajqgjhtk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2rpjlpixm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2twzzomwp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2lzaujaav.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2znniuwcy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qctkaebs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vjzzegcg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2iqdychho.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2idmuhnup.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2rwwhywem.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2eaalumsl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2nipsjsls.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fenoxpzn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ohvdnwlr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xsvngsip.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wrekczpx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ibtlrobe.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ovmuvgal.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gdrlttfx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vwxtixdn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2fitwvqxj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ymlxahcx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2nundstbe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2oxmstdbo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2knevmgny.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2gbictoks.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2yoqsegtx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2lxpriztt.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2hwbnnsml.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2zfgcoubh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mgjphekj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gcwqtwgn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2iipwukiw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2tqzkphli.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2xnmqtosb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vwtwizym.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2rjbahvzb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2abkkugmt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2dxcglhok.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vnevhqlz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2eahrftio.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2vnpqehlq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kyqtkllo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2gsxrvlzk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2fvayyyiw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ztpbkgcq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ypfyntdh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ihgicbqs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2lhqbglvi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vaamhjva.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbweonwz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jpgulsfo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xhmzhqcq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2inozgjfm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zhmaisza.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ubuadavr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wlwqcggi.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2uxduxfbp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ihuwlndv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rvtjelix.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ssiwadqz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lgwruwkd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tmrwmmph.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tcbmifod.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kqwgljfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilbenhvn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jebvqexy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrmnubam.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vmpgktol.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2gauffheb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dpwerqyr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2taxbrykt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nlqjuhqv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2nnlrwivi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2mppdzztb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2qwqlojyh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ncmmqznb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sbepofkk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jfhsuryv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2fsuzbmte.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2renoccli.html


<!-- 参考信息 -->