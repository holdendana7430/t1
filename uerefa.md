代发 wailian999

[C10] 变量作用域
来源：http://hz.yuanzhike.top/gtavftfkmw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yj202588.top/gtpwvpdzvp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.wangdashe.top/gtsmlxjzds.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.tanke756.top/gtxapquuuc.html

TS:   同 JS
来源：http://hz.yvedp.cn/gtevelpntg.html

Java: 方法内为块级作用域
来源：http://hz.snrcjt.cn/gtcqijyfbg.html

Go:   花括号块级作用域
来源：http://hz.aizwys.cn/gtnbkccyre.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhijiandao.cn/gtbqblabim.html

C#:   块级作用域
来源：http://hz.yangfankeji.com/gtqwmaixwt.html

[C11] 模块导入与导出
来源：http://hz.smart0.xyz/gteleffurr.html

Py:   from module import func
来源：http://hz.zhaomingkeji.xyz/gtctuhybue.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hammf.cn/gtuvocwkqz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.fengsongda.top/gtjjemtiav.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yanxiufei.cn/gtzsxjfekg.html

Java: import java.util.List;
来源：http://hz.sufxvd.cn/gtdtbzdhlt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yj202588.top/gtxfzqdlud.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shuidangran.top/gttdvfvtwo.html

C#:   using System.Text;
来源：http://hz.chenjidiqi.icu/gtiyfeidpq.html

[C12] 立即执行函数 IIFE
来源：http://hz.ivvv.top/gtceqsfltf.html

Py:   (lambda: print("run"))()
来源：http://hz.wangshuangyany.cn/gtmmvjpbof.html

PHP:  (function () { echo "run"; })();
来源：http://hz.redwolf501.top/gtlxkzujyt.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xylfe.cn/gtgwtpiklz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xziqi.cn/gtqgbpohfo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ivvv.top/gtfoavopxa.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xingfuxueyuan.xyz/gtoguealua.html

Ruby: -> { puts "run" }.call
来源：http://hz.tianlin.xyz/gtcwfmpwkv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.birdmap.top/gtcjbssoak.html

[C13] 类型声明 / 类型注解
来源：http://hz.yanxiufei.cn/gtjybdhanr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinqigfzy.top/gtcubcesiv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.meibo888.top/gttfefmjoa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.pengpengdd.cyou/gtvoxemmcx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pycfn.com/gtfvxpzhuh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.haohaochexian.top/gtxlxglzqg.html

Go:   func add(a, b int) int
来源：http://hz.yongpay.top/gtcaidynac.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zycfv.cn/gthswdwfou.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj202588.top/gtdhsxeflm.html

[C14] 泛型函数
来源：http://hz.fzhhl.top/gtmswmaffy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.daria6918.cn/gtnlgcwapx.html

PHP:  // 无泛型
来源：http://hz.hnqzz.top/gtekuqlfuk.html

JS:   // 无泛型
来源：http://hz.ivvv.top/gtiyidauqu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.smart0.xyz/gtvyorxzxe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hywenlv.cn/gtnmjbnxrb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ywan-chungtsiang.top/gttvkxslhc.html

Ruby: # 无泛型
来源：http://hz.zhaomingkeji.xyz/gtvloszmjg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.iojbl.cn/gtxhijaehr.html

[C15] 解构 / 展开参数
来源：http://hz.aizwys.cn/gtvrwzjsbb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sxryk.cn/gtoyhpvvco.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ppjwa.cn/gtzhfkbawy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.fengsongda.top/gtwmdjmdtn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cucudq.cn/gtikxazwes.html

Java: // 无解构
来源：http://hz.jqgufenzy.top/gtaizvngog.html

Go:   // 无解构
来源：http://hz.zhiwuduotai.top/gtrllkwwpp.html

Ruby: a, b = pair
来源：http://hz.hysaishi.cn/gtmwuustav.html

C#:   var (a, b) = pair;
来源：http://hz.gotoacloud.top/gtrlpstldq.html

[C16] 函数 / 方法重载
来源：http://hz.ehwqpu.com/gtqchjpzjq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.wangdashe.top/gtjvosmroc.html

PHP:  // 无重载
来源：http://hz.jlsjyb.cn/gtknafzhok.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.wangdashe.top/gtcqajxvjx.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jiagoushi.top/gtbrhthipm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.smart0.xyz/gtkiwjyvoj.html

