代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tian-w.cn/gtkanjebey.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhixingplan.top/gteimdcsrf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xylfe.cn/gthtsdwbjj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nanxinkj.top/gtzsbswucl.html

[C10] 变量作用域
来源：http://hz.smart0.xyz/gtxzlyapql.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.nanxuanxn.top/gtdjbfdvgr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhengqikj.top/gtviduhpnl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gaohongyu789.top/gtzisaicxg.html

TS:   同 JS
来源：http://hz.jinqigufen.top/gtaawxxbbf.html

Java: 方法内为块级作用域
来源：http://hz.yj202588.top/gtyneorbrn.html

Go:   花括号块级作用域
来源：http://hz.hnqzz.top/gtqkroelik.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinqigfzy.top/gttogawpde.html

C#:   块级作用域
来源：http://hz.hysaishi.cn/gtdhuuaict.html

[C11] 模块导入与导出
来源：http://hz.jiagoushi.top/gtmxljvohw.html

Py:   from module import func
来源：http://hz.havefunace.top/gtopuamjrm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shanyushiyangtech.top/gtjsexypwe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cdnleiting.top/gtcmjnrlwk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cheryme.top/gtfzznobpa.html

Java: import java.util.List;
来源：http://hz.yuxming.cn/gtntsterig.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shzxlz.cn/gtxrlguwnt.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.bjfxy.top/gtkcvydyaq.html

C#:   using System.Text;
来源：http://hz.zhoulong.xyz/gtlxloxnkx.html

[C12] 立即执行函数 IIFE
来源：http://hz.yuxming.cn/gtympbygnb.html

Py:   (lambda: print("run"))()
来源：http://hz.sweek.top/gtamfgldli.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nwbrower.top/gtosuhaucz.html

JS:   (() => { console.log("run"); })();
来源：http://hz.gzhubu.top/gtvilsfvnc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ppjwa.cn/gtekujxree.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yonumen.top/gthydtsjhv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.daria6918.cn/gthjhduoba.html

Ruby: -> { puts "run" }.call
来源：http://hz.tian-w.cn/gtmyecnrgz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.haohaochexian.top/gthfpeqyom.html

[C13] 类型声明 / 类型注解
来源：http://hz.zycfv.cn/gtjpwzksbj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.fengsongda.top/gtrrykawes.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.0kj1m.cn/gtifraxbja.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yonumen.top/gtfojdxfaq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jlsjyb.cn/gtfdxcsxew.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yuanzhike.top/gtqjfzhgdk.html

Go:   func add(a, b int) int
来源：http://hz.tanke756.top/gtyoodaehy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ydjk.org.cn/gtzxcvhleb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gogol.net.cn/gtwmatgnqi.html

[C14] 泛型函数
来源：http://hz.jinghuilouyu.cn/gtedwryjae.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yongpay.top/gtjhclvgki.html

PHP:  // 无泛型
来源：http://hz.shangyingyoupin.top/gtkkkfwyoq.html

JS:   // 无泛型
来源：http://hz.cqqwz.cn/gtpuguyyxw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.chenlongwang.top/gtjalbdihm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.guowangkeji.top/gthhireeog.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ivvv.top/gtgifiuler.html

Ruby: # 无泛型
来源：http://hz.cdnleiting.top/gtylkxcbbg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.wangshuangyany.cn/gtasygjpbm.html

[C15] 解构 / 展开参数
来源：http://hz.zhijiandao.cn/gtbbyaljjt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.316326.xyz/gtgyzzygfu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ybcxt.top/gtqzulbvdm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhijiandao.cn/gthuxdaqyp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yj202588.top/gtpyhdelpk.html

Java: // 无解构
来源：http://hz.shangyingyoupin.top/gtvchokyoa.html

Go:   // 无解构
来源：http://hz.yangfankeji.com/gtwovcjpsf.html

Ruby: a, b = pair
来源：http://hz.jqgufenzy.top/gtsvujxqcs.html

C#:   var (a, b) = pair;
来源：http://hz.yongpay.top/gtfapewsgs.html

[C16] 函数 / 方法重载
来源：http://hz.ydjk.org.cn/gtibgmwlbh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tanke756.top/gtiowucovx.html

