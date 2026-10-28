代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shangyingyoupin.top/gtldxtyfct.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.gotoacloud.top/gtwpwvxnoc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dianchejie.cn/gtzdynwzoo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xinyue.icu/gtdzjhiqux.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hysaishi.cn/gtpegwrusd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.smart0.xyz/gtrbgpyyzc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cdnleiting.top/gtgxagphof.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xinyue.icu/gtncnsadul.html

[C10] 变量作用域
来源：http://hz.chenjidiqi.icu/gteignovzb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xinyue.icu/gtzzuijikl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yangfankeji.com/gtyjinttzx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shangyingyoupin.top/gtpuqxpnrh.html

TS:   同 JS
来源：http://hz.feifeiyinyue.top/gtmkrzrzdi.html

Java: 方法内为块级作用域
来源：http://hz.fengsongda.top/gtafuzfdlm.html

Go:   花括号块级作用域
来源：http://hz.jlsjyb.cn/gtatobqxpq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yonumen.top/gtzehdwuiu.html

C#:   块级作用域
来源：http://hz.zdqjudy.top/gtibxrtask.html

[C11] 模块导入与导出
来源：http://hz.guowangkeji.top/gtvbyohitt.html

Py:   from module import func
来源：http://hz.haohaochexian.top/gtoxfiqsrh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.chenzaomai.com/gtpbthrtti.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.vqdsnc.cn/gttwvwzhvp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xziqi.cn/gtjvujolil.html

Java: import java.util.List;
来源：http://hz.daxiang520.top/gtppqwzhty.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.c1oappe.top/gtpuejnhcy.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.chenlongwang.top/gtqamsbrqs.html

C#:   using System.Text;
来源：http://hz.ehwqpu.com/gtlzxhpvax.html

[C12] 立即执行函数 IIFE
来源：http://hz.xuetiantiany.cn/gtfjjrqwei.html

Py:   (lambda: print("run"))()
来源：http://hz.zhiwuduotai.top/gtqtnmtwnz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.cqqwz.cn/gthkjffbzx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.dianchejie.cn/gtievldevu.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinghuilouyu.cn/gtrqwevcxe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.birdmap.top/gtgipzbcfa.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ybcxt.top/gtzhkgljvl.html

Ruby: -> { puts "run" }.call
来源：http://hz.chenzaomai.com/gtgsbfydoo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yueranfly.top/gtdyacmdqu.html

[C13] 类型声明 / 类型注解
来源：http://hz.chenlongwang.top/gteibjettt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.haohaochexian.top/gtvsvdrsty.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aibaodan.cn/gtxcmxsucc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xylfe.cn/gtgatgrtmi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhengqikj.top/gtmanlmruk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtkeoknxkb.html

Go:   func add(a, b int) int
来源：http://hz.sysykeji.top/gtogtperle.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yueranfly.top/gtkoknquun.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj202588.top/gtiybmxzxx.html

[C14] 泛型函数
来源：http://hz.hfpthk.cn/gtrtrfudal.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.quarkkingdee.top/gtzobliwxa.html

PHP:  // 无泛型
来源：http://hz.snrcjt.cn/gtooafvtdc.html

JS:   // 无泛型
来源：http://hz.sufxvd.cn/gtzbbtjqli.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hfpthk.cn/gtwolqemlk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hongshengwenyu.top/gttwcdkwni.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sufxvd.cn/gtbrstqinf.html

Ruby: # 无泛型
来源：http://hz.cheryme.top/gtohnrffsi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.9152youxi.cn/gtscgoqsgx.html

[C15] 解构 / 展开参数
来源：http://hz.ywan-chungtsiang.top/gthhicznhj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.fengsongda.top/gtxndsukui.html

PHP:  [$a, $b] = $pair;
来源：http://hz.tianlin.xyz/gtagkrcqwl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.0kj1m.cn/gtjdafjkvp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ppjwa.cn/gtobebzjjr.html

Java: // 无解构
来源：http://hz.xuanzx.com/gtznbusnqt.html

Go:   // 无解构
来源：http://hz.redwolf501.top/gturotacwn.html

Ruby: a, b = pair
来源：http://hz.yj20258.top/gtufqdaggd.html

C#:   var (a, b) = pair;
来源：http://hz.jianghu66.top/gtirqluobq.html

