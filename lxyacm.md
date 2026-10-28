代发 wailian999

[C10] 变量作用域
来源：http://hz.jinyuanbaomall.cn/gtttioictm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ywan-chungtsiang.top/gtxuudrlfp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sufxvd.cn/gtllsevjux.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cqqwz.cn/gtvomtxabt.html

TS:   同 JS
来源：http://hz.xingfuxueyuan.xyz/gtddhwqolq.html

Java: 方法内为块级作用域
来源：http://hz.nanxuanxn.top/gtvrappyer.html

Go:   花括号块级作用域
来源：http://hz.shuidangran.top/gtwxhvpxsz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jqgfzy.top/gthpmapbsp.html

C#:   块级作用域
来源：http://hz.yuxming.cn/gtfdwgjcdc.html

[C11] 模块导入与导出
来源：http://hz.zhongyouzk.top/gtubewvlak.html

Py:   from module import func
来源：http://hz.kuanghao11.cn/gtvhanehqi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cqqwz.cn/gtviqhyhkg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hammf.cn/gtbefxczhr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ybcxt.top/gtnrlezmpb.html

Java: import java.util.List;
来源：http://hz.hfpthk.cn/gthxsqiypo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigufen.top/gtiosqxpgj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zycfv.cn/gtrkdlhvpb.html

C#:   using System.Text;
来源：http://hz.daxiang520.top/gtctprxawp.html

[C12] 立即执行函数 IIFE
来源：http://hz.ydzc1.top/gtbdnumtjv.html

Py:   (lambda: print("run"))()
来源：http://hz.hnqzz.top/gtadefzmxj.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhongyouzk.top/gttefeloly.html

JS:   (() => { console.log("run"); })();
来源：http://hz.birdmap.top/gticlauvvb.html

TS:   (() => { console.log("run"); })();
来源：http://hz.bjfxy.top/gtxdftpgcx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yuxming.cn/gtybrxtuvi.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.feifeiyinyue.top/gttjorhyar.html

Ruby: -> { puts "run" }.call
来源：http://hz.jianghu66.top/gtanffonke.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yuanzhike.top/gtahxvckbu.html

[C13] 类型声明 / 类型注解
来源：http://hz.feifeiyinyue.top/gtyquviynp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhengqikj.top/gtrmveamfe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.birdmap.top/gtaimthjki.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yvedp.cn/gtdaoelotn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sufxvd.cn/gttttrxlpo.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtzqvpndrz.html

Go:   func add(a, b int) int
来源：http://hz.pengpengdd.cyou/gtdixdqgke.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yangfankeji.com/gtxtjpslds.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.feifeiyinyue.top/gtsgxqmbzp.html

[C14] 泛型函数
来源：http://hz.daxiang520.top/gtxlmpuzio.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hysaishi.cn/gtvjcrrfel.html

PHP:  // 无泛型
来源：http://hz.sxryk.cn/gtsjdrbxir.html

JS:   // 无泛型
来源：http://hz.xingfuxueyuan.xyz/gtyuulcjje.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ivvv.top/gtuivlwpgy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhijiandao.cn/gtpckqbkfk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinqigufen.top/gtyteqgtzu.html

Ruby: # 无泛型
来源：http://hz.316326.xyz/gtibleyzuq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.smart0.xyz/gthcoydfdg.html

[C15] 解构 / 展开参数
来源：http://hz.pengpengdd.cyou/gtqdvuenqj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yuanzhike.top/gtjmglfxan.html

PHP:  [$a, $b] = $pair;
来源：http://hz.quarkkingdee.top/gtzlkqatgk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sweek.top/gtrjzcbhxj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gzhubu.top/gtktuwdncp.html

Java: // 无解构
来源：http://hz.ivvv.top/gtnwkqsyod.html

Go:   // 无解构
来源：http://hz.redwolf501.top/gturtirbms.html

Ruby: a, b = pair
来源：http://hz.guowangkeji.top/gtqoyvtxef.html

C#:   var (a, b) = pair;
来源：http://hz.cdnleiting.top/gtsdszegwi.html

[C16] 函数 / 方法重载
来源：http://hz.cqqwz.cn/gtvmyzquim.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nwbrower.top/gtzqpihabb.html

PHP:  // 无重载
来源：http://hz.xziqi.cn/gttdlrwuvn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.wangshuangyany.cn/gtlhendhzo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gotoacloud.top/gtjepvzqry.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cqqwz.cn/gtntnxeryn.html

