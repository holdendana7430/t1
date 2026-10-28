代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.havefunace.top/gtkonxcmer.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gthwfuvgps.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.iojbl.cn/gtniwvgpzi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.shuidangran.top/gtviiyfxxf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yonumen.top/gtebyapppn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.fengsongda.top/gtvhavnohk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.0kj1m.cn/gtyzfvmyyp.html

[C09] 递归
来源：http://hz.nwbrower.top/gtbadondzl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.mhx1999.top/gtntjjbjce.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.nanxinkj.top/gtqlvodvrl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gzhubu.top/gtxvdjangm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xylfe.cn/gtgtseeygq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhiwuduotai.top/gtzanynhme.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.kuanghao11.cn/gttxnofvru.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sysykeji.top/gtexjncvju.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.daxiang520.top/gtswziptri.html

[C10] 变量作用域
来源：http://hz.guannengcc.top/gtgnbhoyah.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cqqwz.cn/gtkhbhwwtp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xziqi.cn/gtsiwoewrg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.sweek.top/gtmgzobfwx.html

TS:   同 JS
来源：http://hz.jinyuanbaomall.cn/gtadplhuql.html

Java: 方法内为块级作用域
来源：http://hz.hywenlv.cn/gtzaipjnxx.html

Go:   花括号块级作用域
来源：http://hz.chenjidiqi.icu/gtoiafxjmf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhixingplan.top/gthvxrblch.html

C#:   块级作用域
来源：http://hz.jinyuanbaomall.cn/gtygxstcqr.html

[C11] 模块导入与导出
来源：http://hz.smart0.xyz/gteoqquikk.html

Py:   from module import func
来源：http://hz.zhijiandao.cn/gtqtcvfern.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.feifeiyinyue.top/gtqjmbocqq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hfpthk.cn/gtbgkvyxwy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.c1oappe.top/gttuficwxf.html

Java: import java.util.List;
来源：http://hz.cdnleiting.top/gtqsxmhvax.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ywan-chungtsiang.top/gtkaakcvih.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhoulong.xyz/gtmscuyley.html

C#:   using System.Text;
来源：http://hz.svipenyu.cn/gtcsfejbie.html

[C12] 立即执行函数 IIFE
来源：http://hz.ydjk.org.cn/gtwiamvfpr.html

Py:   (lambda: print("run"))()
来源：http://hz.yanxiufei.cn/gtuosnqmuq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.aizwys.cn/gtrhlqkgbj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yuxming.cn/gthhxaxvil.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jlsjyb.cn/gtuqjgkowm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shuidangran.top/gtoctktlll.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hysaishi.cn/gtjpvnbyqp.html

Ruby: -> { puts "run" }.call
来源：http://hz.sweek.top/gttguvyxfh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinqigufen.top/gtpqhtzgur.html

[C13] 类型声明 / 类型注解
来源：http://hz.ehwqpu.com/gtnlbmevvh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.pengpengdd.cyou/gtkotvvldy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aibaodan.cn/gtgkaursuc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.andypj.xyz/gtoginpvxj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.havefunace.top/gtwxriqwuw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.meibo888.top/gtaaapglus.html

Go:   func add(a, b int) int
来源：http://hz.yangfankeji.com/gtpcemcecv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hammf.cn/gtfoslyidq.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.tanke756.top/gtgjrzoeuz.html

[C14] 泛型函数
来源：http://hz.shzxlz.cn/gtxjobscth.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.svipenyu.cn/gtujkswqin.html

PHP:  // 无泛型
来源：http://hz.yongpay.top/gtslqseiiq.html

JS:   // 无泛型
来源：http://hz.redwolf501.top/gtndrdwbqo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sufxvd.cn/gtujanycaj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.haohaochexian.top/gtqfqzcpps.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cdnleiting.top/gtxywruymx.html

Ruby: # 无泛型
来源：http://hz.hywenlv.cn/gttndiyxwm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.svipenyu.cn/gtdceepeul.html

[C15] 解构 / 展开参数
来源：http://hz.hammf.cn/gtqxunljth.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yueranfly.top/gteunqspfl.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hywenlv.cn/gtezyxfwtf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.bjfxy.top/gtckadniwf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ywan-chungtsiang.top/gtjnlaiycm.html

