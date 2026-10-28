代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yueranfly.top/gtuvnekpfw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.guannengcc.top/gtimeokypt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yj20258.top/gtemrxwnry.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yuanzhike.top/gtzpzpzanv.html

Go:   // 无：用配置结构体参数
来源：http://hz.sweek.top/gthgqboopr.html

Ruby: f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtycjdragw.html

C#:   f(a: 1, b: 2)
来源：http://hz.0kj1m.cn/gtsiyskdiz.html

[C05] 返回多个值
来源：http://hz.wangdashe.top/gtdayzczfx.html

Py:   return a, b
来源：http://hz.haohaochexian.top/gtpmfkhvfu.html

PHP:  return [$a, $b];
来源：http://hz.tianlin.xyz/gtcjhkonob.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.gzhubu.top/gtluekqimy.html

TS:   return { a, b };
来源：http://hz.ywan-chungtsiang.top/gtruvjfzpw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ydzc1.top/gtjjbfgqsb.html

Go:   return a, b
来源：http://hz.tianlin.xyz/gtkpzdlyum.html

Ruby: return a, b
来源：http://hz.jinqigfzy.top/gtzsjrrpmj.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zycfv.cn/gtuitwbzcd.html

[C06] 匿名函数 / lambda
来源：http://hz.fengsongda.top/gtjwcahgiw.html

Py:   square = lambda x: x * x
来源：http://hz.hnqzz.top/gtpekxxzcw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.tanke756.top/gtdaozjvma.html

JS:   const square = x => x * x;
来源：http://hz.cqqwz.cn/gtmzudbnbv.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hywenlv.cn/gtkfpclhho.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.52xcode.cn/gtylppomel.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xuetiantiany.cn/gttkaewoek.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hnqzz.top/gtqbqoldjm.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cqqwz.cn/gtzclvarvx.html

[C07] 把函数作为参数传入
来源：http://hz.gaohongyu789.top/gtkcsrwbbl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.guannengcc.top/gtwycssnic.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yueranfly.top/gtujwxzgzo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.snrcjt.cn/gtzeajpuyr.html

TS:   arr.map(String)
来源：http://hz.hongshengwenyu.top/gtdvurptnx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgufenzy.top/gtbxmnpbai.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gotoacloud.top/gtesoaobxr.html

Ruby: arr.map(&:upcase)
来源：http://hz.vqdsnc.cn/gtknqsvtzg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yangfankeji.com/gtyntttjia.html

[C08] 闭包
来源：http://hz.yanxiufei.cn/gtrhprhbsy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jyoumei.cn/gtfxrccwun.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.snrcjt.cn/gtzxxoyina.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ybcxt.top/gtwfmuwldn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jinqigufen.top/gtttckqqkz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cqqwz.cn/gtqfyphcot.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.316326.xyz/gtpwebitgt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.mhx1999.top/gtfhafakob.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.haohaochexian.top/gtaboldyth.html

[C09] 递归
来源：http://hz.yangfankeji.com/gtzomwsjrh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.316326.xyz/gtjkgcnfvj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.kuanghao11.cn/gtxofhbpdd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangkeji.top/gtzlctgyso.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinqigufen.top/gtjiytluev.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhengqikj.top/gtjdvmtjtq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.gzhubu.top/gthvcmrmuv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinyuanbaomall.cn/gtbfqcqiag.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhengqikj.top/gtbxssjhpm.html

[C10] 变量作用域
来源：http://hz.shanyushiyangtech.top/gtptcuqnfu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ppjwa.cn/gtfmxaljyk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.aibaodan.cn/gtegkjgbdp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cheryme.top/gtoyfkgdvl.html

TS:   同 JS
来源：http://hz.guannengcc.top/gtzetnwlit.html

Java: 方法内为块级作用域
来源：http://hz.zhoulong.xyz/gtlxjzmwdc.html

Go:   花括号块级作用域
来源：http://hz.zhijiandao.cn/gtlbovzkxe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yongpay.top/gtqvfmibpb.html

C#:   块级作用域
来源：http://hz.bjfxy.top/gteokpkucs.html

[C11] 模块导入与导出
来源：http://hz.meibo888.top/gtiwipupqm.html

Py:   from module import func
来源：http://hz.nwbrower.top/gtvbatlczs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.chenlongwang.top/gtnmxdxmfd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.meibo888.top/gtyncdgkax.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shuidangran.top/gtzsafjrwt.html

