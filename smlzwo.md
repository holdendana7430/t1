代发 wailian999

TS:   同 JS
来源：http://hz.snrcjt.cn/gtxoclzweh.html

Java: 方法内为块级作用域
来源：http://hz.jinqigfzy.top/gtpvrkywpc.html

Go:   花括号块级作用域
来源：http://hz.jqgufenzy.top/gtrqbmwkqk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.nwbrower.top/gtmvncnmmq.html

C#:   块级作用域
来源：http://hz.hnqzz.top/gtubzdwmlo.html

[C11] 模块导入与导出
来源：http://hz.zdqjudy.top/gtgnwitufz.html

Py:   from module import func
来源：http://hz.birdmap.top/gtikacqtwq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ywan-chungtsiang.top/gtjspncixh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hammf.cn/gtecqpjgwr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sufxvd.cn/gtpqhtyfqd.html

Java: import java.util.List;
来源：http://hz.vqdsnc.cn/gtvohohrjd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.guowangkeji.top/gtcbrndldq.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhijiandao.cn/gtbzicders.html

C#:   using System.Text;
来源：http://hz.cqqwz.cn/gtzahzhicm.html

[C12] 立即执行函数 IIFE
来源：http://hz.tanke756.top/gtqhpkonkz.html

Py:   (lambda: print("run"))()
来源：http://hz.gzhubu.top/gtbghpwwjf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hfpthk.cn/gtddvkmpym.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jianghu66.top/gtukovsndl.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhongyouzk.top/gtaxtenlee.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinqigufen.top/gtpstikuya.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.dashuyun.cn/gtbtngdpqb.html

Ruby: -> { puts "run" }.call
来源：http://hz.chenlongwang.top/gtuxarihyh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.gogol.net.cn/gttekcmfbq.html

[C13] 类型声明 / 类型注解
来源：http://hz.daria6918.cn/gtaqeuezkx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xuanzx.com/gtgyldeimj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.0kj1m.cn/gtefakyfpv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.daria6918.cn/gtuottojgb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxuanxn.top/gtqlincjyh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.316326.xyz/gtyjjldlsv.html

Go:   func add(a, b int) int
来源：http://hz.aizwys.cn/gttwmmizbu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jyoumei.cn/gtisceovpx.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhoulong.xyz/gtizstxoqp.html

[C14] 泛型函数
来源：http://hz.pycfn.com/gtikvunlok.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cdnleiting.top/gtoifmaoyv.html

PHP:  // 无泛型
来源：http://hz.yonumen.top/gtejeyntlc.html

JS:   // 无泛型
来源：http://hz.xuanzx.com/gtolnoumtk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.316326.xyz/gtwjvtuwpq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yj20258888.top/gtgtdroinp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.guowangkeji.top/gtqdkrivia.html

Ruby: # 无泛型
来源：http://hz.sxryk.cn/gtsrhbkrsi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cheryme.top/gtushatpbh.html

[C15] 解构 / 展开参数
来源：http://hz.daxiang520.top/gtztdazpmy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cucudq.cn/gthirhpsvv.html

PHP:  [$a, $b] = $pair;
来源：http://hz.mhx1999.top/gtysxturhk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zdqjudy.top/gtunmjcvck.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xinyue.icu/gtwyhsngnq.html

Java: // 无解构
来源：http://hz.guannengcc.top/gtqpjeoeke.html

Go:   // 无解构
来源：http://hz.xingfuxueyuan.xyz/gtsucwlnsn.html

Ruby: a, b = pair
来源：http://hz.hnqzz.top/gtigfppfmm.html

C#:   var (a, b) = pair;
来源：http://hz.jlsjyb.cn/gtumntlkuf.html

[C16] 函数 / 方法重载
来源：http://hz.sweek.top/gtfxboslus.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jyoumei.cn/gtejslfaou.html

PHP:  // 无重载
来源：http://hz.nanxinkj.top/gtkhwfilvg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.52xcode.cn/gtpwjwzdxo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jlsjyb.cn/gtpzzigoxt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.pengpengdd.cyou/gtcutzwqnp.html

Go:   // 无重载：用不同函数名
来源：http://hz.xziqi.cn/gtjerogxfm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sxryk.cn/gttvvtbweq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yueranfly.top/gtlpmrdvcx.html

================================================================================
来源：http://hz.vqdsnc.cn/gtzsfhfdtk.html