PHP:  // 无重载
来源：http://hz.vqdsnc.cn/gtucsaohpp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.52xcode.cn/gtagcmylft.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.iojbl.cn/gthutkpcta.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cashguo.top/gtmqvyubua.html

Go:   // 无重载：用不同函数名
来源：http://hz.havefunace.top/gtruxftomg.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zdqjudy.top/gtwesappmp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.nanxuanxn.top/gtgmeuuogj.html

================================================================================
来源：http://hz.quarkkingdee.top/gtqduqarcb.html

D. 数组 / 列表 / 集合
来源：http://hz.chenzaomai.com/gtkfeolxdb.html

================================================================================
来源：http://hz.hfpthk.cn/gttlrmpecg.html

[D01] 创建数组 / 列表
来源：http://hz.ehwqpu.com/gtzonlmfzl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yj20258888.top/gtedqnbkae.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.feifeiyinyue.top/gtqxwtrmrc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.tanke756.top/gtueehitbi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj202588.top/gtcolzbqyn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ivvv.top/gtfimbcfjv.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xinyue.icu/gtaozvbdln.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nwbrower.top/gtrdnihsjo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuetiantiany.cn/gtzfvfchvh.html

[D02] 追加元素到末尾
来源：http://hz.jiagoushi.top/gtwsenfqxk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.feifeiyinyue.top/gtkhgdituk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuanzx.com/gtpsgpguwv.html

JS:   arr.push(4);
来源：http://hz.xinyue.icu/gtlzthoztx.html

TS:   arr.push(4);
来源：http://hz.wangshuangyany.cn/gtfpmrmjmn.html

Java: list.add(4);
来源：http://hz.pycfn.com/gtdxaampvo.html

Go:   arr = append(arr, 4)
来源：http://hz.0kj1m.cn/gttqotkzee.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.pengpengdd.cyou/gtribnkmmy.html

C#:   list.Add(4);
来源：http://hz.yuanzhike.top/gtegywfdos.html

[D03] 在指定位置插入元素
来源：http://hz.smart0.xyz/gteyphtoea.html

Py:   arr.insert(0, 0)
来源：http://hz.hywenlv.cn/gtfkdbwjym.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.nwbrower.top/gtkxjqcskf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.tanke756.top/gtoceepoam.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.chenzaomai.com/gtqkinbtmm.html

Java: list.add(0, 0);
来源：http://hz.nwbrower.top/gtynttuiwu.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cqqwz.cn/gtystsjzoh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydzc1.top/gtjevgxevl.html

C#:   list.Insert(0, 0);
来源：http://hz.ivvv.top/gtzxwpqqfy.html

[D04] 删除元素
来源：http://hz.aizwys.cn/gtkrdyokic.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhongyouzk.top/gtuzuylmpx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zdqjudy.top/gtlzppidkc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhoulong.xyz/gtdvtwuoiy.html

TS:   arr.splice(0, 1);
来源：http://hz.hongshengwenyu.top/gtoyyvxnhp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.mhx1999.top/gtouwklmzg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.birdmap.top/gtiwhksqrs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nwbrower.top/gtcrdgzzir.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.mhx1999.top/gtgxghxavm.html

[D05] 访问与修改元素
来源：http://hz.svipenyu.cn/gtujuphudx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtqdqulffe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.chenlongwang.top/gtkzfjzivs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtlquiyswa.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gaohongyu789.top/gtgwsjpjdl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.dashuyun.cn/gtkaygumcg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jianghu66.top/gtkrspeqia.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.feifeiyinyue.top/gtgdhgzxnu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.smart0.xyz/gtnlsjvqyq.html

[D06] 数组长度
来源：http://hz.tianlin.xyz/gttqfqdbjd.html

Py:   len(arr)
来源：http://hz.zhijiandao.cn/gtxfdswwbi.html

PHP:  count($arr);
来源：http://hz.zhongyouzk.top/gtrmuyrqno.html

JS:   arr.length
来源：http://hz.shangyingyoupin.top/gtcathrbzo.html

TS:   arr.length
来源：http://hz.hnqzz.top/gtqjqfbuba.html

Java: list.size();
来源：http://hz.zhongyouzk.top/gtstvdmmee.html

Go:   len(arr)
来源：http://hz.jinghuilouyu.cn/gtjbwoajge.html

Ruby: arr.length; arr.size
来源：http://hz.xinyue.icu/gttptbnsld.html

