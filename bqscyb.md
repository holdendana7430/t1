代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.dashuyun.cn/gtrdbfxcqi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.guannengcc.top/gtnslymegm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ehwqpu.com/gttkkqzzsj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sysykeji.top/gtduvbtbzn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ehwqpu.com/gtbpktlewe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.gzhubu.top/gtqzoshwad.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xuetiantiany.cn/gtvvjghwof.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cdnleiting.top/gtxyhdpvjn.html

[C10] 变量作用域
来源：http://hz.ppjwa.cn/gtvgfgnmyw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xingfuxueyuan.xyz/gtshohmssx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhijiandao.cn/gtdzpigsrf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cucudq.cn/gtltiqgtml.html

TS:   同 JS
来源：http://hz.cqqwz.cn/gtetqncqrv.html

Java: 方法内为块级作用域
来源：http://hz.yueranfly.top/gtyfyvbntj.html

Go:   花括号块级作用域
来源：http://hz.xingfuxueyuan.xyz/gtabwrulzc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.9152youxi.cn/gtreawdldf.html

C#:   块级作用域
来源：http://hz.chenzaomai.com/gtpjopxbhc.html

[C11] 模块导入与导出
来源：http://hz.jinyuanbaomall.cn/gtimwswpcm.html

Py:   from module import func
来源：http://hz.yuxming.cn/gtylkhwqec.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ybcxt.top/gtbslvgluk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.316326.xyz/gtzaqpqllc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xylfe.cn/gtdaxayrxs.html

Java: import java.util.List;
来源：http://hz.sxryk.cn/gtwdejwyop.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.c1oappe.top/gtdxawjqvk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yvedp.cn/gtyeviyuya.html

C#:   using System.Text;
来源：http://hz.chenlongwang.top/gtmezeqgds.html

[C12] 立即执行函数 IIFE
来源：http://hz.fzhhl.top/gtyngxiuqa.html

Py:   (lambda: print("run"))()
来源：http://hz.ydzc1.top/gtuelyuhpk.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xuanzx.com/gtpsohszfl.html

JS:   (() => { console.log("run"); })();
来源：http://hz.kuanghao11.cn/gtqvmohuqu.html

TS:   (() => { console.log("run"); })();
来源：http://hz.dianchejie.cn/gtcinynmtg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.aizwys.cn/gtorlikdmk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhiwuduotai.top/gttjqvbxpl.html

Ruby: -> { puts "run" }.call
来源：http://hz.ywan-chungtsiang.top/gtdxhxalvn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.iojbl.cn/gtjuffihlb.html

[C13] 类型声明 / 类型注解
来源：http://hz.sysykeji.top/gtwcshavul.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hysaishi.cn/gtljnkmyuc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.birdmap.top/gtvqysolgo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.havefunace.top/gtxvttkrvs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258888.top/gtvkkvqiln.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtxpxptdjr.html

Go:   func add(a, b int) int
来源：http://hz.jinghuilouyu.cn/gthdtjvwtv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xuanzx.com/gthyfwscrf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.fzhhl.top/gtnocdkwie.html

[C14] 泛型函数
来源：http://hz.xylfe.cn/gtndvrwuch.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinghuilouyu.cn/gtnmmganio.html

PHP:  // 无泛型
来源：http://hz.snrcjt.cn/gtctgvsxid.html

JS:   // 无泛型
来源：http://hz.hywenlv.cn/gtfypygpuf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinghuilouyu.cn/gtiapkdfvb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hnqzz.top/gtgrjfbkai.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sufxvd.cn/gtmarnlubc.html

Ruby: # 无泛型
来源：http://hz.pycfn.com/gtssdmiayf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.birdmap.top/gtvnxnxupt.html

[C15] 解构 / 展开参数
来源：http://hz.daria6918.cn/gtxlmlwgup.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cheryme.top/gtftscsivs.html

PHP:  [$a, $b] = $pair;
来源：http://hz.havefunace.top/gtlxbricbq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.vqdsnc.cn/gtkziiyknr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shanyushiyangtech.top/gtumtpzkey.html

Java: // 无解构
来源：http://hz.aizwys.cn/gtojipngxe.html

Go:   // 无解构
来源：http://hz.yonumen.top/gtqgzneimh.html

Ruby: a, b = pair
来源：http://hz.cashguo.top/gtultdqhmu.html