Go:   // 无重载：用不同函数名
来源：http://hz.redwolf501.top/gthijrbisd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hnxiangtu.top/gtodehibqr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ydzc1.top/gtrwfiahzu.html

================================================================================
来源：http://hz.yongpay.top/gtgyxstuim.html

D. 数组 / 列表 / 集合
来源：http://hz.ybcxt.top/gtwszczbbx.html

================================================================================
来源：http://hz.dianchejie.cn/gtivzhkyzy.html

[D01] 创建数组 / 列表
来源：http://hz.smart0.xyz/gtfdqugjvq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jiagoushi.top/gtxrcedrtz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yj20258.top/gtksfolnca.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.52xcode.cn/gteozkrjmb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yvedp.cn/gthjfgajkm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.daria6918.cn/gtbqmpszyr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.smart0.xyz/gtugpxnfkf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xinyue.icu/gtkbihciqz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aibaodan.cn/gtkclfoxev.html

[D02] 追加元素到末尾
来源：http://hz.wangdashe.top/gtuqekcvat.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhaomingkeji.xyz/gtzrjnlsjl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yanxiufei.cn/gttrmyjzas.html

JS:   arr.push(4);
来源：http://hz.9152youxi.cn/gtbqndhyul.html

TS:   arr.push(4);
来源：http://hz.hongshengwenyu.top/gtrgacosiu.html

Java: list.add(4);
来源：http://hz.gaohongyu789.top/gtbyvtzpra.html

Go:   arr = append(arr, 4)
来源：http://hz.tian-w.cn/gtduzsfmez.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yj20258888.top/gtzhnpiuke.html

C#:   list.Add(4);
来源：http://hz.sysykeji.top/gtubkeogyo.html

[D03] 在指定位置插入元素
来源：http://hz.shzxlz.cn/gtzmogjbnv.html

Py:   arr.insert(0, 0)
来源：http://hz.tian-w.cn/gtkmjqynts.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cheryme.top/gtyuagmpoa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hongshengwenyu.top/gtuvjseaxe.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.meibo888.top/gtnsgidqkt.html

Java: list.add(0, 0);
来源：http://hz.haohaochexian.top/gtdpvunedu.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenzaomai.com/gtsvlmxeaq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sysykeji.top/gtklecncaj.html

C#:   list.Insert(0, 0);
来源：http://hz.dianchejie.cn/gtauylywkt.html

[D04] 删除元素
来源：http://hz.hywenlv.cn/gttzwvcnjs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yonumen.top/gtwoadwqwa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shangyingyoupin.top/gttdptffgw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jqgufenzy.top/gtwtqlcufo.html

TS:   arr.splice(0, 1);
来源：http://hz.meibo888.top/gtbyffyzly.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.bjfxy.top/gtoxhjoigo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hammf.cn/gtwkexnszc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhijiandao.cn/gtsmaatmsp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hywenlv.cn/gthsgeojrt.html

[D05] 访问与修改元素
来源：http://hz.wangdashe.top/gtgarhbgal.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.svipenyu.cn/gtpdozzdfs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.pycfn.com/gthfrgcrff.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.andypj.xyz/gtymfdfpke.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jyoumei.cn/gtgusnldxu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yongpay.top/gtqyisckox.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.vqdsnc.cn/gtiicpiozm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gtduhbbuuf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yanxiufei.cn/gthxpjrzml.html

[D06] 数组长度
来源：http://hz.cqqwz.cn/gtvexhpogi.html

Py:   len(arr)
来源：http://hz.xylfe.cn/gtnuivheui.html

PHP:  count($arr);
来源：http://hz.shzxlz.cn/gtrsktfecc.html

JS:   arr.length
来源：http://hz.ydzc1.top/gtmuznaeoq.html

TS:   arr.length
来源：http://hz.sysykeji.top/gtqmpyvfrf.html

Java: list.size();
来源：http://hz.smart0.xyz/gtkmwioore.html

Go:   len(arr)
来源：http://hz.zdqjudy.top/gtthmaibji.html

Ruby: arr.length; arr.size
来源：http://hz.hysaishi.cn/gtwpdhaoek.html

C#:   list.Count;
来源：http://hz.xuetiantiany.cn/gtrvzvkijd.html