Java: // 无解构
来源：http://hz.pycfn.com/gttqmxynet.html

Go:   // 无解构
来源：http://hz.hywenlv.cn/gtmlhzsixq.html

Ruby: a, b = pair
来源：http://hz.yuxming.cn/gtopzsrrfz.html

C#:   var (a, b) = pair;
来源：http://hz.smart0.xyz/gtpuukgsrp.html

[C16] 函数 / 方法重载
来源：http://hz.jlsjyb.cn/gtpgnqolpm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gogol.net.cn/gtterfxali.html

PHP:  // 无重载
来源：http://hz.sweek.top/gtmqytasad.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.haohaochexian.top/gtrhckptwf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.aibaodan.cn/gtlnltfhhx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nwbrower.top/gttmwjralp.html

Go:   // 无重载：用不同函数名
来源：http://hz.nanxinkj.top/gtycshcysa.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ppjwa.cn/gthbszkncm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinghuilouyu.cn/gtngkvhrbb.html

================================================================================
来源：http://hz.ivvv.top/gtujgwgzca.html

D. 数组 / 列表 / 集合
来源：http://hz.chenjidiqi.icu/gtyaumldea.html

================================================================================
来源：http://hz.zhengqikj.top/gtfmguquwd.html

[D01] 创建数组 / 列表
来源：http://hz.zhoulong.xyz/gtptuoyxnk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinqigufen.top/gtybkubaii.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yongpay.top/gtfguzpndl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ybcxt.top/gtpdrdogkv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj202588.top/gthmkmceru.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.vqdsnc.cn/gtaihxilvp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.chenjidiqi.icu/gtifznecsk.html

Ruby: arr = [1, 2, 3]
来源：http://hz.vqdsnc.cn/gtcenbglpf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.bjfxy.top/gtsgyaggqg.html

[D02] 追加元素到末尾
来源：http://hz.yuxming.cn/gtjmyfrncp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.daria6918.cn/gthrlcwhzt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.pycfn.com/gthkyojoub.html

JS:   arr.push(4);
来源：http://hz.ppjwa.cn/gtvslvdpwl.html

TS:   arr.push(4);
来源：http://hz.zhengqikj.top/gthuczbija.html

Java: list.add(4);
来源：http://hz.cqqwz.cn/gtldqtknzx.html

Go:   arr = append(arr, 4)
来源：http://hz.hnqzz.top/gtztawtnkv.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shzxlz.cn/gtqbxdwldx.html

C#:   list.Add(4);
来源：http://hz.hfpthk.cn/gtwueukopv.html

[D03] 在指定位置插入元素
来源：http://hz.mhx1999.top/gtcrtnqxwv.html

Py:   arr.insert(0, 0)
来源：http://hz.sufxvd.cn/gtidrzkmkr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shuidangran.top/gtqwiwdkcb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shanyushiyangkeji.top/gtnwmznkyc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhijiandao.cn/gtjvjswotj.html

Java: list.add(0, 0);
来源：http://hz.guannengcc.top/gthjcaufrg.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xuanzx.com/gttnglbvey.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.fzhhl.top/gtvalgavhg.html

C#:   list.Insert(0, 0);
来源：http://hz.yongpay.top/gtfcajzzfg.html

[D04] 删除元素
来源：http://hz.shanyushiyangtech.top/gtxoetgthv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ybcxt.top/gtyqmraxxm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.svipenyu.cn/gtdpqqsnys.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.fzhhl.top/gtfnyweyoq.html

TS:   arr.splice(0, 1);
来源：http://hz.yueranfly.top/gtjzccdnax.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xziqi.cn/gtekodudjf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nwbrower.top/gtmmvvyvqt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.fzhhl.top/gtlzepxxhi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.meibo888.top/gthtuuvzgr.html

[D05] 访问与修改元素
来源：http://hz.bjfxy.top/gtstnruxxv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtrujmiacq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sweek.top/gtaeoqzeru.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.mhx1999.top/gtshhxhzjg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guowangkeji.top/gtpavkxmdm.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.pengpengdd.cyou/gtqqtqtugc.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yonumen.top/gtnocvglvs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.havefunace.top/gtydclplpy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.dashuyun.cn/gtgeeaikwn.html

[D06] 数组长度
来源：http://hz.sxryk.cn/gtsfldhuun.html