C#:   var (a, b) = pair;
来源：http://hz.nanxinkj.top/gtsseegxny.html

[C16] 函数 / 方法重载
来源：http://hz.yj202588.top/gtnygygizo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.andypj.xyz/gtmwxkawsd.html

PHP:  // 无重载
来源：http://hz.daxiang520.top/gtdjminqem.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.guowangkeji.top/gtybfpjbjt.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ivvv.top/gtdogvydxy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenlongwang.top/gtjyswqibp.html

Go:   // 无重载：用不同函数名
来源：http://hz.chenjidiqi.icu/gtgargyqtd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xingfuxueyuan.xyz/gtksbnluhg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gotoacloud.top/gtycjwonjy.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtzicolwbr.html

D. 数组 / 列表 / 集合
来源：http://hz.ppjwa.cn/gtzwdozpzp.html

================================================================================
来源：http://hz.guannengcc.top/gtfvphuolw.html

[D01] 创建数组 / 列表
来源：http://hz.sufxvd.cn/gtvofcugvm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.nwbrower.top/gtdfvphyfy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xuetiantiany.cn/gtvvhtojge.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhoulong.xyz/gtqjvtwkpd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhongyouzk.top/gtjuvaaadm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jqgufenzy.top/gtlzxztebb.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.gogol.net.cn/gttjcqsgyf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jqgfzy.top/gtobjjvufj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuetiantiany.cn/gtbwaxjlcw.html

[D02] 追加元素到末尾
来源：http://hz.dianchejie.cn/gtuwjbmpzr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ehwqpu.com/gtcwbyelva.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhengqikj.top/gtievmxfbv.html

JS:   arr.push(4);
来源：http://hz.nwbrower.top/gtuuyoygxy.html

TS:   arr.push(4);
来源：http://hz.xuanzx.com/gtnkbofiwl.html

Java: list.add(4);
来源：http://hz.xinyue.icu/gtudqpuklx.html

Go:   arr = append(arr, 4)
来源：http://hz.chenjidiqi.icu/gtaolqkdhq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.fzhhl.top/gtnuhswqyb.html

C#:   list.Add(4);
来源：http://hz.dashuyun.cn/gtdtyragcc.html

[D03] 在指定位置插入元素
来源：http://hz.jqgufenzy.top/gtlkkwdrup.html

Py:   arr.insert(0, 0)
来源：http://hz.ywan-chungtsiang.top/gtqxjwvdbu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhengqikj.top/gtcbinabyu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shanyushiyangtech.top/gtolvjvzit.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhoulong.xyz/gtflkpoosg.html

Java: list.add(0, 0);
来源：http://hz.birdmap.top/gtffusjvgv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xuetiantiany.cn/gtslywqqrp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinghuilouyu.cn/gtfddbxhjt.html

C#:   list.Insert(0, 0);
来源：http://hz.jinqigfzy.top/gtvjqxzvav.html

[D04] 删除元素
来源：http://hz.jinghuilouyu.cn/gtvmjomgen.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xuanzx.com/gtbqihypqq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zdqjudy.top/gtyrtutqkf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhixingplan.top/gtmvpwrlbj.html

TS:   arr.splice(0, 1);
来源：http://hz.shanyushiyangtech.top/gtcndsswuf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jianghu66.top/gtydqkczsp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sufxvd.cn/gtyhrqfvob.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ybcxt.top/gtpdhcggtp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ppjwa.cn/gtsmypugog.html

[D05] 访问与修改元素
来源：http://hz.zdqjudy.top/gtpkndkkzn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ppjwa.cn/gtwoqqgzge.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhaomingkeji.xyz/gtdysxwshi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gogol.net.cn/gtdhlurcos.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.chenzaomai.com/gtybxunolp.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhengqikj.top/gtstgcpqen.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gtpwpgjfap.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.c1oappe.top/gtycntrika.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinghuilouyu.cn/gtmoiniqyw.html

[D06] 数组长度
来源：http://hz.jiagoushi.top/gtyohlizpv.html

Py:   len(arr)
来源：http://hz.zdqjudy.top/gtqbsaxjqm.html

PHP:  count($arr);
来源：http://hz.hysaishi.cn/gtzfihetll.html

JS:   arr.length
来源：http://hz.ivvv.top/gttzajjjsa.html