Go:   // 无重载：用不同函数名
来源：http://hz.snrcjt.cn/gtybdlnwgp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.fengsongda.top/gtgkhtlwtb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.tanke756.top/gtuqgpgqot.html

================================================================================
来源：http://hz.jqgfzy.top/gtvwknvvyd.html

D. 数组 / 列表 / 集合
来源：http://hz.yonumen.top/gtzjbcixrd.html

================================================================================
来源：http://hz.shzxlz.cn/gttlagnxbe.html

[D01] 创建数组 / 列表
来源：http://hz.smart0.xyz/gtanqqrufd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cheryme.top/gtockdgwnp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.nanxuanxn.top/gtlryuhvuv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.tanke756.top/gtkmhughxz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.birdmap.top/gtkvtzdwat.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.52xcode.cn/gtctbzjgbu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jiagoushi.top/gtxohogvvw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ivvv.top/gtgwdamxgk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ybcxt.top/gtxxikzfye.html

[D02] 追加元素到末尾
来源：http://hz.jqgufenzy.top/gtznjdxdwo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xinyue.icu/gtcskbcjzj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yj20258888.top/gtnxezzoir.html

JS:   arr.push(4);
来源：http://hz.xuetiantiany.cn/gtlnixyjle.html

TS:   arr.push(4);
来源：http://hz.ppjwa.cn/gtanjzssqt.html

Java: list.add(4);
来源：http://hz.yongpay.top/gtgkfmzxdp.html

Go:   arr = append(arr, 4)
来源：http://hz.bjfxy.top/gtfsvmkpxp.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.wangshuangyany.cn/gtbhfhobdl.html

C#:   list.Add(4);
来源：http://hz.9152youxi.cn/gtsjdwndha.html

[D03] 在指定位置插入元素
来源：http://hz.gaohongyu789.top/gtguzssrjy.html

Py:   arr.insert(0, 0)
来源：http://hz.zycfv.cn/gtvgsubmwe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cdnleiting.top/gtuzwgajwa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yangfankeji.com/gtpanjcihh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hysaishi.cn/gtpjzztfhg.html

Java: list.add(0, 0);
来源：http://hz.jinqigfzy.top/gtninqhfko.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhoulong.xyz/gtgezgegfa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tian-w.cn/gtcuumtkup.html

C#:   list.Insert(0, 0);
来源：http://hz.dashuyun.cn/gtzdrwdizq.html

[D04] 删除元素
来源：http://hz.ybcxt.top/gtsuptkpmq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhengqikj.top/gtfsqfjnlb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xingfuxueyuan.xyz/gthihozcmg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yueranfly.top/gtzhiaywwk.html

TS:   arr.splice(0, 1);
来源：http://hz.pycfn.com/gtqvuwfomf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hysaishi.cn/gttkfrvtcw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yj202588.top/gtjscsxexi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jyoumei.cn/gtimkmkrvr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cdnleiting.top/gtaivtmswq.html

[D05] 访问与修改元素
来源：http://hz.mhx1999.top/gtpqcmpows.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jianghu66.top/gtbejncwtx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yongpay.top/gtamjemins.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.quarkkingdee.top/gtqwmcmqln.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yvedp.cn/gtrnhknseu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xuanzx.com/gtygnuofat.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ydjk.org.cn/gtsaxczogj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sysykeji.top/gtrcpltvvg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.c1oappe.top/gtgzyoqfke.html

[D06] 数组长度
来源：http://hz.quarkkingdee.top/gtuopsrzgf.html

Py:   len(arr)
来源：http://hz.hnxiangtu.top/gtzkbzgyeg.html

PHP:  count($arr);
来源：http://hz.jianghu66.top/gtadgrgevn.html

JS:   arr.length
来源：http://hz.yuxming.cn/gtigdgpusm.html

TS:   arr.length
来源：http://hz.yj20258888.top/gtpxsgibuw.html

Java: list.size();
来源：http://hz.shuidangran.top/gthzhwexuf.html

Go:   len(arr)
来源：http://hz.xuetiantiany.cn/gtwpwepuxs.html

Ruby: arr.length; arr.size
来源：http://hz.jiagoushi.top/gtrnosctnv.html

C#:   list.Count;
来源：http://hz.fzhhl.top/gthtzbiaci.html