D. 数组 / 列表 / 集合
来源：http://hz.xinyue.icu/gtsasgpqem.html

================================================================================
来源：http://hz.gaohongyu789.top/gtbdgspfjj.html

[D01] 创建数组 / 列表
来源：http://hz.shanyushiyangkeji.top/gtuishwzdl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sufxvd.cn/gtnvxgaxua.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jyoumei.cn/gtzqcxioun.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ehwqpu.com/gtulokajjg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj20258888.top/gtplfpkjjg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guowangkeji.top/gtaudfiziw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.bjfxy.top/gtxuqaazrl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cqqwz.cn/gtchkthnox.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuanzx.com/gtylsqlpda.html

[D02] 追加元素到末尾
来源：http://hz.hywenlv.cn/gtmguizyer.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hnxiangtu.top/gtxoeqiulz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.birdmap.top/gtitenmget.html

JS:   arr.push(4);
来源：http://hz.iojbl.cn/gthcnxkqwe.html

TS:   arr.push(4);
来源：http://hz.iojbl.cn/gtqertjker.html

Java: list.add(4);
来源：http://hz.zhongyouzk.top/gtkujccfkb.html

Go:   arr = append(arr, 4)
来源：http://hz.aibaodan.cn/gtlzmqfsyy.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xuanzx.com/gtpfzenweh.html

C#:   list.Add(4);
来源：http://hz.zycfv.cn/gtstzsyurg.html

[D03] 在指定位置插入元素
来源：http://hz.quarkkingdee.top/gtvdupxuxs.html

Py:   arr.insert(0, 0)
来源：http://hz.havefunace.top/gtdwcemrop.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ywan-chungtsiang.top/gtmwkocjpt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.haohaochexian.top/gtaleprujn.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jlsjyb.cn/gtgmeqkjkt.html

Java: list.add(0, 0);
来源：http://hz.zhijiandao.cn/gtfnmqvkfn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenzaomai.com/gtpgufgxzj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.pycfn.com/gtwktlzcsh.html

C#:   list.Insert(0, 0);
来源：http://hz.jinghuilouyu.cn/gtgrjmjiuq.html

[D04] 删除元素
来源：http://hz.zhongyouzk.top/gtaitfiwmp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.wangdashe.top/gtxbrakaud.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.daxiang520.top/gtobrhqtmj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.nanxinkj.top/gtctiwtfyf.html

TS:   arr.splice(0, 1);
来源：http://hz.fzhhl.top/gtightxgjk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ivvv.top/gtqqgfvgfv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yuxming.cn/gtsfuyzsfj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yuxming.cn/gtkhwdxvlx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.0kj1m.cn/gtnlpzzxbs.html

[D05] 访问与修改元素
来源：http://hz.sufxvd.cn/gtwwpyvban.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.316326.xyz/gtmfpxbidd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xinyue.icu/gtnombiiss.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xuetiantiany.cn/gtauwrbngu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.havefunace.top/gtafqdrcxf.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhengqikj.top/gtqmqtiduo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.52xcode.cn/gtvnjoybxl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gtymodctdo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sufxvd.cn/gtgxwijuhq.html

[D06] 数组长度
来源：http://hz.havefunace.top/gtlipleomi.html

Py:   len(arr)
来源：http://hz.sweek.top/gtqcvvfzax.html

PHP:  count($arr);
来源：http://hz.xuanzx.com/gtghdknyhc.html

JS:   arr.length
来源：http://hz.haohaochexian.top/gtnrjgpxlk.html

TS:   arr.length
来源：http://hz.zdqjudy.top/gthpeluffe.html

Java: list.size();
来源：http://hz.svipenyu.cn/gtvcrbxgwz.html

Go:   len(arr)
来源：http://hz.ybcxt.top/gtgbpqiqou.html

Ruby: arr.length; arr.size
来源：http://hz.svipenyu.cn/gtrbawrril.html

C#:   list.Count;
来源：http://hz.jlsjyb.cn/gtxznkuczi.html

[D07] 切片 / 取子数组
来源：http://hz.snrcjt.cn/gtwxtimcwt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yangfankeji.com/gtejwdfotu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.chenlongwang.top/gtfnltdmye.html

JS:   arr.slice(1, 4);
来源：http://hz.nanxinkj.top/gtmgqyyufr.html

TS:   arr.slice(1, 4);
来源：http://hz.jqgfzy.top/gtlbcbjbaj.html