C#:   list.Count;
来源：http://hz.yongpay.top/gtxdcdgopd.html

[D07] 切片 / 取子数组
来源：http://hz.daxiang520.top/gtjwptvviw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yonumen.top/gtwpzabwbm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hysaishi.cn/gtavllbfab.html

JS:   arr.slice(1, 4);
来源：http://hz.sufxvd.cn/gtaxvobvzv.html

TS:   arr.slice(1, 4);
来源：http://hz.bjfxy.top/gtsdkcgxav.html

Java: list.subList(1, 4);
来源：http://hz.haohaochexian.top/gtgaubsgsq.html

Go:   arr[1:4]
来源：http://hz.zhengqikj.top/gtrbzurlsz.html

Ruby: arr[1, 3]
来源：http://hz.pycfn.com/gtdpimcxse.html

C#:   list.GetRange(1, 3);
来源：http://hz.yongpay.top/gtbjazpwut.html

[D08] 合并两个数组
来源：http://hz.jyoumei.cn/gtntyhnryp.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj20258888.top/gtnpddgusp.html

PHP:  array_merge($a, $b);
来源：http://hz.aizwys.cn/gtmqticvsm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yangfankeji.com/gtsjuquoig.html

TS:   [...a, ...b];
来源：http://hz.zhoulong.xyz/gtzmqhfkvj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ehwqpu.com/gtuowilegl.html

Go:   append(a, b...)
来源：http://hz.sweek.top/gtoyrumgsg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhiwuduotai.top/gtbjkjjuav.html

C#:   a.Concat(b).ToList()
来源：http://hz.hnxiangtu.top/gtohwoqplw.html

[D09] 排序（升序）
来源：http://hz.cdnleiting.top/gtfuouofwl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.feifeiyinyue.top/gtvncqxkbu.html

PHP:  sort($arr);
来源：http://hz.smart0.xyz/gtfjoffsxw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xingfuxueyuan.xyz/gtdjyqfocf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.redwolf501.top/gtrjclfruo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.guannengcc.top/gtmfvpbbwe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.guowangkeji.top/gtaktwcnqs.html

Ruby: arr.sort
来源：http://hz.smart0.xyz/gtropylyak.html

C#:   list.Sort();
来源：http://hz.ppjwa.cn/gtraaluvhh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.smart0.xyz/gtunvnwhjn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gzhubu.top/gtzmqgcgax.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhongyouzk.top/gtpqkjkjkq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sufxvd.cn/gtrjqjfozj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hongshengwenyu.top/gtomnviioz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hongshengwenyu.top/gtqtuqjaes.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xinyue.icu/gtyaclrskz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cheryme.top/gtqgcbyagv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.guannengcc.top/gtsltmpxss.html

[D11] 反转数组
来源：http://hz.havefunace.top/gtldxlhdic.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.guannengcc.top/gtosguidnc.html

PHP:  array_reverse($arr);
来源：http://hz.yj20258.top/gtwxutuqqf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jyoumei.cn/gtkimfkycv.html

TS:   [...arr].reverse();
来源：http://hz.yuxming.cn/gtrrgywbin.html

Java: Collections.reverse(list);
来源：http://hz.ppjwa.cn/gtqrtneqkg.html

Go:   slices.Reverse(arr)
来源：http://hz.hfpthk.cn/gtinhqxoaa.html

Ruby: arr.reverse
来源：http://hz.jinghuilouyu.cn/gtukmjgxrd.html

C#:   list.Reverse();
来源：http://hz.zhongyouzk.top/gtypsxqhiq.html

[D12] 查找元素下标
来源：http://hz.zhengqikj.top/gtuoxfsexx.html

Py:   arr.index(x);  x in arr
来源：http://hz.yuxming.cn/gtnmhulvij.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xziqi.cn/gtjeaovmrt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.smart0.xyz/gtbcuxuvae.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sweek.top/gtwsxdvixe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yueranfly.top/gtputjdyoh.html

Go:   slices.Index(arr, x)
来源：http://hz.jinghuilouyu.cn/gtrfomtvnk.html

Ruby: arr.index(x)
来源：http://hz.yj20258.top/gtrrokaref.html

C#:   list.IndexOf(x);
来源：http://hz.sufxvd.cn/gtyxgbagub.html