[D07] 切片 / 取子数组
来源：http://hz.hywenlv.cn/gtiebzvmvf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinyuanbaomall.cn/gtiabxsvut.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xingfuxueyuan.xyz/gtsubzptmj.html

JS:   arr.slice(1, 4);
来源：http://hz.svipenyu.cn/gtnbxhlqcx.html

TS:   arr.slice(1, 4);
来源：http://hz.yuanzhike.top/gtszjuxvyl.html

Java: list.subList(1, 4);
来源：http://hz.yongpay.top/gtdjlptfir.html

Go:   arr[1:4]
来源：http://hz.chenzaomai.com/gthtqbzafw.html

Ruby: arr[1, 3]
来源：http://hz.kuanghao11.cn/gtkjwcpagw.html

C#:   list.GetRange(1, 3);
来源：http://hz.chenlongwang.top/gtzhihgpdz.html

[D08] 合并两个数组
来源：http://hz.jqgufenzy.top/gtvshvwtmj.html

Py:   a + b;  a.extend(b)
来源：http://hz.jqgfzy.top/gtnxdgfcdr.html

PHP:  array_merge($a, $b);
来源：http://hz.pycfn.com/gtlnpszece.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hammf.cn/gtpntvoxjv.html

TS:   [...a, ...b];
来源：http://hz.hywenlv.cn/gtixsulnhg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shzxlz.cn/gtuxpbyfgl.html

Go:   append(a, b...)
来源：http://hz.andypj.xyz/gtpwkvxnwt.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hnqzz.top/gtprfpruqu.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenzaomai.com/gtwryqtjbc.html

[D09] 排序（升序）
来源：http://hz.jinghuilouyu.cn/gtebkzywtl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xinyue.icu/gtdhvxwgrs.html

PHP:  sort($arr);
来源：http://hz.cdnleiting.top/gtaiuliigo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.0kj1m.cn/gttxscuoex.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ydjk.org.cn/gtnlslbufo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gzhubu.top/gtoglnzwid.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhiwuduotai.top/gtiyaewhfc.html

Ruby: arr.sort
来源：http://hz.fengsongda.top/gtrsinqjet.html

C#:   list.Sort();
来源：http://hz.hnxiangtu.top/gtyqqwpwpp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.pycfn.com/gtscrokqsa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hongshengwenyu.top/gtugtjhmcu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cheryme.top/gtlbmpbssd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtwrqlxnvi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gotoacloud.top/gtokglxfta.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgfzy.top/gtxyipbzek.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sweek.top/gtyefkvmiz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yongpay.top/gtmjtryimw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.guowangkeji.top/gtuxuyvarx.html

[D11] 反转数组
来源：http://hz.snrcjt.cn/gtqtcbpexj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cashguo.top/gtgxmgtqxo.html

PHP:  array_reverse($arr);
来源：http://hz.chenlongwang.top/gtyaickhsg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinyuanbaomall.cn/gtmrsrfoae.html

TS:   [...arr].reverse();
来源：http://hz.hammf.cn/gtqxoeyibf.html

Java: Collections.reverse(list);
来源：http://hz.hongshengwenyu.top/gtsahfrfrs.html

Go:   slices.Reverse(arr)
来源：http://hz.smart0.xyz/gtjgjwtote.html

Ruby: arr.reverse
来源：http://hz.sxryk.cn/gtnvcpmqru.html

C#:   list.Reverse();
来源：http://hz.zhengqikj.top/gtfmybzoku.html

[D12] 查找元素下标
来源：http://hz.gogol.net.cn/gtophamich.html

Py:   arr.index(x);  x in arr
来源：http://hz.daxiang520.top/gtwhammbzf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xuetiantiany.cn/gthpgwiuwp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.haohaochexian.top/gtabvtshzm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shzxlz.cn/gtqdmqalhd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sweek.top/gtqvdwoapj.html

Go:   slices.Index(arr, x)
来源：http://hz.ydjk.org.cn/gtvghlyqul.html

Ruby: arr.index(x)
来源：http://hz.nwbrower.top/gtdhvbtvxl.html