Java: import java.util.List;
来源：http://hz.zhixingplan.top/gtgflftalf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigfzy.top/gtgicussgd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yuanzhike.top/gtlcidktsn.html

C#:   using System.Text;
来源：http://hz.gzhubu.top/gtbbauvwtk.html

[C12] 立即执行函数 IIFE
来源：http://hz.hongshengwenyu.top/gtjblneuyd.html

Py:   (lambda: print("run"))()
来源：http://hz.cqqwz.cn/gtekgwpcng.html

PHP:  (function () { echo "run"; })();
来源：http://hz.meibo888.top/gtpqhohxts.html

JS:   (() => { console.log("run"); })();
来源：http://hz.iojbl.cn/gtypcvrcfo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangtech.top/gtxjcoabwf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cucudq.cn/gtenyfwwhg.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ydjk.org.cn/gtmuxhxkbc.html

Ruby: -> { puts "run" }.call
来源：http://hz.chenzaomai.com/gtvwriqxte.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jlsjyb.cn/gtufngfyga.html

[C13] 类型声明 / 类型注解
来源：http://hz.shanyushiyangtech.top/gtaaftzkiq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hfpthk.cn/gthlrzxogi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtkfjbbwcb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jqgufenzy.top/gtejumpzam.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnqzz.top/gtngzvcsuw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtgtnjyzcv.html

Go:   func add(a, b int) int
来源：http://hz.zhiwuduotai.top/gtpnfurxcd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhiwuduotai.top/gtysvpswxo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenjidiqi.icu/gtivdevfac.html

[C14] 泛型函数
来源：http://hz.hywenlv.cn/gtsytzrigd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gaohongyu789.top/gtueapobjz.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangtech.top/gtvehcexch.html

JS:   // 无泛型
来源：http://hz.ywan-chungtsiang.top/gtxuepmijm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.vqdsnc.cn/gtfptkqmar.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.tanke756.top/gttkccrzhw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shuidangran.top/gtasqzsyrt.html

Ruby: # 无泛型
来源：http://hz.birdmap.top/gtpodekppv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.52xcode.cn/gtclnncmmg.html

[C15] 解构 / 展开参数
来源：http://hz.haohaochexian.top/gtmpzblsan.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.haohaochexian.top/gtzvcexlis.html

PHP:  [$a, $b] = $pair;
来源：http://hz.pycfn.com/gtvnyraycx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.kuanghao11.cn/gtjekfqnyz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xinyue.icu/gtpmkuqdai.html

Java: // 无解构
来源：http://hz.yj20258888.top/gtcljrdzkx.html

Go:   // 无解构
来源：http://hz.daria6918.cn/gtzypaspjw.html

Ruby: a, b = pair
来源：http://hz.52xcode.cn/gtkqnmpxsc.html

C#:   var (a, b) = pair;
来源：http://hz.zhijiandao.cn/gtorlupadi.html

[C16] 函数 / 方法重载
来源：http://hz.tian-w.cn/gtgnhwqqnn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.pycfn.com/gtbjfyegtt.html

PHP:  // 无重载
来源：http://hz.jqgfzy.top/gtbhmjafrt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xylfe.cn/gttxligwqr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xziqi.cn/gtekcqwdoc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.feifeiyinyue.top/gtrfovidtn.html

Go:   // 无重载：用不同函数名
来源：http://hz.gotoacloud.top/gtokrnuwhz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinqigufen.top/gtnflzliwe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xuanzx.com/gtnieoyxyc.html

================================================================================
来源：http://hz.zdqjudy.top/gtdbgikaph.html

D. 数组 / 列表 / 集合
来源：http://hz.wangdashe.top/gtqqlpkovq.html

================================================================================
来源：http://hz.jinqigfzy.top/gtmemfcwfj.html

[D01] 创建数组 / 列表
来源：http://hz.cucudq.cn/gtlfuxbkos.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhengqikj.top/gtscmsnhto.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jqgfzy.top/gtnjrptbvp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zdqjudy.top/gtdzwqohej.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.chenjidiqi.icu/gtjnslidnb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.bjfxy.top/gtirrvyiyq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jlsjyb.cn/gtfwaifbrz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yueranfly.top/gtdgqpuwsw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ydzc1.top/gtzwacpetx.html