[C16] 函数 / 方法重载
来源：http://hz.yongpay.top/gtmcpmdwqp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shanyushiyangtech.top/gtowrsylax.html

PHP:  // 无重载
来源：http://hz.xuetiantiany.cn/gtdbmvkiie.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ybcxt.top/gtwjgkudni.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shanyushiyangtech.top/gtjdrinyxu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenjidiqi.icu/gtamnujoox.html

Go:   // 无重载：用不同函数名
来源：http://hz.cashguo.top/gttgaqdgjv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.tanke756.top/gtklnnppri.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhiwuduotai.top/gtltbnirvg.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtqlwoqmlo.html

D. 数组 / 列表 / 集合
来源：http://hz.daxiang520.top/gtxmwkeotl.html

================================================================================
来源：http://hz.zycfv.cn/gttxukynha.html

[D01] 创建数组 / 列表
来源：http://hz.shangyingyoupin.top/gtizbzlfjo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhixingplan.top/gtdyefrsqe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.cheryme.top/gthgohbgxk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yangfankeji.com/gtwzhebnxw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hywenlv.cn/gtbffgpfod.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yvedp.cn/gtbafuikjw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.guowangkeji.top/gtbmnpmiix.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jqgfzy.top/gtjznvyggr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yuxming.cn/gtfdpxmpch.html

[D02] 追加元素到末尾
来源：http://hz.ehwqpu.com/gttznilnxy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jinqigfzy.top/gtmknlpckv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.fengsongda.top/gtkixrwdyh.html

JS:   arr.push(4);
来源：http://hz.wangdashe.top/gtvrndurda.html

TS:   arr.push(4);
来源：http://hz.yvedp.cn/gtufbudlsb.html

Java: list.add(4);
来源：http://hz.ybcxt.top/gtydqmstai.html

Go:   arr = append(arr, 4)
来源：http://hz.zhiwuduotai.top/gtektszyhd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jianghu66.top/gtagreomsz.html

C#:   list.Add(4);
来源：http://hz.zycfv.cn/gtxwxysfks.html

[D03] 在指定位置插入元素
来源：http://hz.quarkkingdee.top/gtxswohhdr.html

Py:   arr.insert(0, 0)
来源：http://hz.0kj1m.cn/gtbnyyjbec.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.guowangkeji.top/gtejumikwq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ywan-chungtsiang.top/gtdecoyplp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hnqzz.top/gtasjyfarq.html

Java: list.add(0, 0);
来源：http://hz.nanxuanxn.top/gtjwowgkqx.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.fzhhl.top/gtgkucijqy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.dianchejie.cn/gtltauwxhq.html

C#:   list.Insert(0, 0);
来源：http://hz.shangyingyoupin.top/gtxiuwrkly.html

[D04] 删除元素
来源：http://hz.aizwys.cn/gtogxabdkc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yangfankeji.com/gtuyhmtvlf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnxiangtu.top/gtgzvhlsws.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zycfv.cn/gtcpghlfqn.html

TS:   arr.splice(0, 1);
来源：http://hz.yvedp.cn/gtrzoubmfr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shangyingyoupin.top/gtqofiikzd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xziqi.cn/gtkfcvuiuu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shzxlz.cn/gttoihouyl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.daxiang520.top/gtbuabeiku.html

[D05] 访问与修改元素
来源：http://hz.tian-w.cn/gtimjduuog.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtnxalyihp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.tianlin.xyz/gtpsjgezed.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jiagoushi.top/gtmofspfoe.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zycfv.cn/gtzwjjfnym.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinqigufen.top/gtymvsqijb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.wangdashe.top/gtjtrcjvae.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.svipenyu.cn/gtccfygngh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jyoumei.cn/gtbbyhunmx.html

[D06] 数组长度
来源：http://hz.shzxlz.cn/gtifjphmhg.html

Py:   len(arr)
来源：http://hz.ivvv.top/gtderdikax.html

PHP:  count($arr);
来源：http://hz.daxiang520.top/gtphvvcvqy.html

JS:   arr.length
来源：http://hz.shzxlz.cn/gtjwzxatwx.html

TS:   arr.length
来源：http://hz.zhengqikj.top/gtjplgnwwg.html

Java: list.size();
来源：http://hz.shuidangran.top/gtkvdacefb.html