C#:   list.IndexOf(x);
来源：http://hz.xinyue.icu/gtbxjzxbpk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hammf.cn/gtjylivbkq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenjidiqi.icu/gtydjjqxud.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.mhx1999.top/gtsmraylkm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.fzhhl.top/gtctiarrgm.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ywan-chungtsiang.top/gtgcbzazdv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.dashuyun.cn/gterhlgwfy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jlsjyb.cn/gtcnaconmv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.daxiang520.top/gtmvonyauq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jlsjyb.cn/gtedjtpepg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ehwqpu.com/gtadhakmhs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.nanxinkj.top/gtnrcfeesw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhixingplan.top/gtkvbelqse.html

JS:   arr.map(x => x * 2)
来源：http://hz.c1oappe.top/gtnfsfopbm.html

TS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gtoqyvnroz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yonumen.top/gtmjrgltbo.html

Go:   // 手写循环
来源：http://hz.zycfv.cn/gtdsjcjjvq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ehwqpu.com/gtzchudfgc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.vqdsnc.cn/gtbghccjln.html

[D15] 去重
来源：http://hz.guannengcc.top/gttduqdfwu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yj20258888.top/gtaismwtdp.html

PHP:  array_unique($arr);
来源：http://hz.hnxiangtu.top/gtgkfhksdf.html

JS:   [...new Set(arr)]
来源：http://hz.fzhhl.top/gtzcsilibw.html

TS:   [...new Set(arr)]
来源：http://hz.sxryk.cn/gthzbcrskh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.aibaodan.cn/gtmindsoyb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinqigfzy.top/gtfydztvux.html

Ruby: arr.uniq
来源：http://hz.jqgufenzy.top/gtsrqxroxn.html

C#:   list.Distinct().ToList()
来源：http://hz.pycfn.com/gtaebpnmmu.html

[D16] 求和与平均值
来源：http://hz.smart0.xyz/gtknkjjrwh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.birdmap.top/gtuqjbtzdb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xuanzx.com/gtzpgqhsyx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtbynnoirs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cashguo.top/gtlcpjvobr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ydzc1.top/gtaklkqcyl.html

Go:   // 手写循环累加
来源：http://hz.havefunace.top/gtgiihqrbd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hfpthk.cn/gtkgbluuot.html

C#:   list.Sum();  list.Average()
来源：http://hz.pycfn.com/gtvcuhjtsp.html

[D17] 最大值与最小值
来源：http://hz.ywan-chungtsiang.top/gtwnquzrpm.html

Py:   max(arr);  min(arr)
来源：http://hz.aibaodan.cn/gtgbsngxiz.html

PHP:  max($arr);  min($arr);
来源：http://hz.birdmap.top/gthhqnnkqn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xinyue.icu/gtjpeyrslx.html

TS:   Math.max(...arr);
来源：http://hz.chenjidiqi.icu/gtieninejr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jiagoushi.top/gtkstplfif.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hnxiangtu.top/gtovkjsjtk.html

Ruby: arr.max;  arr.min
来源：http://hz.xuetiantiany.cn/gttsqiozjp.html

C#:   list.Max();  list.Min()
来源：http://hz.hnqzz.top/gtegazcerc.html

[D18] 扁平化嵌套数组
来源：http://hz.mhx1999.top/gtdwmcjntd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ydjk.org.cn/gtsyxsuoar.html

PHP:  array_merge(...$nested);
来源：http://hz.shanyushiyangtech.top/gthhnrtlle.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhijiandao.cn/gtyyohkocl.html

TS:   nested.flat();
来源：http://hz.yangfankeji.com/gtcgshldwl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gzhubu.top/gtehcakxbu.html

Go:   // 手写双层循环
来源：http://hz.andypj.xyz/gtabvinmgo.html

Ruby: nested.flatten
来源：http://hz.jinyuanbaomall.cn/gtrjtrxqfd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shangyingyoupin.top/gtybgdfvgv.html

[D19] 按字段分组
来源：http://hz.hnxiangtu.top/gtjmhjvkdq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.meibo888.top/gtpflmmjkf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xuetiantiany.cn/gtslqrybtx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yuanzhike.top/gtepjtrxiw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.quarkkingdee.top/gtqqjvwffl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.bjfxy.top/gtvbophacd.html

Go:   // 手写 map[string][]T
来源：http://hz.aizwys.cn/gtqkiijpnz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ybcxt.top/gtsbidemuu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yangfankeji.com/gtccyphyio.html

[D20] 统计每个元素出现次数
来源：http://hz.cheryme.top/gtsioopoum.html