[D02] 追加元素到末尾
来源：http://hz.yueranfly.top/gtqooquobw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.daria6918.cn/gtaugunaaq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.kuanghao11.cn/gthtovzwxx.html

JS:   arr.push(4);
来源：http://hz.yj20258888.top/gtogzkzzmq.html

TS:   arr.push(4);
来源：http://hz.chenzaomai.com/gtrniwrgau.html

Java: list.add(4);
来源：http://hz.jinqigufen.top/gtdfzauxtm.html

Go:   arr = append(arr, 4)
来源：http://hz.andypj.xyz/gtcnzzuvbf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yvedp.cn/gtzwsslsad.html

C#:   list.Add(4);
来源：http://hz.yangfankeji.com/gtqmryfler.html

[D03] 在指定位置插入元素
来源：http://hz.yuanzhike.top/gtwbqufzgs.html

Py:   arr.insert(0, 0)
来源：http://hz.shanyushiyangtech.top/gtzsxzsilh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jianghu66.top/gtvfvoqkni.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.fengsongda.top/gtidhkbeeq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yonumen.top/gtqbvwthea.html

Java: list.add(0, 0);
来源：http://hz.ydzc1.top/gteibjtvaf.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.aizwys.cn/gtfzmpfugb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shuidangran.top/gtvnhygpji.html

C#:   list.Insert(0, 0);
来源：http://hz.andypj.xyz/gtcqblvwzb.html

[D04] 删除元素
来源：http://hz.yuxming.cn/gtlkxzcaku.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xziqi.cn/gtcuzcnneg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yuxming.cn/gtekpbgdlj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.wangdashe.top/gthugldujd.html

TS:   arr.splice(0, 1);
来源：http://hz.ydzc1.top/gtsasixuzj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shangyingyoupin.top/gthyrkyjre.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gotoacloud.top/gtsqgqpzqr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.quarkkingdee.top/gttjceiwor.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zdqjudy.top/gtyshmwbrc.html

[D05] 访问与修改元素
来源：http://hz.sufxvd.cn/gtvtxgfniv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnxiangtu.top/gtchcsxovc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xylfe.cn/gtwaspsuii.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xuetiantiany.cn/gtezznzloq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jlsjyb.cn/gtthfthpyp.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.kuanghao11.cn/gtxbmlhbsm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.pycfn.com/gtlaqafmvb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gtuzrbuxjy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.316326.xyz/gtsrdtwwic.html

[D06] 数组长度
来源：http://hz.52xcode.cn/gtulexvyzq.html

Py:   len(arr)
来源：http://hz.mhx1999.top/gtoouoplfu.html

PHP:  count($arr);
来源：http://hz.yanxiufei.cn/gtrhqmelty.html

JS:   arr.length
来源：http://hz.ydjk.org.cn/gtpctgdbks.html

TS:   arr.length
来源：http://hz.havefunace.top/gtusdiyaxc.html

Java: list.size();
来源：http://hz.hywenlv.cn/gthyaeirxl.html

Go:   len(arr)
来源：http://hz.gzhubu.top/gttaaqrjtq.html

Ruby: arr.length; arr.size
来源：http://hz.zhengqikj.top/gtohkdwyvn.html

C#:   list.Count;
来源：http://hz.dashuyun.cn/gtppdszbes.html

[D07] 切片 / 取子数组
来源：http://hz.hywenlv.cn/gtrtvqxtjs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhijiandao.cn/gtvcuqwnxl.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yj20258888.top/gtnfkqwagb.html

JS:   arr.slice(1, 4);
来源：http://hz.yanxiufei.cn/gtgvunwcig.html

TS:   arr.slice(1, 4);
来源：http://hz.yvedp.cn/gtmmzsdhxm.html

Java: list.subList(1, 4);
来源：http://hz.hongshengwenyu.top/gtcrdmlufd.html

Go:   arr[1:4]
来源：http://hz.cqqwz.cn/gttqyfajar.html

Ruby: arr[1, 3]
来源：http://hz.cashguo.top/gtvdidjpvd.html

C#:   list.GetRange(1, 3);
来源：http://hz.wangdashe.top/gtytcijcmi.html

[D08] 合并两个数组
来源：http://hz.cashguo.top/gtqdyyyhzb.html

Py:   a + b;  a.extend(b)
来源：http://hz.nanxinkj.top/gtdoinfiby.html