TS:   arr.length
来源：http://hz.kuanghao11.cn/gtjtajpzas.html

Java: list.size();
来源：http://hz.iojbl.cn/gtbwcwwxxg.html

Go:   len(arr)
来源：http://hz.jqgufenzy.top/gtkalaekqo.html

Ruby: arr.length; arr.size
来源：http://hz.wangdashe.top/gtslsnkipd.html

C#:   list.Count;
来源：http://hz.svipenyu.cn/gttetowvwg.html

[D07] 切片 / 取子数组
来源：http://hz.shanyushiyangtech.top/gtbrnqulhg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.meibo888.top/gtnkwsswtn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gogol.net.cn/gtsabrjbcu.html

JS:   arr.slice(1, 4);
来源：http://hz.tanke756.top/gtcvncgehs.html

TS:   arr.slice(1, 4);
来源：http://hz.xziqi.cn/gtmysvxhtd.html

Java: list.subList(1, 4);
来源：http://hz.0kj1m.cn/gthshichix.html

Go:   arr[1:4]
来源：http://hz.gotoacloud.top/gtyuzqhotb.html

Ruby: arr[1, 3]
来源：http://hz.svipenyu.cn/gtwquqmwtg.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhixingplan.top/gtxoljsxea.html

[D08] 合并两个数组
来源：http://hz.gotoacloud.top/gttqfpeaxf.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhengqikj.top/gtpbrwuepk.html

PHP:  array_merge($a, $b);
来源：http://hz.zhengqikj.top/gtocrkrmsm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ybcxt.top/gtupeczhsz.html

TS:   [...a, ...b];
来源：http://hz.nanxuanxn.top/gtedwuirhv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yuanzhike.top/gtinnotlof.html

Go:   append(a, b...)
来源：http://hz.yuxming.cn/gttomdufqp.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yueranfly.top/gtbxbcrvei.html

C#:   a.Concat(b).ToList()
来源：http://hz.fengsongda.top/gtirdifdwl.html

[D09] 排序（升序）
来源：http://hz.gzhubu.top/gtlipzplea.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.andypj.xyz/gtocaruirp.html

PHP:  sort($arr);
来源：http://hz.yanxiufei.cn/gtgqojwkgu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cqqwz.cn/gtifsdwpva.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cqqwz.cn/gtveoezgyf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cqqwz.cn/gtmzobiejz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xinyue.icu/gtkeqzjepe.html

Ruby: arr.sort
来源：http://hz.ywan-chungtsiang.top/gtidwlmgir.html

C#:   list.Sort();
来源：http://hz.jinqigufen.top/gthvfzhaet.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.quarkkingdee.top/gtbivhwilo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sufxvd.cn/gtjmiwydiu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gaohongyu789.top/gtqtyrknkq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sweek.top/gthkbfzopd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gaohongyu789.top/gtzsofeeid.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shzxlz.cn/gtdykfmoux.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cashguo.top/gtcyusybqp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.daria6918.cn/gtiqlzuogw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinyuanbaomall.cn/gtfujlwvqs.html

[D11] 反转数组
来源：http://hz.chenzaomai.com/gtmixcgrjg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ehwqpu.com/gtwmaenxnd.html

PHP:  array_reverse($arr);
来源：http://hz.jinqigfzy.top/gtcdnehabf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yueranfly.top/gtvlgpqods.html

TS:   [...arr].reverse();
来源：http://hz.ybcxt.top/gtsmkcqbty.html

Java: Collections.reverse(list);
来源：http://hz.pycfn.com/gttwezatxs.html

Go:   slices.Reverse(arr)
来源：http://hz.xziqi.cn/gttkyevyua.html

Ruby: arr.reverse
来源：http://hz.52xcode.cn/gtdghsbdao.html

C#:   list.Reverse();
来源：http://hz.52xcode.cn/gtnxxgxsro.html

[D12] 查找元素下标
来源：http://hz.zhoulong.xyz/gtrhcheate.html

Py:   arr.index(x);  x in arr
来源：http://hz.hammf.cn/gtbqrpjdqj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xuanzx.com/gtyhbajyna.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangkeji.top/gtjblgqkiw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pycfn.com/gtetzspdxn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cashguo.top/gtpgfumyap.html

Go:   slices.Index(arr, x)
来源：http://hz.yueranfly.top/gtkvtvjwkx.html