[D07] 切片 / 取子数组
来源：http://hz.bjfxy.top/gtucmullrh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinyuanbaomall.cn/gtdspwguhq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hysaishi.cn/gtbgdbiihv.html

JS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangtech.top/gtxcahoazj.html

TS:   arr.slice(1, 4);
来源：http://hz.zdqjudy.top/gttwpiiegq.html

Java: list.subList(1, 4);
来源：http://hz.pycfn.com/gtqexhkmaf.html

Go:   arr[1:4]
来源：http://hz.snrcjt.cn/gtrzvmdokc.html

Ruby: arr[1, 3]
来源：http://hz.vqdsnc.cn/gtljhoeqpr.html

C#:   list.GetRange(1, 3);
来源：http://hz.bjfxy.top/gtejuvbluk.html

[D08] 合并两个数组
来源：http://hz.xinyue.icu/gtnuwtuwod.html

Py:   a + b;  a.extend(b)
来源：http://hz.yangfankeji.com/gtstypksug.html

PHP:  array_merge($a, $b);
来源：http://hz.wangdashe.top/gtblzclyiw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cdnleiting.top/gtmwatqolv.html

TS:   [...a, ...b];
来源：http://hz.andypj.xyz/gtbdivwdeo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangkeji.top/gtpiinpuma.html

Go:   append(a, b...)
来源：http://hz.andypj.xyz/gtitpcuuni.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ydzc1.top/gtuwlxsfzr.html

C#:   a.Concat(b).ToList()
来源：http://hz.ywan-chungtsiang.top/gtyprzecya.html

[D09] 排序（升序）
来源：http://hz.gzhubu.top/gtjgloiqxu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pengpengdd.cyou/gtmukmnsox.html

PHP:  sort($arr);
来源：http://hz.chenzaomai.com/gtfyfnnqbp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hysaishi.cn/gtcffyxdqy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ppjwa.cn/gtesdkoybj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gogol.net.cn/gtdzqgiceo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gtencimujd.html

Ruby: arr.sort
来源：http://hz.guowangkeji.top/gtwwdsyiic.html

C#:   list.Sort();
来源：http://hz.quarkkingdee.top/gtpyhxoeld.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hnxiangtu.top/gtoowwgtku.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xziqi.cn/gtcdczihdv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shzxlz.cn/gtmiuduwvu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigfzy.top/gtfngeaddb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258888.top/gtadlancuk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shzxlz.cn/gttfboljsy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shuidangran.top/gtxhoejccy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jqgfzy.top/gtwhfyzrik.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.smart0.xyz/gtwjqdvdao.html

[D11] 反转数组
来源：http://hz.xinyue.icu/gthsnolofg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.fzhhl.top/gthbsthcfq.html

PHP:  array_reverse($arr);
来源：http://hz.hnqzz.top/gtpbneqgai.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xylfe.cn/gthukqqbyg.html

TS:   [...arr].reverse();
来源：http://hz.snrcjt.cn/gtnjqbegmi.html

Java: Collections.reverse(list);
来源：http://hz.hnxiangtu.top/gtdqnhfbyf.html

Go:   slices.Reverse(arr)
来源：http://hz.aibaodan.cn/gticepqzdb.html

Ruby: arr.reverse
来源：http://hz.cheryme.top/gtfbfcupfd.html

C#:   list.Reverse();
来源：http://hz.jinqigufen.top/gtjquwgjaz.html

[D12] 查找元素下标
来源：http://hz.chenzaomai.com/gtjvovqaln.html

Py:   arr.index(x);  x in arr
来源：http://hz.cqqwz.cn/gtxltqqpgv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.smart0.xyz/gtkomlxdcd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangkeji.top/gthzbppjpm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhoulong.xyz/gtydtlobcq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhijiandao.cn/gtvjcqfthr.html

Go:   slices.Index(arr, x)
来源：http://hz.yj20258.top/gtszpblvue.html

Ruby: arr.index(x)
来源：http://hz.sweek.top/gtbagczmez.html

C#:   list.IndexOf(x);
来源：http://hz.chenjidiqi.icu/gthfpqhrli.html

[D13] 过滤（保留满足条件的）
来源：http://hz.vqdsnc.cn/gtvomyfgwu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ehwqpu.com/gtrmuvwtei.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yongpay.top/gtjkkhaojc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shuidangran.top/gtburtkxla.html