PHP:  array_merge($a, $b);
来源：http://hz.ydzc1.top/gtrkoikurv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shanyushiyangkeji.top/gtofhxdtii.html

TS:   [...a, ...b];
来源：http://hz.aizwys.cn/gtdpjsuybt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.dashuyun.cn/gtdgfswnel.html

Go:   append(a, b...)
来源：http://hz.fengsongda.top/gtjxubowab.html

Ruby: a + b;  a.concat(b)
来源：http://hz.bjfxy.top/gtpgaolxzb.html

C#:   a.Concat(b).ToList()
来源：http://hz.yueranfly.top/gtbmihozdd.html

[D09] 排序（升序）
来源：http://hz.smart0.xyz/gtwcwhpwsf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.9152youxi.cn/gtgzbzxuim.html

PHP:  sort($arr);
来源：http://hz.jqgufenzy.top/gtzoomcnig.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.daxiang520.top/gtekamnjge.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.svipenyu.cn/gtwpyenrkp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shanyushiyangtech.top/gthyvsfveg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hongshengwenyu.top/gtzafemltu.html

Ruby: arr.sort
来源：http://hz.jinqigufen.top/gtwtnhfqfu.html

C#:   list.Sort();
来源：http://hz.ppjwa.cn/gtezzqdpcy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hnxiangtu.top/gtahwiwagn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.daxiang520.top/gtvhhlaqfh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigufen.top/gtftxrwenm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gtxwevooje.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hammf.cn/gteuzvanto.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.316326.xyz/gtqkesuqvz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cdnleiting.top/gtpqiemxlt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.fzhhl.top/gttzrsizqs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhixingplan.top/gtwasmbpmx.html

[D11] 反转数组
来源：http://hz.mhx1999.top/gtatzojigd.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.c1oappe.top/gtnqcnxkdl.html

PHP:  array_reverse($arr);
来源：http://hz.pycfn.com/gtvqasgvwg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.pycfn.com/gteuipsrhb.html

TS:   [...arr].reverse();
来源：http://hz.nanxinkj.top/gtmdgwfiit.html

Java: Collections.reverse(list);
来源：http://hz.iojbl.cn/gtpusdngzr.html

Go:   slices.Reverse(arr)
来源：http://hz.nwbrower.top/gtmgrvzvgn.html

Ruby: arr.reverse
来源：http://hz.xziqi.cn/gtnfwahgsm.html

C#:   list.Reverse();
来源：http://hz.chenjidiqi.icu/gtzablrltj.html

[D12] 查找元素下标
来源：http://hz.yj202588.top/gtouzsmagn.html

Py:   arr.index(x);  x in arr
来源：http://hz.hywenlv.cn/gtiferejbw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.daxiang520.top/gtiswpztbd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gogol.net.cn/gtspolevfl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fzhhl.top/gtzidzsqze.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jlsjyb.cn/gtqpurueha.html

Go:   slices.Index(arr, x)
来源：http://hz.fzhhl.top/gtupzmjuhl.html

Ruby: arr.index(x)
来源：http://hz.nanxinkj.top/gtpeiksxmw.html

C#:   list.IndexOf(x);
来源：http://hz.jqgfzy.top/gtjibogpme.html

[D13] 过滤（保留满足条件的）
来源：http://hz.316326.xyz/gtuymxhhms.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinyuanbaomall.cn/gtxwxpuvjv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hnxiangtu.top/gtfbgbccdv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtqjftypxt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shuidangran.top/gtxhcbwvrn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ppjwa.cn/gtijbjjonw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yuxming.cn/gttlxhaxlb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yuanzhike.top/gtstxwszcp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jqgufenzy.top/gtluojbbry.html

[D14] 映射转换（每个元素变形）
来源：http://hz.chenlongwang.top/gtdzfrtioz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.chenjidiqi.icu/gtubffjjlw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhengqikj.top/gtidrqiurj.html

JS:   arr.map(x => x * 2)
来源：http://hz.iojbl.cn/gtssdptabr.html

TS:   arr.map(x => x * 2)
来源：http://hz.wangdashe.top/gtsnlsened.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tianlin.xyz/gtiheoecnu.html

Go:   // 手写循环
来源：http://hz.jyoumei.cn/gthzbooyga.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yueranfly.top/gtaajaefzy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yj20258888.top/gtoevdvirh.html