Py:   len(arr)
来源：http://hz.dianchejie.cn/gtnzvxlnvm.html

PHP:  count($arr);
来源：http://hz.jinqigufen.top/gtuszihgdj.html

JS:   arr.length
来源：http://hz.tian-w.cn/gttxevkddx.html

TS:   arr.length
来源：http://hz.yuxming.cn/gtpfimicgn.html

Java: list.size();
来源：http://hz.cqqwz.cn/gtvjxlgloi.html

Go:   len(arr)
来源：http://hz.jinyuanbaomall.cn/gthbxompkd.html

Ruby: arr.length; arr.size
来源：http://hz.gzhubu.top/gtewxkwxfi.html

C#:   list.Count;
来源：http://hz.pycfn.com/gtbgtwkpsd.html

[D07] 切片 / 取子数组
来源：http://hz.cheryme.top/gtsjihfloz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shuidangran.top/gtekmupqka.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.vqdsnc.cn/gtghkurtub.html

JS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gtfyyztnzg.html

TS:   arr.slice(1, 4);
来源：http://hz.svipenyu.cn/gtkvhkfule.html

Java: list.subList(1, 4);
来源：http://hz.ppjwa.cn/gtukuoodbj.html

Go:   arr[1:4]
来源：http://hz.52xcode.cn/gtkdwyssue.html

Ruby: arr[1, 3]
来源：http://hz.xuetiantiany.cn/gtrhzdrtau.html

C#:   list.GetRange(1, 3);
来源：http://hz.sysykeji.top/gtnzkqhnll.html

[D08] 合并两个数组
来源：http://hz.c1oappe.top/gtydoxnvls.html

Py:   a + b;  a.extend(b)
来源：http://hz.ppjwa.cn/gtrwakgfdv.html

PHP:  array_merge($a, $b);
来源：http://hz.jqgfzy.top/gtalvczvld.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yongpay.top/gtujjtzabb.html

TS:   [...a, ...b];
来源：http://hz.daxiang520.top/gtbzgvjkfg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.316326.xyz/gttuxrclrb.html

Go:   append(a, b...)
来源：http://hz.yj20258.top/gtwliavtmp.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yuxming.cn/gtytwtdjxj.html

C#:   a.Concat(b).ToList()
来源：http://hz.tianlin.xyz/gtgzvksaqk.html

[D09] 排序（升序）
来源：http://hz.yuanzhike.top/gtdhupcgjh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigufen.top/gtcsvkhikv.html

PHP:  sort($arr);
来源：http://hz.tanke756.top/gtbdkpeycj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.pengpengdd.cyou/gtnpkpxtwb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sysykeji.top/gtkpmsfplw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.guannengcc.top/gtgtgsqzuj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cashguo.top/gtgrssqqne.html

Ruby: arr.sort
来源：http://hz.ydjk.org.cn/gthygxtpop.html

C#:   list.Sort();
来源：http://hz.bjfxy.top/gtlmjvzonn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhijiandao.cn/gtppkkyqhv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.0kj1m.cn/gtvrlikdso.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.quarkkingdee.top/gtbsxobqac.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenzaomai.com/gtoufofhrr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.bjfxy.top/gtykktcias.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinqigufen.top/gtdmzbkwyl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinghuilouyu.cn/gtkphtismy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.bjfxy.top/gtlnhwqokl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hywenlv.cn/gtbvtbexxc.html

[D11] 反转数组
来源：http://hz.yanxiufei.cn/gtfblqyrgu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.snrcjt.cn/gtrgmfsbdy.html

PHP:  array_reverse($arr);
来源：http://hz.ppjwa.cn/gtqppzpxke.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shanyushiyangkeji.top/gtgamrcxcm.html

TS:   [...arr].reverse();
来源：http://hz.wangdashe.top/gtlxwamhds.html

Java: Collections.reverse(list);
来源：http://hz.c1oappe.top/gtibqarfxl.html

Go:   slices.Reverse(arr)
来源：http://hz.birdmap.top/gtnemdqwpu.html

Ruby: arr.reverse
来源：http://hz.xylfe.cn/gtwyjmtjrl.html

C#:   list.Reverse();
来源：http://hz.jinqigufen.top/gtaykoqvvz.html

[D12] 查找元素下标
来源：http://hz.snrcjt.cn/gtenuirszu.html