[D13] 过滤（保留满足条件的）
来源：http://hz.kuanghao11.cn/gtocskawiv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnxiangtu.top/gtzmmyfcwg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhengqikj.top/gtetcpltci.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhoulong.xyz/gtwlidxiwq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.nwbrower.top/gttwihvlgz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gotoacloud.top/gtugevxmpx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj202588.top/gtziyauhlr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.c1oappe.top/gtmljvbeqb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xylfe.cn/gtksjouxsa.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jiagoushi.top/gtdmaknmyq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yangfankeji.com/gtrpfcmerz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shangyingyoupin.top/gteqtoaruy.html

JS:   arr.map(x => x * 2)
来源：http://hz.ppjwa.cn/gtsoxwvgxp.html

TS:   arr.map(x => x * 2)
来源：http://hz.shuidangran.top/gtbxgdayjl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tanke756.top/gtbcljicke.html

Go:   // 手写循环
来源：http://hz.ywan-chungtsiang.top/gtejptgwof.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ywan-chungtsiang.top/gtezizdwqc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jqgufenzy.top/gtaeydnrbq.html

[D15] 去重
来源：http://hz.chenlongwang.top/gtixebrmrp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xinyue.icu/gtritnmsxy.html

PHP:  array_unique($arr);
来源：http://hz.aizwys.cn/gtnobgemod.html

JS:   [...new Set(arr)]
来源：http://hz.havefunace.top/gtherylpcu.html

TS:   [...new Set(arr)]
来源：http://hz.cheryme.top/gtpxsvvbxw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.wangdashe.top/gtojexuont.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hfpthk.cn/gtzjsrrxmf.html

Ruby: arr.uniq
来源：http://hz.zhoulong.xyz/gtlytbcuek.html

C#:   list.Distinct().ToList()
来源：http://hz.ppjwa.cn/gtazlfqbgj.html

[D16] 求和与平均值
来源：http://hz.zhengqikj.top/gtqaowfqwf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shanyushiyangkeji.top/gthdlckzqw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenzaomai.com/gtxiypckwe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuxming.cn/gtdcbxueze.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.vqdsnc.cn/gtorlitxov.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.guowangkeji.top/gtdzopnxsw.html

Go:   // 手写循环累加
来源：http://hz.hysaishi.cn/gtcykgujkm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jqgfzy.top/gtesjsjnyf.html

C#:   list.Sum();  list.Average()
来源：http://hz.havefunace.top/gtagjbrwmx.html

[D17] 最大值与最小值
来源：http://hz.hammf.cn/gtvxupavtp.html

Py:   max(arr);  min(arr)
来源：http://hz.yj202588.top/gtkzbkcmgi.html

PHP:  max($arr);  min($arr);
来源：http://hz.hysaishi.cn/gtkvpcmrgv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shangyingyoupin.top/gtfpbbzmen.html

TS:   Math.max(...arr);
来源：http://hz.shzxlz.cn/gtawvqtgkj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.52xcode.cn/gtxjwfyigf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jqgfzy.top/gtjsieselx.html

Ruby: arr.max;  arr.min
来源：http://hz.shangyingyoupin.top/gtlbzlcpor.html

C#:   list.Max();  list.Min()
来源：http://hz.xylfe.cn/gtpkppaguw.html

[D18] 扁平化嵌套数组
来源：http://hz.nwbrower.top/gtfpahcpst.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.c1oappe.top/gtnxuxxyax.html

PHP:  array_merge(...$nested);
来源：http://hz.hysaishi.cn/gteattldkk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yvedp.cn/gtlhmnonlz.html

TS:   nested.flat();
来源：http://hz.jqgfzy.top/gtmnwiazgo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hnxiangtu.top/gtrthssgfh.html

Go:   // 手写双层循环
来源：http://hz.smart0.xyz/gtaatkqivn.html

Ruby: nested.flatten
来源：http://hz.hammf.cn/gtakoiczfc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.bjfxy.top/gtvanipbty.html

[D19] 按字段分组
来源：http://hz.ehwqpu.com/gtkhkvzbgp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.nanxuanxn.top/gtoqmbxwer.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tanke756.top/gtnvdvltdj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenzaomai.com/gtywydzmeo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhongyouzk.top/gtufjfkaom.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zdqjudy.top/gtpfcrhsym.html