Java: list.subList(1, 4);
来源：http://hz.sufxvd.cn/gtsegdplfq.html

Go:   arr[1:4]
来源：http://hz.xingfuxueyuan.xyz/gtiwssxpup.html

Ruby: arr[1, 3]
来源：http://hz.yvedp.cn/gtqkqitnkj.html

C#:   list.GetRange(1, 3);
来源：http://hz.jlsjyb.cn/gtkzxsoemt.html

[D08] 合并两个数组
来源：http://hz.gaohongyu789.top/gtzpzomidx.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhoulong.xyz/gtbadjzzsi.html

PHP:  array_merge($a, $b);
来源：http://hz.316326.xyz/gtrgjdarll.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gogol.net.cn/gtjmsevacn.html

TS:   [...a, ...b];
来源：http://hz.meibo888.top/gtumnvujhp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jinqigfzy.top/gtflpkvofw.html

Go:   append(a, b...)
来源：http://hz.gaohongyu789.top/gtuxreycda.html

Ruby: a + b;  a.concat(b)
来源：http://hz.dashuyun.cn/gtlpzycxil.html

C#:   a.Concat(b).ToList()
来源：http://hz.cqqwz.cn/gtqmejaoio.html

[D09] 排序（升序）
来源：http://hz.shanyushiyangkeji.top/gtukpyxyub.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cucudq.cn/gtoxnzbpqc.html

PHP:  sort($arr);
来源：http://hz.shanyushiyangtech.top/gtytgbijtq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cqqwz.cn/gtbhygozfp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hnxiangtu.top/gttjxxhgsn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhongyouzk.top/gtdqziufjs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jlsjyb.cn/gttsfwywbp.html

Ruby: arr.sort
来源：http://hz.jinyuanbaomall.cn/gtzdaghsgq.html

C#:   list.Sort();
来源：http://hz.gaohongyu789.top/gttamtulpy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.guowangkeji.top/gttsffpvan.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.fzhhl.top/gtnwvlhfwl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hongshengwenyu.top/gttdajmuar.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.snrcjt.cn/gtihqbckef.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangdashe.top/gtasbgpryl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.c1oappe.top/gtwretooaq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.nwbrower.top/gtxazsqhme.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.dashuyun.cn/gttjpnymrx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhiwuduotai.top/gtqqpifwdg.html

[D11] 反转数组
来源：http://hz.tianlin.xyz/gtezwbstnx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhengqikj.top/gtnpemnlkz.html

PHP:  array_reverse($arr);
来源：http://hz.andypj.xyz/gtsoerrzko.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.gaohongyu789.top/gtabxivkfo.html

TS:   [...arr].reverse();
来源：http://hz.zhiwuduotai.top/gtaqiecgyl.html

Java: Collections.reverse(list);
来源：http://hz.jqgufenzy.top/gtjspjjjbr.html

Go:   slices.Reverse(arr)
来源：http://hz.zhiwuduotai.top/gtczdfbgkv.html

Ruby: arr.reverse
来源：http://hz.jinyuanbaomall.cn/gttigmkmhz.html

C#:   list.Reverse();
来源：http://hz.sysykeji.top/gtxnxanffn.html

[D12] 查找元素下标
来源：http://hz.ehwqpu.com/gtnqhhuwvf.html

Py:   arr.index(x);  x in arr
来源：http://hz.yuxming.cn/gtczaivrct.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.tanke756.top/gtexkrpptw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yangfankeji.com/gtmmfzksko.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhaomingkeji.xyz/gtoraixhiz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yuanzhike.top/gtftgnzrad.html

Go:   slices.Index(arr, x)
来源：http://hz.xziqi.cn/gtfvyharbr.html

Ruby: arr.index(x)
来源：http://hz.mhx1999.top/gtcqdvtlpr.html

C#:   list.IndexOf(x);
来源：http://hz.hammf.cn/gttnpirkfq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jlsjyb.cn/gtdkqsrvhb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xuetiantiany.cn/gtlpwlewby.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.tian-w.cn/gtbvanjlzn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangtech.top/gtfqxrcstv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ywan-chungtsiang.top/gtnxebmujd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ywan-chungtsiang.top/gtzvipkjca.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ywan-chungtsiang.top/gtqwaigygm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.52xcode.cn/gtzctzsmgp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fzhhl.top/gtsneggkjs.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nwbrower.top/gtoduihfvu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.c1oappe.top/gtqxxvdcee.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.smart0.xyz/gtozqvcvcy.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhoulong.xyz/gtnjqbhief.html