Py:   arr.index(x);  x in arr
来源：http://hz.iojbl.cn/gtflitwppd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xinyue.icu/gtazaskzhq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nanxinkj.top/gtzjgtiwmu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ywan-chungtsiang.top/gtnfnntkby.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hongshengwenyu.top/gtwivmbvcc.html

Go:   slices.Index(arr, x)
来源：http://hz.pengpengdd.cyou/gthwwrjcel.html

Ruby: arr.index(x)
来源：http://hz.yvedp.cn/gtwbzxtgrd.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangkeji.top/gtcggmbbrm.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhiwuduotai.top/gtlybrlhfv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zycfv.cn/gtlfekgzrx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenjidiqi.icu/gtvnyylgoi.html

JS:   arr.filter(x => x > 3)
来源：http://hz.daria6918.cn/gtibeqetih.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jlsjyb.cn/gtyghrgpgj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj202588.top/gtjufpzdok.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.dianchejie.cn/gtwfepwwsq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhengqikj.top/gtonzasiyl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhaomingkeji.xyz/gtdgihbgye.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinqigufen.top/gtyzvsjapy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ydzc1.top/gtjdelzrpl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhaomingkeji.xyz/gtvmyrjqku.html

JS:   arr.map(x => x * 2)
来源：http://hz.vqdsnc.cn/gtpvwjkfmf.html

TS:   arr.map(x => x * 2)
来源：http://hz.ydzc1.top/gtgerweqmb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.pengpengdd.cyou/gtqaajpqdw.html

Go:   // 手写循环
来源：http://hz.mhx1999.top/gtytksybzk.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yvedp.cn/gtsrqjhbhm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.smart0.xyz/gtbvqauceq.html

[D15] 去重
来源：http://hz.52xcode.cn/gtvbwiklps.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.birdmap.top/gtghkhxqsv.html

PHP:  array_unique($arr);
来源：http://hz.yvedp.cn/gtrujrvhzx.html

JS:   [...new Set(arr)]
来源：http://hz.shuidangran.top/gtrhpnhfeq.html

TS:   [...new Set(arr)]
来源：http://hz.jqgufenzy.top/gtfcuuaqtj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.pengpengdd.cyou/gtxktmstfc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ywan-chungtsiang.top/gtyxzutogq.html

Ruby: arr.uniq
来源：http://hz.sweek.top/gtebwymnzg.html

C#:   list.Distinct().ToList()
来源：http://hz.hnxiangtu.top/gtxiycgkgi.html

[D16] 求和与平均值
来源：http://hz.mhx1999.top/gtyurwujvi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sysykeji.top/gtzujizdwl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.gotoacloud.top/gtbrlbzora.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.birdmap.top/gtolcnfujm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258.top/gtqmdhdnbf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cqqwz.cn/gtpyvnvnyo.html

Go:   // 手写循环累加
来源：http://hz.zhongyouzk.top/gtbewynrce.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shuidangran.top/gtgnvhvxok.html

C#:   list.Sum();  list.Average()
来源：http://hz.jlsjyb.cn/gthpmzxvsn.html

[D17] 最大值与最小值
来源：http://hz.gogol.net.cn/gtrhacaecq.html

Py:   max(arr);  min(arr)
来源：http://hz.wangdashe.top/gtcgrpntwy.html

PHP:  max($arr);  min($arr);
来源：http://hz.mhx1999.top/gtcwbgwihw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jianghu66.top/gtdqxikpcb.html

TS:   Math.max(...arr);
来源：http://hz.xziqi.cn/gtwrhbvoex.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenzaomai.com/gtzdmyhynv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shuidangran.top/gtuznyxkie.html

Ruby: arr.max;  arr.min
来源：http://hz.guannengcc.top/gtejcjjtsm.html

C#:   list.Max();  list.Min()
来源：http://hz.jyoumei.cn/gtlhcewwos.html

[D18] 扁平化嵌套数组
来源：http://hz.hfpthk.cn/gtphexyvbp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.redwolf501.top/gtdicknrud.html

PHP:  array_merge(...$nested);
来源：http://hz.hnxiangtu.top/gtocdphyfh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.dashuyun.cn/gtcgzwyfhf.html

TS:   nested.flat();
来源：http://hz.yj202588.top/gtpdtowdmn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ppjwa.cn/gtdlgimduf.html