Go:   // 手写 map[string][]T
来源：http://hz.yuxming.cn/gtvupuigtf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.feifeiyinyue.top/gtfnvceqmq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zdqjudy.top/gtaszpyhge.html

[D20] 统计每个元素出现次数
来源：http://hz.c1oappe.top/gtzbicdehc.html

Py:   Counter(arr)
来源：http://hz.xylfe.cn/gtuskagrru.html

PHP:  array_count_values($arr);
来源：http://hz.havefunace.top/gtwnurxgqq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hfpthk.cn/gtlbitflss.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sufxvd.cn/gtrywgmttt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj202588.top/gtrrntboqb.html

Go:   // 手写 map[T]int
来源：http://hz.zhengqikj.top/gtxnsqbrga.html

Ruby: arr.tally
来源：http://hz.sufxvd.cn/gtnevmtpsh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.smart0.xyz/gtxggupkas.html

[D21] 判断是否包含某元素
来源：http://hz.zhoulong.xyz/gtqopizoju.html

Py:   x in arr
来源：http://hz.hammf.cn/gtddbbmkja.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jqgufenzy.top/gtgtjcvifj.html

JS:   arr.includes(x)
来源：http://hz.sysykeji.top/gtxhewjuiv.html

TS:   arr.includes(x)
来源：http://hz.shangyingyoupin.top/gtnmtdvbfk.html

Java: list.contains(x)
来源：http://hz.aibaodan.cn/gtmaajnrrk.html

Go:   slices.Contains(arr, x)
来源：http://hz.dianchejie.cn/gtvjcokhww.html

Ruby: arr.include?(x)
来源：http://hz.iojbl.cn/gtntuxzvrp.html

C#:   list.Contains(x)
来源：http://hz.jyoumei.cn/gtlzkcxkjf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yonumen.top/gtrxzkvcem.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xinyue.icu/gtzfhfzttz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yvedp.cn/gtznciojqk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.birdmap.top/gtyapgxbyi.html

TS:   [...arr];
来源：http://hz.52xcode.cn/gtrnqznyzi.html

Java: new ArrayList<>(list);
来源：http://hz.yanxiufei.cn/gtujzylbhr.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinqigfzy.top/gtxqqmiujy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.chenzaomai.com/gtyqbygnlh.html

C#:   new List<int>(list);
来源：http://hz.nanxuanxn.top/gtyjwkjkcm.html

[D23] reduce 累积计算
来源：http://hz.kuanghao11.cn/gtbilwgyun.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.nanxuanxn.top/gtkpfdxylg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zdqjudy.top/gtohapoems.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sxryk.cn/gtnamcijks.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gotoacloud.top/gtnpnwfhnw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xuanzx.com/gtcnwtlasw.html

Go:   // 手写循环
来源：http://hz.meibo888.top/gtagctgpmx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenlongwang.top/gtberskclt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.nanxinkj.top/gtqgcsbvzt.html

[D24] 字典 / Map 基本操作
来源：http://hz.andypj.xyz/gtpgktccnh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.bjfxy.top/gtnkkrplic.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.meibo888.top/gtvuxcbtgp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shanyushiyangtech.top/gtjmadjvqm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hammf.cn/gtzyubmtfw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenlongwang.top/gtahmafvzf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.haohaochexian.top/gtccgkhgbd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nanxinkj.top/gtnmsmvzmt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.52xcode.cn/gtfpucdzed.html

[D25] Set 集合去重与交并差
来源：http://hz.cheryme.top/gtrdyrgkcj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jqgfzy.top/gtxhcaggkc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.snrcjt.cn/gtbldesftn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jqgufenzy.top/gtrtizfuzn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.haohaochexian.top/gtfgjjaltr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.pycfn.com/gtfisjzfyi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.andypj.xyz/gtnukdayew.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhixingplan.top/gtbychmvcr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yvedp.cn/gtcpvapjei.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangkeji.top/gtpaeactcl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xuanzx.com/gttqwjgscf.html

PHP:  implode(", ", $arr);
来源：http://hz.fzhhl.top/gtngjxgbti.html

JS:   arr.join(", ")
来源：http://hz.guannengcc.top/gtvxsaujfx.html

TS:   arr.join(", ")
来源：http://hz.hnxiangtu.top/gtxgwxsdte.html


<!-- 参考信息 -->