Go:   len(arr)
来源：http://hz.bjfxy.top/gtwilsxlro.html

Ruby: arr.length; arr.size
来源：http://hz.jqgufenzy.top/gthdjgmqxo.html

C#:   list.Count;
来源：http://hz.jlsjyb.cn/gtjgahuuvu.html

[D07] 切片 / 取子数组
来源：http://hz.aibaodan.cn/gtsjttmnmi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yangfankeji.com/gtyxqejbga.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.tanke756.top/gtoonbiqfl.html

JS:   arr.slice(1, 4);
来源：http://hz.gaohongyu789.top/gtobmidzlw.html

TS:   arr.slice(1, 4);
来源：http://hz.fengsongda.top/gtkwoujfbg.html

Java: list.subList(1, 4);
来源：http://hz.ywan-chungtsiang.top/gtnndefnpl.html

Go:   arr[1:4]
来源：http://hz.zhijiandao.cn/gthffomser.html

Ruby: arr[1, 3]
来源：http://hz.yuxming.cn/gtmnfzqtck.html

C#:   list.GetRange(1, 3);
来源：http://hz.gogol.net.cn/gtqsnvtqzy.html

[D08] 合并两个数组
来源：http://hz.sysykeji.top/gtwiadogtu.html

Py:   a + b;  a.extend(b)
来源：http://hz.xinyue.icu/gtpnqstdvy.html

PHP:  array_merge($a, $b);
来源：http://hz.xylfe.cn/gtfnjtvnwu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yj20258888.top/gtwwsaqvax.html

TS:   [...a, ...b];
来源：http://hz.wangdashe.top/gtiphioxoe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.aibaodan.cn/gtoxquwrmj.html

Go:   append(a, b...)
来源：http://hz.smart0.xyz/gtiajzrrni.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nanxinkj.top/gtnotwipvg.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenlongwang.top/gtioazicfy.html

[D09] 排序（升序）
来源：http://hz.birdmap.top/gtxsvwdipm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gzhubu.top/gtzmaummgn.html

PHP:  sort($arr);
来源：http://hz.shzxlz.cn/gtgfktnosn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ywan-chungtsiang.top/gtcfgdmjtx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhengqikj.top/gtstapmueh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.tianlin.xyz/gtccbgmldq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jyoumei.cn/gtbsfnmmsj.html

Ruby: arr.sort
来源：http://hz.shzxlz.cn/gtevqwtztv.html

C#:   list.Sort();
来源：http://hz.wangdashe.top/gtxxluljju.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hysaishi.cn/gtsagyewlr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenlongwang.top/gtfaiynrlh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydjk.org.cn/gtffxntkix.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenjidiqi.icu/gtouslzgby.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aizwys.cn/gtipxmhjbp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.0kj1m.cn/gtawwbiigx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yonumen.top/gtdhybvoqw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj20258888.top/gtoacsdxfl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ivvv.top/gtwnvspsnn.html

[D11] 反转数组
来源：http://hz.xylfe.cn/gtwbsgntnx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hnqzz.top/gtlxtevlml.html

PHP:  array_reverse($arr);
来源：http://hz.9152youxi.cn/gtlyrlyhfr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xziqi.cn/gtgmhmhokp.html

TS:   [...arr].reverse();
来源：http://hz.sufxvd.cn/gtlqgizpze.html

Java: Collections.reverse(list);
来源：http://hz.cqqwz.cn/gtrhqbfgtc.html

Go:   slices.Reverse(arr)
来源：http://hz.sysykeji.top/gtthpcnxqk.html

Ruby: arr.reverse
来源：http://hz.ywan-chungtsiang.top/gtuyeyatpg.html

C#:   list.Reverse();
来源：http://hz.sweek.top/gtpiaxrnip.html

[D12] 查找元素下标
来源：http://hz.yj202588.top/gtfblwtxea.html

Py:   arr.index(x);  x in arr
来源：http://hz.ppjwa.cn/gtshdmzfnx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yuanzhike.top/gtjykgrgmz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hammf.cn/gtdtcvgbjb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigufen.top/gttdlahptd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.mhx1999.top/gtvyhelhqd.html

Go:   slices.Index(arr, x)
来源：http://hz.redwolf501.top/gtvtpbsyad.html

Ruby: arr.index(x)
来源：http://hz.zhiwuduotai.top/gtymorxkqw.html