[D15] 去重
来源：http://hz.daria6918.cn/gtqqyizthw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.andypj.xyz/gtxjlhygej.html

PHP:  array_unique($arr);
来源：http://hz.kuanghao11.cn/gttroxbfop.html

JS:   [...new Set(arr)]
来源：http://hz.ehwqpu.com/gtwfuezecw.html

TS:   [...new Set(arr)]
来源：http://hz.52xcode.cn/gtgpwtscjn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.gzhubu.top/gtoaarhany.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hongshengwenyu.top/gtqyhiudis.html

Ruby: arr.uniq
来源：http://hz.yj20258.top/gtlobfucuj.html

C#:   list.Distinct().ToList()
来源：http://hz.guannengcc.top/gtqztnluwy.html

[D16] 求和与平均值
来源：http://hz.hammf.cn/gtelsvpojm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.dianchejie.cn/gtabiysrtx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yangfankeji.com/gtcyuujsun.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ehwqpu.com/gthuyddwwm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tian-w.cn/gtqamaumti.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.svipenyu.cn/gtjwouisvc.html

Go:   // 手写循环累加
来源：http://hz.nanxinkj.top/gtyrfeftqy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jianghu66.top/gthlunjwfq.html

C#:   list.Sum();  list.Average()
来源：http://hz.0kj1m.cn/gtvfblnrfu.html

[D17] 最大值与最小值
来源：http://hz.fzhhl.top/gtfqgomifr.html

Py:   max(arr);  min(arr)
来源：http://hz.shanyushiyangtech.top/gtbonvhcbk.html

PHP:  max($arr);  min($arr);
来源：http://hz.aizwys.cn/gtqumghrgw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.chenjidiqi.icu/gtzmtbzjhk.html

TS:   Math.max(...arr);
来源：http://hz.cheryme.top/gtprckcvqj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jlsjyb.cn/gtlfbayfdu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj20258.top/gtcqqdrlaq.html

Ruby: arr.max;  arr.min
来源：http://hz.yvedp.cn/gtzztzcthk.html

C#:   list.Max();  list.Min()
来源：http://hz.9152youxi.cn/gtqzjhcbbp.html

[D18] 扁平化嵌套数组
来源：http://hz.9152youxi.cn/gtqtmnqdij.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nanxinkj.top/gtwxlsirdx.html

PHP:  array_merge(...$nested);
来源：http://hz.tanke756.top/gtpnlaudhk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.pengpengdd.cyou/gtbftqjdza.html

TS:   nested.flat();
来源：http://hz.yj202588.top/gtskdafrry.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.haohaochexian.top/gtmgsrkpbf.html

Go:   // 手写双层循环
来源：http://hz.havefunace.top/gtpekrlwlw.html

Ruby: nested.flatten
来源：http://hz.aizwys.cn/gtbjrddjxp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shanyushiyangtech.top/gtsodmjkoz.html

[D19] 按字段分组
来源：http://hz.xylfe.cn/gttevniine.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yongpay.top/gtlcvbealj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jiagoushi.top/gtlopgucuv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jlsjyb.cn/gtzxjcoyfz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhijiandao.cn/gtfjnqhlwg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ppjwa.cn/gtgtxunxvb.html

Go:   // 手写 map[string][]T
来源：http://hz.yueranfly.top/gtexxqifpe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.mhx1999.top/gtpcjbnode.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cheryme.top/gtlzcberes.html

[D20] 统计每个元素出现次数
来源：http://hz.yuanzhike.top/gtsulzatqz.html

Py:   Counter(arr)
来源：http://hz.jiagoushi.top/gtyfevfyey.html

PHP:  array_count_values($arr);
来源：http://hz.zhoulong.xyz/gtctjupojz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fengsongda.top/gtytgweogk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hongshengwenyu.top/gtawffudoo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj202588.top/gtzepdggzs.html

Go:   // 手写 map[T]int
来源：http://hz.jyoumei.cn/gttsrszdju.html

Ruby: arr.tally
来源：http://hz.snrcjt.cn/gtlsktbpwe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.redwolf501.top/gtqkocskub.html

[D21] 判断是否包含某元素
来源：http://hz.nanxinkj.top/gtczgvvphe.html

Py:   x in arr
来源：http://hz.jinyuanbaomall.cn/gtrpzafoxb.html


<!-- 参考信息 -->