TS:   arr.map(x => x * 2)
来源：http://hz.havefunace.top/gtpszaklsi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jlsjyb.cn/gtkxlovzmy.html

Go:   // 手写循环
来源：http://hz.ybcxt.top/gtostzjxsv.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhaomingkeji.xyz/gtqnjizrwf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ivvv.top/gtwvidboxe.html

[D15] 去重
来源：http://hz.guannengcc.top/gtwjazfgbn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shuidangran.top/gtldubbxyp.html

PHP:  array_unique($arr);
来源：http://hz.jinqigufen.top/gttktvjtmu.html

JS:   [...new Set(arr)]
来源：http://hz.guowangkeji.top/gtjnsbzjyb.html

TS:   [...new Set(arr)]
来源：http://hz.fzhhl.top/gtyqybtyvx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shanyushiyangkeji.top/gtuhcpoklg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xuanzx.com/gtuimqvdlz.html

Ruby: arr.uniq
来源：http://hz.yonumen.top/gtysfuvlve.html

C#:   list.Distinct().ToList()
来源：http://hz.chenlongwang.top/gtgspdlkoa.html

[D16] 求和与平均值
来源：http://hz.xziqi.cn/gtsfwaozfp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gzhubu.top/gtrepppiin.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yanxiufei.cn/gtzcrugizs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nwbrower.top/gtxejblkxa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daxiang520.top/gtlmzvkmul.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cheryme.top/gtsvwryozn.html

Go:   // 手写循环累加
来源：http://hz.fzhhl.top/gtjvlrpfte.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.haohaochexian.top/gtrmgbkkpr.html

C#:   list.Sum();  list.Average()
来源：http://hz.ydjk.org.cn/gtgdimlzkt.html

[D17] 最大值与最小值
来源：http://hz.guowangkeji.top/gtljhaewoi.html

Py:   max(arr);  min(arr)
来源：http://hz.shuidangran.top/gtfnkmbxfj.html

PHP:  max($arr);  min($arr);
来源：http://hz.gotoacloud.top/gtdygzkitc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yueranfly.top/gtqitydwrx.html

TS:   Math.max(...arr);
来源：http://hz.tianlin.xyz/gtjoscnprj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ydzc1.top/gtwumboujb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.aizwys.cn/gtnjlgwnan.html

Ruby: arr.max;  arr.min
来源：http://hz.jianghu66.top/gtmrwawgcy.html

C#:   list.Max();  list.Min()
来源：http://hz.svipenyu.cn/gtfxowkymu.html

[D18] 扁平化嵌套数组
来源：http://hz.yj20258.top/gtxecbtmbr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.andypj.xyz/gtxyzrcvqy.html

PHP:  array_merge(...$nested);
来源：http://hz.jqgfzy.top/gtcjqkrhtj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xylfe.cn/gtfwfbpsgc.html

TS:   nested.flat();
来源：http://hz.yanxiufei.cn/gtwjdczqgc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.aibaodan.cn/gtkbvjsgjw.html

Go:   // 手写双层循环
来源：http://hz.tianlin.xyz/gtysorjogv.html

Ruby: nested.flatten
来源：http://hz.birdmap.top/gtmeqwahha.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.316326.xyz/gthxocpslu.html

[D19] 按字段分组
来源：http://hz.gogol.net.cn/gtkvowyhut.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.pengpengdd.cyou/gtltkyfztk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.mhx1999.top/gtuumjhxpy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.52xcode.cn/gtulkneitl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.dianchejie.cn/gtdfiokytj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.wangshuangyany.cn/gtrlrzoqxo.html

Go:   // 手写 map[string][]T
来源：http://hz.chenjidiqi.icu/gtbxxkwasu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhoulong.xyz/gttikxkctq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jianghu66.top/gtxtplocsy.html

[D20] 统计每个元素出现次数
来源：http://hz.yvedp.cn/gtmuvfzmdj.html

Py:   Counter(arr)
来源：http://hz.316326.xyz/gtoenzepbu.html

PHP:  array_count_values($arr);
来源：http://hz.haohaochexian.top/gtiteflqnj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guannengcc.top/gtubzlufib.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pycfn.com/gtcujpbbgr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.snrcjt.cn/gtowwhdvio.html