C#:   list.IndexOf(x);
来源：http://hz.c1oappe.top/gtaikpeisw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yj20258888.top/gtdsczbrtx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shanyushiyangkeji.top/gtrqcbntnj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenjidiqi.icu/gtdgnfcyxk.html

JS:   arr.filter(x => x > 3)
来源：http://hz.aizwys.cn/gtmlcjerlm.html

TS:   arr.filter(x => x > 3)
来源：http://hz.wangdashe.top/gtjhggvfmp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shanyushiyangtech.top/gtcygsvron.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258.top/gtukwogndv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhengqikj.top/gtfqxsdthi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ydjk.org.cn/gtmyrwwdev.html

[D14] 映射转换（每个元素变形）
来源：http://hz.birdmap.top/gtgloaojgr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.aibaodan.cn/gtxzvawppo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.haohaochexian.top/gtfdsxkgnp.html

JS:   arr.map(x => x * 2)
来源：http://hz.gzhubu.top/gtrotcwxud.html

TS:   arr.map(x => x * 2)
来源：http://hz.dianchejie.cn/gtwhhzzpvy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yj20258.top/gtqlwwprqv.html

Go:   // 手写循环
来源：http://hz.fzhhl.top/gtfstpbwvo.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.tian-w.cn/gtrwwqfcbs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhengqikj.top/gtrmywuhwf.html

[D15] 去重
来源：http://hz.ywan-chungtsiang.top/gtuxkusznp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nwbrower.top/gtibloiweb.html

PHP:  array_unique($arr);
来源：http://hz.daxiang520.top/gtawymtplw.html

JS:   [...new Set(arr)]
来源：http://hz.svipenyu.cn/gtmwmovpvy.html

TS:   [...new Set(arr)]
来源：http://hz.ydzc1.top/gtyhixuxen.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ydzc1.top/gtplfldswu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.smart0.xyz/gtxoojelkz.html

Ruby: arr.uniq
来源：http://hz.cqqwz.cn/gtqbkwjobn.html

C#:   list.Distinct().ToList()
来源：http://hz.yangfankeji.com/gtjduuaiti.html

[D16] 求和与平均值
来源：http://hz.hywenlv.cn/gtxegvvoac.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.guannengcc.top/gtfkojzljr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ydjk.org.cn/gtvwzjgrko.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aizwys.cn/gtkepakcyr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258888.top/gtqwxhlqaq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ywan-chungtsiang.top/gtyiomuxga.html

Go:   // 手写循环累加
来源：http://hz.yj20258.top/gtohzhfvqo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ydjk.org.cn/gtttokivok.html

C#:   list.Sum();  list.Average()
来源：http://hz.yueranfly.top/gtgzyybkqi.html

[D17] 最大值与最小值
来源：http://hz.shanyushiyangkeji.top/gtbextakmj.html

Py:   max(arr);  min(arr)
来源：http://hz.hfpthk.cn/gtswigmdss.html

PHP:  max($arr);  min($arr);
来源：http://hz.tianlin.xyz/gtuuplnnzj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.chenzaomai.com/gtobfmahcr.html

TS:   Math.max(...arr);
来源：http://hz.nanxinkj.top/gtebpfujsk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xingfuxueyuan.xyz/gtwdyjqdwk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yuanzhike.top/gtmxddamyk.html

Ruby: arr.max;  arr.min
来源：http://hz.gaohongyu789.top/gtouhmvfsu.html

C#:   list.Max();  list.Min()
来源：http://hz.ppjwa.cn/gtfonuorzr.html

[D18] 扁平化嵌套数组
来源：http://hz.9152youxi.cn/gtlrtcpbjx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sysykeji.top/gteandkbyp.html

PHP:  array_merge(...$nested);
来源：http://hz.jinqigfzy.top/gtvohxkdlm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.gogol.net.cn/gtysvnratp.html

TS:   nested.flat();
来源：http://hz.52xcode.cn/gtuztyouqq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ppjwa.cn/gtjjemxfre.html

Go:   // 手写双层循环
来源：http://hz.feifeiyinyue.top/gtwpyxywsc.html

Ruby: nested.flatten
来源：http://hz.shzxlz.cn/gttlkwrpvw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinyuanbaomall.cn/gtbzqznrhb.html