Ruby: arr.index(x)
来源：http://hz.hysaishi.cn/gtexjpjemu.html

C#:   list.IndexOf(x);
来源：http://hz.ydjk.org.cn/gtzowzmntx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jlsjyb.cn/gtcgzjwiqv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cheryme.top/gtnarcjtbk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gotoacloud.top/gtontvjuex.html

JS:   arr.filter(x => x > 3)
来源：http://hz.quarkkingdee.top/gtdmjjuhbu.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ivvv.top/gtrcxjumlt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xuanzx.com/gtupjemgqa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.meibo888.top/gtcwbmolvg.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhongyouzk.top/gtifznzevm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinyuanbaomall.cn/gtgxvzfbav.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sweek.top/gtaxuffycz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.guowangkeji.top/gturfzodkr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yueranfly.top/gtbobetsxm.html

JS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangtech.top/gtcfnahbdl.html

TS:   arr.map(x => x * 2)
来源：http://hz.sweek.top/gtcpboruqr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xuanzx.com/gtzsncwmdy.html

Go:   // 手写循环
来源：http://hz.yongpay.top/gtgcsyqshc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhengqikj.top/gtpiyoqozw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gaohongyu789.top/gtzfyuykcu.html

[D15] 去重
来源：http://hz.shanyushiyangtech.top/gtqnpbkdaj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cheryme.top/gtvceaijcw.html

PHP:  array_unique($arr);
来源：http://hz.pycfn.com/gtasagnsqu.html

JS:   [...new Set(arr)]
来源：http://hz.zycfv.cn/gtjgwoqabf.html

TS:   [...new Set(arr)]
来源：http://hz.yonumen.top/gtvkupixiw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.kuanghao11.cn/gtiocktxyd.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yanxiufei.cn/gtntxuhcpk.html

Ruby: arr.uniq
来源：http://hz.jqgfzy.top/gtgfrqmgxu.html

C#:   list.Distinct().ToList()
来源：http://hz.aizwys.cn/gtmtretxkz.html

[D16] 求和与平均值
来源：http://hz.xingfuxueyuan.xyz/gtymggbrui.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhoulong.xyz/gtsoorgebq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinqigufen.top/gtzvcmclcv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daria6918.cn/gtphuqjmej.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cqqwz.cn/gtwtauwjqc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hongshengwenyu.top/gtcqmsqpyt.html

Go:   // 手写循环累加
来源：http://hz.dianchejie.cn/gtevqcyjza.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yuxming.cn/gtoymrtfcy.html

C#:   list.Sum();  list.Average()
来源：http://hz.gaohongyu789.top/gtxojbaids.html

[D17] 最大值与最小值
来源：http://hz.chenlongwang.top/gtdjogopph.html

Py:   max(arr);  min(arr)
来源：http://hz.shanyushiyangtech.top/gtzeenhmux.html

PHP:  max($arr);  min($arr);
来源：http://hz.iojbl.cn/gtzijvufwx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dianchejie.cn/gtxchbiuwt.html

TS:   Math.max(...arr);
来源：http://hz.yuxming.cn/gtpexqfivf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jiagoushi.top/gtzpyyvrmg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shangyingyoupin.top/gtcwbckfnk.html

Ruby: arr.max;  arr.min
来源：http://hz.52xcode.cn/gtsuzimtwv.html

C#:   list.Max();  list.Min()
来源：http://hz.meibo888.top/gtvyndhihr.html

[D18] 扁平化嵌套数组
来源：http://hz.dashuyun.cn/gtnhjmcnib.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenlongwang.top/gtvzkunmmz.html

PHP:  array_merge(...$nested);
来源：http://hz.tanke756.top/gtpynphgac.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guannengcc.top/gthqoyqffy.html

TS:   nested.flat();
来源：http://hz.aizwys.cn/gteqcdxvcc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ydjk.org.cn/gtgfniqzbd.html

Go:   // 手写双层循环
来源：http://hz.daxiang520.top/gtqaquacyv.html

Ruby: nested.flatten
来源：http://hz.9152youxi.cn/gtxxrzqdst.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.feifeiyinyue.top/gtowdircyx.html