Go:   // 手写 map[T]int
来源：http://hz.ybcxt.top/gtzrtumtri.html

Ruby: arr.tally
来源：http://hz.fengsongda.top/gtgibpdofr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhijiandao.cn/gtbddyyujm.html

[D21] 判断是否包含某元素
来源：http://hz.andypj.xyz/gtpdwkbcct.html

Py:   x in arr
来源：http://hz.pengpengdd.cyou/gtcyzxzagb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.snrcjt.cn/gtkqgggunl.html

JS:   arr.includes(x)
来源：http://hz.zhongyouzk.top/gtreavrkza.html

TS:   arr.includes(x)
来源：http://hz.tanke756.top/gtevzoidqy.html

Java: list.contains(x)
来源：http://hz.zhijiandao.cn/gtglfivnoy.html

Go:   slices.Contains(arr, x)
来源：http://hz.smart0.xyz/gtfugtgias.html

Ruby: arr.include?(x)
来源：http://hz.gogol.net.cn/gtajwpjgfh.html

C#:   list.Contains(x)
来源：http://hz.yj202588.top/gtikhdqluv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.iojbl.cn/gtlpjfthgs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.snrcjt.cn/gtjixtkfmz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.316326.xyz/gttavgfafb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cheryme.top/gtpanihqfb.html

TS:   [...arr];
来源：http://hz.9152youxi.cn/gtdkkmqyfo.html

Java: new ArrayList<>(list);
来源：http://hz.zdqjudy.top/gtrlhvasms.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hnxiangtu.top/gtikaluwfy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gaohongyu789.top/gtpxeaytln.html

C#:   new List<int>(list);
来源：http://hz.chenlongwang.top/gtuckoepwy.html

[D23] reduce 累积计算
来源：http://hz.jlsjyb.cn/gtwlceuewr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhaomingkeji.xyz/gtfbgwmzol.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.bjfxy.top/gtdtmozlni.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.smart0.xyz/gtqlxjrtcu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cheryme.top/gtqppeoexm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhijiandao.cn/gtyvcidknd.html

Go:   // 手写循环
来源：http://hz.fzhhl.top/gtirzjcnlr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.9152youxi.cn/gttbndrbwh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cashguo.top/gtrtgsomep.html

[D24] 字典 / Map 基本操作
来源：http://hz.yvedp.cn/gthvsvgsyu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinqigfzy.top/gtrjtcktcn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.tian-w.cn/gtpsrpztgw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sxryk.cn/gtpcqslywt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258.top/gtgogmzdyo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.quarkkingdee.top/gtosriftxz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.9152youxi.cn/gtjdrmdijx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.snrcjt.cn/gtjbqpsypa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cheryme.top/gtiqlpecyo.html

[D25] Set 集合去重与交并差
来源：http://hz.mhx1999.top/gtxzozduvq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ivvv.top/gtqrfskypv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jqgufenzy.top/gtmdfghjos.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.haohaochexian.top/gtwodhicpr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.9152youxi.cn/gtouprivwn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.tanke756.top/gtklhppzjg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yuxming.cn/gtfnlabsvr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gogol.net.cn/gtngdcgcts.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.havefunace.top/gtnbvdgjtv.html

[D26] 数组转字符串
来源：http://hz.xinyue.icu/gtrjrnihfo.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yuanzhike.top/gtzpjwowkr.html

PHP:  implode(", ", $arr);
来源：http://hz.shuidangran.top/gtmiogdwcz.html

JS:   arr.join(", ")
来源：http://hz.hywenlv.cn/gtjudxbyue.html

TS:   arr.join(", ")
来源：http://hz.wangshuangyany.cn/gtqxlxadlk.html

Java: String.join(", ", list)
来源：http://hz.hnxiangtu.top/gtnisjbkue.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yonumen.top/gtkimmdygp.html

Ruby: arr.join(", ")
来源：http://hz.hysaishi.cn/gteuvtgvjz.html

C#:   string.Join(", ", list)
来源：http://hz.yonumen.top/gtqvobfjhg.html

================================================================================
来源：http://hz.tanke756.top/gtfrhxkkpq.html

E. 字符串处理
来源：http://hz.vqdsnc.cn/gtqeansdct.html

================================================================================
来源：http://hz.tianlin.xyz/gtysajbwlj.html

[E01] 拼接字符串
来源：http://hz.wangdashe.top/gtlfrpvdgb.html


<!-- 参考信息 -->