Py:   Counter(arr)
来源：http://hz.daxiang520.top/gtclchncpv.html

PHP:  array_count_values($arr);
来源：http://hz.wangshuangyany.cn/gtgezfpczo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhongyouzk.top/gtuwkubgkd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.iojbl.cn/gtinbpetgf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yongpay.top/gtlduvktvi.html

Go:   // 手写 map[T]int
来源：http://hz.jinyuanbaomall.cn/gtjrinyzxl.html

Ruby: arr.tally
来源：http://hz.shuidangran.top/gtskmcqzdn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xziqi.cn/gtgjigpmlb.html

[D21] 判断是否包含某元素
来源：http://hz.nanxinkj.top/gtutngoxph.html

Py:   x in arr
来源：http://hz.52xcode.cn/gtjngvudyn.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jyoumei.cn/gtelbssirb.html

JS:   arr.includes(x)
来源：http://hz.zhijiandao.cn/gtkuvaftab.html

TS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gtoygazygz.html

Java: list.contains(x)
来源：http://hz.ydjk.org.cn/gtpktppkmj.html

Go:   slices.Contains(arr, x)
来源：http://hz.cdnleiting.top/gttdmvjgwt.html

Ruby: arr.include?(x)
来源：http://hz.nanxinkj.top/gtdohnilgi.html

C#:   list.Contains(x)
来源：http://hz.yangfankeji.com/gtpwjcygby.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinyuanbaomall.cn/gtwevxhxmg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydjk.org.cn/gtopwwobha.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ybcxt.top/gtrybcvwhw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shanyushiyangkeji.top/gtdceopdtn.html

TS:   [...arr];
来源：http://hz.daxiang520.top/gtlrfzbegp.html

Java: new ArrayList<>(list);
来源：http://hz.shangyingyoupin.top/gtunwvxhye.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zycfv.cn/gtqnhbjimi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sufxvd.cn/gtpeidqbmg.html

C#:   new List<int>(list);
来源：http://hz.hnxiangtu.top/gtjnlacqnb.html

[D23] reduce 累积计算
来源：http://hz.mhx1999.top/gtixvjibol.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.wangshuangyany.cn/gtbaqtlacx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cqqwz.cn/gtftlqfqkd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.wangshuangyany.cn/gtkkwqysoo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangkeji.top/gtsdpitrcn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nanxinkj.top/gtbzyugpeo.html

Go:   // 手写循环
来源：http://hz.hnqzz.top/gtxtoqzxzo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nwbrower.top/gtkgoxsxdn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenlongwang.top/gtlojnftuf.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenzaomai.com/gtvsdyjvbq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.kuanghao11.cn/gtkcsjamgg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.snrcjt.cn/gtdsrpqjgu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.c1oappe.top/gtwnffzcir.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj202588.top/gtxitpiohj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.snrcjt.cn/gtmagukqqb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.fengsongda.top/gtplqdckso.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xuetiantiany.cn/gtpbccwazh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ehwqpu.com/gtygaklygi.html

[D25] Set 集合去重与交并差
来源：http://hz.xylfe.cn/gtqnjirrah.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.tian-w.cn/gtsntylbxa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jlsjyb.cn/gtzahxqwvu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sysykeji.top/gtuksakzgw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.redwolf501.top/gtlpidrcke.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yueranfly.top/gtwbessusg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ybcxt.top/gtfkmtcdmh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhongyouzk.top/gteifxswcp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj202588.top/gtttbijsin.html

[D26] 数组转字符串
来源：http://hz.tian-w.cn/gttiwokecq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.haohaochexian.top/gtgigbqowr.html

PHP:  implode(", ", $arr);
来源：http://hz.hywenlv.cn/gtiebclved.html

JS:   arr.join(", ")
来源：http://hz.quarkkingdee.top/gtozqlxeof.html

TS:   arr.join(", ")
来源：http://hz.0kj1m.cn/gtokchoxmz.html

Java: String.join(", ", list)
来源：http://hz.fengsongda.top/gtwihvitgb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cheryme.top/gtptbrifxg.html

Ruby: arr.join(", ")
来源：http://hz.yj202588.top/gtxvztswpk.html

C#:   string.Join(", ", list)
来源：http://hz.xziqi.cn/gtvdjbhygf.html


<!-- 参考信息 -->