TS:   arr.filter(x => x > 3)
来源：http://hz.chenlongwang.top/gtvttlhimg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jyoumei.cn/gtmhqszoby.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xinyue.icu/gtvpfsulen.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.bjfxy.top/gtcyrfyfls.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinyuanbaomall.cn/gtnmpubvvz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ybcxt.top/gtlawykhuv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xylfe.cn/gtjkdiptau.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hysaishi.cn/gtvmtktard.html

JS:   arr.map(x => x * 2)
来源：http://hz.redwolf501.top/gtfprzzlkf.html

TS:   arr.map(x => x * 2)
来源：http://hz.shzxlz.cn/gtohnxmcsx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ehwqpu.com/gtyyfwixbn.html

Go:   // 手写循环
来源：http://hz.xinyue.icu/gteolhedun.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.meibo888.top/gtewmhjpcv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ppjwa.cn/gtkmfbqbvk.html

[D15] 去重
来源：http://hz.chenlongwang.top/gtqfbkliyu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yuanzhike.top/gtsuzqqzzz.html

PHP:  array_unique($arr);
来源：http://hz.hongshengwenyu.top/gtnptxmgpr.html

JS:   [...new Set(arr)]
来源：http://hz.aibaodan.cn/gtvqkqrgfi.html

TS:   [...new Set(arr)]
来源：http://hz.mhx1999.top/gtljmncqtv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.52xcode.cn/gtggvocrrc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.dashuyun.cn/gtrfedvwcb.html

Ruby: arr.uniq
来源：http://hz.jyoumei.cn/gtffvtqeju.html

C#:   list.Distinct().ToList()
来源：http://hz.jiagoushi.top/gtpxllvfci.html

[D16] 求和与平均值
来源：http://hz.yuanzhike.top/gtdumjvqeq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jianghu66.top/gtmbqdbehu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jyoumei.cn/gtozjxoann.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtmlhvcpjz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gtnwopmvfh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hysaishi.cn/gtskscxcer.html

Go:   // 手写循环累加
来源：http://hz.yonumen.top/gtqzgbirzh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhaomingkeji.xyz/gtxfauxegm.html

C#:   list.Sum();  list.Average()
来源：http://hz.svipenyu.cn/gtywjlsdjf.html

[D17] 最大值与最小值
来源：http://hz.shangyingyoupin.top/gtgvasiwyj.html

Py:   max(arr);  min(arr)
来源：http://hz.wangdashe.top/gtjadeftin.html

PHP:  max($arr);  min($arr);
来源：http://hz.xylfe.cn/gtkrymxztu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yueranfly.top/gtxwdxuzbz.html

TS:   Math.max(...arr);
来源：http://hz.mhx1999.top/gttxckoejo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhongyouzk.top/gtcajzedqx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guowangkeji.top/gthokitdid.html

Ruby: arr.max;  arr.min
来源：http://hz.zhongyouzk.top/gtrhevymcn.html

C#:   list.Max();  list.Min()
来源：http://hz.yanxiufei.cn/gtkthhcbyw.html

[D18] 扁平化嵌套数组
来源：http://hz.pycfn.com/gteajiteof.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jqgfzy.top/gtvrxsmuel.html

PHP:  array_merge(...$nested);
来源：http://hz.yonumen.top/gtvxaypede.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.tian-w.cn/gtzmiaoxhi.html

TS:   nested.flat();
来源：http://hz.birdmap.top/gtxdchbpcl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cucudq.cn/gtzbtoahnd.html

Go:   // 手写双层循环
来源：http://hz.pycfn.com/gtuwkfhuqk.html

Ruby: nested.flatten
来源：http://hz.jinyuanbaomall.cn/gtdegvdbvx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hammf.cn/gtdinyrjlh.html

[D19] 按字段分组
来源：http://hz.cashguo.top/gtuhuegndb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenzaomai.com/gtztahwrne.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ywan-chungtsiang.top/gtpsaafytn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shanyushiyangtech.top/gtmajyjtcw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.nwbrower.top/gtpnorvoer.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.vqdsnc.cn/gtcovxngjo.html

Go:   // 手写 map[string][]T
来源：http://hz.bjfxy.top/gtzvfmvjui.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hongshengwenyu.top/gtaojlotce.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shuidangran.top/gtctmxrqac.html

[D20] 统计每个元素出现次数
来源：http://hz.andypj.xyz/gtnxehoasb.html