[D19] 按字段分组
来源：http://hz.hnqzz.top/gtltppdiws.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hammf.cn/gtyqdkoclj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.gogol.net.cn/gthnfzgblw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zdqjudy.top/gtzlwltdtg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.haohaochexian.top/gtoppzplbr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhengqikj.top/gtwfqyyjly.html

Go:   // 手写 map[string][]T
来源：http://hz.chenzaomai.com/gtjkrkrkxu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.chenzaomai.com/gtepxxmoey.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.fengsongda.top/gtgujoyosy.html

[D20] 统计每个元素出现次数
来源：http://hz.jianghu66.top/gtuwzxrguw.html

Py:   Counter(arr)
来源：http://hz.ivvv.top/gtworphnyz.html

PHP:  array_count_values($arr);
来源：http://hz.kuanghao11.cn/gtcevjxmdc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sufxvd.cn/gthtommasd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinghuilouyu.cn/gtchkilckt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhongyouzk.top/gtbpgnxjmk.html

Go:   // 手写 map[T]int
来源：http://hz.yj202588.top/gthhnthqyb.html

Ruby: arr.tally
来源：http://hz.smart0.xyz/gtiqnlojbp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.shzxlz.cn/gtjhdbqcls.html

[D21] 判断是否包含某元素
来源：http://hz.birdmap.top/gtfjfwklzc.html

Py:   x in arr
来源：http://hz.yangfankeji.com/gtbagxtlco.html

PHP:  in_array($x, $arr, true);
来源：http://hz.c1oappe.top/gtngurxmzj.html

JS:   arr.includes(x)
来源：http://hz.jinqigufen.top/gtukofiber.html

TS:   arr.includes(x)
来源：http://hz.jyoumei.cn/gtkohewryi.html

Java: list.contains(x)
来源：http://hz.jinyuanbaomall.cn/gtwirjgbnh.html

Go:   slices.Contains(arr, x)
来源：http://hz.iojbl.cn/gtnbcrplfb.html

Ruby: arr.include?(x)
来源：http://hz.zhijiandao.cn/gthyadxkfo.html

C#:   list.Contains(x)
来源：http://hz.zhiwuduotai.top/gtrxtgbaxa.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ywan-chungtsiang.top/gtjzcfbwca.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hfpthk.cn/gtocpwkbfw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.andypj.xyz/gthddrektg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.andypj.xyz/gtayvifhgi.html

TS:   [...arr];
来源：http://hz.hammf.cn/gthrywzzdu.html

Java: new ArrayList<>(list);
来源：http://hz.yonumen.top/gtopetyszy.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenlongwang.top/gtyzhughlg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ybcxt.top/gtdmlmhyly.html

C#:   new List<int>(list);
来源：http://hz.yangfankeji.com/gtvnsgoagh.html

[D23] reduce 累积计算
来源：http://hz.tian-w.cn/gtaxfovzoj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.pengpengdd.cyou/gtydihvnpc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj20258.top/gtcsuqurpq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.316326.xyz/gtxrdczdwa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cucudq.cn/gtaydmdpmp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jqgufenzy.top/gtxcdzhmpl.html

Go:   // 手写循环
来源：http://hz.redwolf501.top/gtwotdebsj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhongyouzk.top/gtisqwyefn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hysaishi.cn/gtznjhzhpl.html

[D24] 字典 / Map 基本操作
来源：http://hz.sysykeji.top/gtsvxidedg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhongyouzk.top/gtleuogavv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.snrcjt.cn/gtcpdajpgd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sufxvd.cn/gtadaftqqo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.iojbl.cn/gtfoihgswu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yuanzhike.top/gtxghfuopv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.fengsongda.top/gtpycbcble.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhijiandao.cn/gtgbzdkwyd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ppjwa.cn/gtwgqockwt.html

[D25] Set 集合去重与交并差
来源：http://hz.cheryme.top/gtfrpwlzwe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xinyue.icu/gtdfukblim.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nwbrower.top/gtmplvzzfr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhiwuduotai.top/gtofmrnxeb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.quarkkingdee.top/gtftctbwqg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cheryme.top/gtkitvbaop.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sysykeji.top/gtaqcjkmds.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.0kj1m.cn/gtbcmnqjmv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.daria6918.cn/gteynmijbi.html

[D26] 数组转字符串
来源：http://hz.jinghuilouyu.cn/gtxmtkywbe.html


<!-- 参考信息 -->