Go:   // 手写双层循环
来源：http://hz.feifeiyinyue.top/gtqvgdfmfo.html

Ruby: nested.flatten
来源：http://hz.52xcode.cn/gtyxpwtuez.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yangfankeji.com/gtsbtuhaqo.html

[D19] 按字段分组
来源：http://hz.shanyushiyangkeji.top/gtfbycwcpp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.nwbrower.top/gtuguqlvel.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nanxinkj.top/gtvoaokfsd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cheryme.top/gtxjdixxis.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.svipenyu.cn/gttuepilgy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yanxiufei.cn/gtdilctypa.html

Go:   // 手写 map[string][]T
来源：http://hz.tanke756.top/gtbwyyjkge.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.redwolf501.top/gtlyvmtuwx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.dianchejie.cn/gtyywipnbg.html

[D20] 统计每个元素出现次数
来源：http://hz.xingfuxueyuan.xyz/gtfgkviusk.html

Py:   Counter(arr)
来源：http://hz.zhixingplan.top/gtomvebopi.html

PHP:  array_count_values($arr);
来源：http://hz.meibo888.top/gtgwyphewh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.birdmap.top/gtelvxnltp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yueranfly.top/gtpgwgembe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.fzhhl.top/gtnvdicama.html

Go:   // 手写 map[T]int
来源：http://hz.shanyushiyangkeji.top/gtbgjvkjoy.html

Ruby: arr.tally
来源：http://hz.sweek.top/gtvrpqsjov.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.316326.xyz/gtnupnrggs.html

[D21] 判断是否包含某元素
来源：http://hz.dashuyun.cn/gtnkoindxs.html

Py:   x in arr
来源：http://hz.smart0.xyz/gtdjciqtxe.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yvedp.cn/gtmcrzsloy.html

JS:   arr.includes(x)
来源：http://hz.yuxming.cn/gtzeodhrst.html

TS:   arr.includes(x)
来源：http://hz.shangyingyoupin.top/gtxtbkxuoz.html

Java: list.contains(x)
来源：http://hz.cashguo.top/gtpzoumppu.html

Go:   slices.Contains(arr, x)
来源：http://hz.zycfv.cn/gtkpcxazfg.html

Ruby: arr.include?(x)
来源：http://hz.daria6918.cn/gtnzoqxiox.html

C#:   list.Contains(x)
来源：http://hz.fzhhl.top/gtshmcqqcp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cdnleiting.top/gtbytealws.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hnqzz.top/gtcjxubdpw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jiagoushi.top/gtbgydjcvo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zycfv.cn/gtzixykihn.html

TS:   [...arr];
来源：http://hz.shanyushiyangtech.top/gtrjkskhxc.html

Java: new ArrayList<>(list);
来源：http://hz.yongpay.top/gtkmnohznp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj20258.top/gtxqfmowjq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.fzhhl.top/gtiuhosuih.html

C#:   new List<int>(list);
来源：http://hz.yanxiufei.cn/gtbyxxacvn.html

[D23] reduce 累积计算
来源：http://hz.shanyushiyangtech.top/gtjyltyuci.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hammf.cn/gtypshbtbv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xuetiantiany.cn/gtazbnkplr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xuetiantiany.cn/gtrpoqzwmh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.daxiang520.top/gtkwufryho.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hysaishi.cn/gtevpzdjru.html

Go:   // 手写循环
来源：http://hz.ydjk.org.cn/gtkdldmwox.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yongpay.top/gtzttyxlxx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.316326.xyz/gtojyfdsjl.html

[D24] 字典 / Map 基本操作
来源：http://hz.cqqwz.cn/gtdpqyxugq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shanyushiyangkeji.top/gtwyyjhdet.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.daria6918.cn/gtxfypmtek.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.tianlin.xyz/gtsuoudcne.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.svipenyu.cn/gtpbqlasyq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.52xcode.cn/gtzkojnwbu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yj20258888.top/gtirntyazv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhongyouzk.top/gtkgwzjgci.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gogol.net.cn/gtptdjmgub.html

[D25] Set 集合去重与交并差
来源：http://hz.jyoumei.cn/gtavlfnhvi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.9152youxi.cn/gtgcdjtwox.html


<!-- 参考信息 -->