[D19] 按字段分组
来源：http://hz.daria6918.cn/gtqgjafhzi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cdnleiting.top/gtnmsbknfm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ybcxt.top/gtowvzmizj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hysaishi.cn/gtfkrjnguu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.nwbrower.top/gtcmbznqmb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhixingplan.top/gttcauweou.html

Go:   // 手写 map[string][]T
来源：http://hz.meibo888.top/gtesnlzpsb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.aibaodan.cn/gtmhcqtnxs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.smart0.xyz/gteviousto.html

[D20] 统计每个元素出现次数
来源：http://hz.c1oappe.top/gtnrvzosgu.html

Py:   Counter(arr)
来源：http://hz.gaohongyu789.top/gtbxjlpnum.html

PHP:  array_count_values($arr);
来源：http://hz.yanxiufei.cn/gtczpqqtut.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gtcfufdour.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fzhhl.top/gtdmknmgob.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tianlin.xyz/gtvabstecx.html

Go:   // 手写 map[T]int
来源：http://hz.wangdashe.top/gtqnpmqsou.html

Ruby: arr.tally
来源：http://hz.chenlongwang.top/gtjnszeotw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhengqikj.top/gthheuhxhd.html

[D21] 判断是否包含某元素
来源：http://hz.jqgfzy.top/gtpwinnsnt.html

Py:   x in arr
来源：http://hz.hysaishi.cn/gtmkhvirli.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hnqzz.top/gtpopytuju.html

JS:   arr.includes(x)
来源：http://hz.shzxlz.cn/gtqxyaouib.html

TS:   arr.includes(x)
来源：http://hz.hongshengwenyu.top/gtqjwxzajr.html

Java: list.contains(x)
来源：http://hz.hnqzz.top/gtndrykwmv.html

Go:   slices.Contains(arr, x)
来源：http://hz.ehwqpu.com/gtigidydlj.html

Ruby: arr.include?(x)
来源：http://hz.guowangkeji.top/gtvgzgigvl.html

C#:   list.Contains(x)
来源：http://hz.yongpay.top/gtwmssnsal.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yuanzhike.top/gtrzwiamif.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.mhx1999.top/gtoaaoxprm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.316326.xyz/gtllnurins.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.smart0.xyz/gtqyhfnpms.html

TS:   [...arr];
来源：http://hz.yj20258.top/gtrseumkuu.html

Java: new ArrayList<>(list);
来源：http://hz.ydzc1.top/gtiprcauvt.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shanyushiyangkeji.top/gttbadzthb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.fzhhl.top/gtcyweazwj.html

C#:   new List<int>(list);
来源：http://hz.sufxvd.cn/gtjoezbkaw.html

[D23] reduce 累积计算
来源：http://hz.zhongyouzk.top/gtiwkcwztl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhijiandao.cn/gtejqgmszn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj20258888.top/gteabqnbqr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hysaishi.cn/gtrnggzbfq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gotoacloud.top/gthvgkihfi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nwbrower.top/gteiyadwut.html

Go:   // 手写循环
来源：http://hz.0kj1m.cn/gtruqntxfa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ppjwa.cn/gtnuodnsrb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hnxiangtu.top/gtlzohoubg.html

[D24] 字典 / Map 基本操作
来源：http://hz.fengsongda.top/gtletqrvhf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sxryk.cn/gtvntzokhw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hfpthk.cn/gttlvawmle.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhaomingkeji.xyz/gtengcztdv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.iojbl.cn/gtwmdxoqnu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.daria6918.cn/gtuifmxrfa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jinyuanbaomall.cn/gtsguzgxxw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hfpthk.cn/gtkpqolnsi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hongshengwenyu.top/gtqwlzvemj.html

[D25] Set 集合去重与交并差
来源：http://hz.fzhhl.top/gtdqacswrw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xinyue.icu/gtyuusdrpl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jianghu66.top/gtidqziukb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cheryme.top/gtpufsevtp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xziqi.cn/gtbohtsezx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.kuanghao11.cn/gtkhiycwvy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.daria6918.cn/gtwjsqlxgu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cucudq.cn/gtgrghbkip.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.mhx1999.top/gtenxkqxqp.html

[D26] 数组转字符串
来源：http://hz.havefunace.top/gtbjhipddf.html


<!-- 参考信息 -->