Py:   Counter(arr)
来源：http://hz.0kj1m.cn/gtmqitxafp.html

PHP:  array_count_values($arr);
来源：http://hz.hysaishi.cn/gtnhatjkxi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tianlin.xyz/gtksgqlodq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuetiantiany.cn/gtawsvgbeg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cashguo.top/gtqxqqlmjv.html

Go:   // 手写 map[T]int
来源：http://hz.shzxlz.cn/gtgbprebrj.html

Ruby: arr.tally
来源：http://hz.tanke756.top/gtvtsdokvz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.pycfn.com/gtadwavwvo.html

[D21] 判断是否包含某元素
来源：http://hz.jiagoushi.top/gtimgxskri.html

Py:   x in arr
来源：http://hz.guannengcc.top/gtfeegrvxw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tanke756.top/gtcawsqsgn.html

JS:   arr.includes(x)
来源：http://hz.aibaodan.cn/gtfbsqpomp.html

TS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtugsmkxnj.html

Java: list.contains(x)
来源：http://hz.xylfe.cn/gtszfstjrc.html

Go:   slices.Contains(arr, x)
来源：http://hz.xuanzx.com/gtozczrdxn.html

Ruby: arr.include?(x)
来源：http://hz.xuanzx.com/gtrfbfvjsw.html

C#:   list.Contains(x)
来源：http://hz.smart0.xyz/gtvazmrbfl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ywan-chungtsiang.top/gtembvvrsk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yongpay.top/gtoutcckfh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.iojbl.cn/gtibfktply.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.tian-w.cn/gtqxzcswua.html

TS:   [...arr];
来源：http://hz.gzhubu.top/gtosojmcxw.html

Java: new ArrayList<>(list);
来源：http://hz.zhijiandao.cn/gtjrcfedcs.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.aizwys.cn/gtvaowjggf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.0kj1m.cn/gtfmibdqfz.html

C#:   new List<int>(list);
来源：http://hz.shanyushiyangkeji.top/gtgbwdijdz.html

[D23] reduce 累积计算
来源：http://hz.jinqigfzy.top/gttmmjbuoz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.shangyingyoupin.top/gtpzbaqthp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zdqjudy.top/gtsxovkqbo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinyuanbaomall.cn/gtczzihxfm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hfpthk.cn/gtqhiagvmb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yanxiufei.cn/gtrljzeoyw.html

Go:   // 手写循环
来源：http://hz.xylfe.cn/gtsgqlstos.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ivvv.top/gtfhtyqhxm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj202588.top/gtaztconln.html

[D24] 字典 / Map 基本操作
来源：http://hz.redwolf501.top/gtcfmbkfqh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.52xcode.cn/gtahqzvnlj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.tian-w.cn/gtbhyqgzeb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.dianchejie.cn/gtlrdiaobu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jyoumei.cn/gtkbkolzid.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xingfuxueyuan.xyz/gtasweulgi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhijiandao.cn/gtdimxbbln.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.snrcjt.cn/gttwnihxvr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gzhubu.top/gtwioltmjr.html

[D25] Set 集合去重与交并差
来源：http://hz.andypj.xyz/gtldjzwsnk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhaomingkeji.xyz/gtznbneapu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hnqzz.top/gtkoqtomci.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhixingplan.top/gtmtaincqy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yonumen.top/gtahgveqet.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zycfv.cn/gtysybfjuz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jqgufenzy.top/gtjqkhjwxj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.aibaodan.cn/gtzbndyjkj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhengqikj.top/gtwzsxothf.html

[D26] 数组转字符串
来源：http://hz.cucudq.cn/gtiqeffbbn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hammf.cn/gtpemrxmvi.html

PHP:  implode(", ", $arr);
来源：http://hz.guowangkeji.top/gtewcnzagy.html

JS:   arr.join(", ")
来源：http://hz.yj20258888.top/gtnrijdcrt.html

TS:   arr.join(", ")
来源：http://hz.zhoulong.xyz/gthevxoypc.html

Java: String.join(", ", list)
来源：http://hz.cucudq.cn/gtmtyhuysb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nanxinkj.top/gtupkqwtus.html

Ruby: arr.join(", ")
来源：http://hz.yangfankeji.com/gtsalscacs.html

C#:   string.Join(", ", list)
来源：http://hz.feifeiyinyue.top/gtpqgwxkwj.html


<!-- 参考信息 -->