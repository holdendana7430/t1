代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gzhubu.top/gtvyztpaqv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tianlin.xyz/gttaukznkv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yonumen.top/gtnieoehst.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhaomingkeji.xyz/gtdtllxwur.html

[C10] 变量作用域
来源：http://hz.52xcode.cn/gtytupqupe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.316326.xyz/gtomeudapp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.quarkkingdee.top/gtxdarhwja.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.guannengcc.top/gtudspvlzo.html

TS:   同 JS
来源：http://hz.cashguo.top/gtzuarakkz.html

Java: 方法内为块级作用域
来源：http://hz.jinghuilouyu.cn/gtpvguofjv.html

Go:   花括号块级作用域
来源：http://hz.jlsjyb.cn/gtzzcofqkq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.gogol.net.cn/gtthmxmkxl.html

C#:   块级作用域
来源：http://hz.smart0.xyz/gtcvxecrcr.html

[C11] 模块导入与导出
来源：http://hz.shangyingyoupin.top/gtuujgptfd.html

Py:   from module import func
来源：http://hz.nanxinkj.top/gtxhgflalf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tanke756.top/gttstcrolf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shuidangran.top/gtfkymukcy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.feifeiyinyue.top/gtoodnjodm.html

Java: import java.util.List;
来源：http://hz.yvedp.cn/gtlpxzpphh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gotoacloud.top/gtzwwhunoh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.svipenyu.cn/gtrsdaulps.html

C#:   using System.Text;
来源：http://hz.dianchejie.cn/gtmzzjwztc.html

[C12] 立即执行函数 IIFE
来源：http://hz.xylfe.cn/gtyanuload.html

Py:   (lambda: print("run"))()
来源：http://hz.sufxvd.cn/gtpnzqhqgy.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yonumen.top/gtonljafga.html

JS:   (() => { console.log("run"); })();
来源：http://hz.andypj.xyz/gtobeqtzpn.html

TS:   (() => { console.log("run"); })();
来源：http://hz.fengsongda.top/gtvcsyawfc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.svipenyu.cn/gtpwupvxqu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hfpthk.cn/gtezmrmjqc.html

Ruby: -> { puts "run" }.call
来源：http://hz.guowangkeji.top/gtiizorhij.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hnqzz.top/gtphpghwpg.html

[C13] 类型声明 / 类型注解
来源：http://hz.mhx1999.top/gtnlipaocl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hysaishi.cn/gtkwuiojsm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.andypj.xyz/gtoxegohmq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.wangshuangyany.cn/gtxtgjseub.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuetiantiany.cn/gtcbxbwiah.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj20258888.top/gtigsyyywj.html

Go:   func add(a, b int) int
来源：http://hz.chenjidiqi.icu/gtpcykqzbc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hysaishi.cn/gtzvocnzmi.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.quarkkingdee.top/gtrekijzxz.html

[C14] 泛型函数
来源：http://hz.daria6918.cn/gtffyadfvi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sxryk.cn/gtympxvubo.html

PHP:  // 无泛型
来源：http://hz.snrcjt.cn/gtpzgwmmle.html

JS:   // 无泛型
来源：http://hz.yj202588.top/gtrltbirqn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ybcxt.top/gtbigdvslw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhixingplan.top/gtsoivwpmj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zdqjudy.top/gtcvevfget.html

Ruby: # 无泛型
来源：http://hz.316326.xyz/gtqyuisjer.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhoulong.xyz/gtrwgknuxd.html

[C15] 解构 / 展开参数
来源：http://hz.cucudq.cn/gtmhresezs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.smart0.xyz/gtssdeuode.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ywan-chungtsiang.top/gtrqcianad.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yanxiufei.cn/gtxlqtitev.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.c1oappe.top/gtwxgizqmy.html

Java: // 无解构
来源：http://hz.wangdashe.top/gtvldengkz.html

Go:   // 无解构
来源：http://hz.tanke756.top/gtqiaizdfl.html

Ruby: a, b = pair
来源：http://hz.0kj1m.cn/gtvdznwhoq.html

C#:   var (a, b) = pair;
来源：http://hz.316326.xyz/gtxvlqlccb.html

[C16] 函数 / 方法重载
来源：http://hz.wangdashe.top/gthfumnuks.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hammf.cn/gtjozcfaxl.html

PHP:  // 无重载
来源：http://hz.ywan-chungtsiang.top/gtiwsmeert.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hnxiangtu.top/gttsqurkiq.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cashguo.top/gtteizgvxi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xylfe.cn/gtnkqzfaya.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhengqikj.top/gtvtbxhvry.html

Ruby: # 无重载：靠动态参数
来源：http://hz.dianchejie.cn/gtrkhaizbz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhongyouzk.top/gtbdycriic.html

================================================================================
来源：http://hz.gotoacloud.top/gtlvtlzmoz.html

D. 数组 / 列表 / 集合
来源：http://hz.haohaochexian.top/gtonpyjkny.html

================================================================================
来源：http://hz.sysykeji.top/gtwjzcqunp.html

[D01] 创建数组 / 列表
来源：http://hz.jyoumei.cn/gttyovvsql.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ivvv.top/gtfnlzbpqp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shanyushiyangkeji.top/gtnhkmhbry.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.iojbl.cn/gtndrczmon.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ppjwa.cn/gttogxlasr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yueranfly.top/gtlxhtiewl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ywan-chungtsiang.top/gtfpequpuz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.chenlongwang.top/gtukeicdzz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.guowangkeji.top/gtbsyuohzf.html

[D02] 追加元素到末尾
来源：http://hz.yuanzhike.top/gtnkhziahi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sufxvd.cn/gtbhnzjqev.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhengqikj.top/gtonzmumhu.html

JS:   arr.push(4);
来源：http://hz.guannengcc.top/gtmjhfzgpm.html

TS:   arr.push(4);
来源：http://hz.pengpengdd.cyou/gtqbopgcbl.html

Java: list.add(4);
来源：http://hz.shangyingyoupin.top/gtlvxzztog.html

Go:   arr = append(arr, 4)
来源：http://hz.tianlin.xyz/gtptecaprm.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yongpay.top/gtanrcltcj.html

C#:   list.Add(4);
来源：http://hz.zhiwuduotai.top/gtscixelvj.html

[D03] 在指定位置插入元素
来源：http://hz.zhaomingkeji.xyz/gtaczqikqr.html

Py:   arr.insert(0, 0)
来源：http://hz.zhengqikj.top/gtwjduhcbq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinghuilouyu.cn/gtxqsxszfa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xuetiantiany.cn/gtfqhebqlz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yanxiufei.cn/gtrewxejzp.html

Java: list.add(0, 0);
来源：http://hz.jlsjyb.cn/gtonfuvdxt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.vqdsnc.cn/gtzlggeqvp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.aizwys.cn/gtbycujbzr.html

C#:   list.Insert(0, 0);
来源：http://hz.cheryme.top/gthfnrdqme.html

[D04] 删除元素
来源：http://hz.birdmap.top/gtlqgdsybr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yuxming.cn/gtnhcmdfpb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.52xcode.cn/gtsthztdiz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.aibaodan.cn/gtemkljwsz.html

TS:   arr.splice(0, 1);
来源：http://hz.ydjk.org.cn/gtdvmzsqie.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhoulong.xyz/gtpkgyuxdc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yongpay.top/gtqzgbuvqs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yonumen.top/gthndpfuyf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hongshengwenyu.top/gtnxzrombc.html

[D05] 访问与修改元素
来源：http://hz.yj202588.top/gtamglkfmo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhoulong.xyz/gtviaazdib.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhiwuduotai.top/gtppujcbrg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hnqzz.top/gtkrlsciue.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.c1oappe.top/gtmclbybxa.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.9152youxi.cn/gtewfmuopt.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtkstidzkl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sufxvd.cn/gtaveiktkv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhongyouzk.top/gtykohpkdd.html

[D06] 数组长度
来源：http://hz.bjfxy.top/gtpxkratke.html

Py:   len(arr)
来源：http://hz.0kj1m.cn/gtwfygwlsb.html

PHP:  count($arr);
来源：http://hz.sxryk.cn/gtylyxltke.html

JS:   arr.length
来源：http://hz.hfpthk.cn/gtfdlqiiqn.html

TS:   arr.length
来源：http://hz.hysaishi.cn/gtwccacwsv.html

Java: list.size();
来源：http://hz.zhongyouzk.top/gtlmbmcbni.html

Go:   len(arr)
来源：http://hz.shanyushiyangtech.top/gtcwzftshp.html

Ruby: arr.length; arr.size
来源：http://hz.quarkkingdee.top/gtnnrdduiu.html

C#:   list.Count;
来源：http://hz.zhengqikj.top/gtcuooexmt.html

[D07] 切片 / 取子数组
来源：http://hz.cheryme.top/gtahejfrby.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ppjwa.cn/gtcqrwwczz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yonumen.top/gteqgemwos.html

JS:   arr.slice(1, 4);
来源：http://hz.ivvv.top/gtvrocsjhy.html

TS:   arr.slice(1, 4);
来源：http://hz.sufxvd.cn/gtdpjneeyp.html

Java: list.subList(1, 4);
来源：http://hz.zhixingplan.top/gtcffjnksd.html

Go:   arr[1:4]
来源：http://hz.jqgfzy.top/gtzszjxffk.html

Ruby: arr[1, 3]
来源：http://hz.quarkkingdee.top/gttefolgqa.html

C#:   list.GetRange(1, 3);
来源：http://hz.bjfxy.top/gtmehpefqk.html

[D08] 合并两个数组
来源：http://hz.chenzaomai.com/gtcqvrcpai.html

Py:   a + b;  a.extend(b)
来源：http://hz.birdmap.top/gtcbhbnflk.html

PHP:  array_merge($a, $b);
来源：http://hz.yvedp.cn/gtykhfdxgg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ivvv.top/gtomfkpliu.html

TS:   [...a, ...b];
来源：http://hz.tanke756.top/gtsqhmmiey.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.fzhhl.top/gtjptkgclh.html

Go:   append(a, b...)
来源：http://hz.sysykeji.top/gtnroumiwj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.tanke756.top/gtgoqjxmjf.html

C#:   a.Concat(b).ToList()
来源：http://hz.jiagoushi.top/gtkokycjay.html

[D09] 排序（升序）
来源：http://hz.jianghu66.top/gtpkcnpqif.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hnxiangtu.top/gtlwxddvev.html

PHP:  sort($arr);
来源：http://hz.haohaochexian.top/gtxdyvzstd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yuanzhike.top/gtipurmjaj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.daria6918.cn/gtvaqauyzr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shanyushiyangtech.top/gtuddvcjjt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jinghuilouyu.cn/gtgebowcnw.html

Ruby: arr.sort
来源：http://hz.meibo888.top/gtsvqozlgy.html

C#:   list.Sort();
来源：http://hz.jinghuilouyu.cn/gtwzsbusnb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ivvv.top/gtdgkjagsg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xingfuxueyuan.xyz/gtfipxcwtk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jianghu66.top/gtzsmccahs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.quarkkingdee.top/gtjebsrspn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangkeji.top/gtdkqvmjkf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.guowangkeji.top/gtcavprnru.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.kuanghao11.cn/gtvtfhyzdu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ywan-chungtsiang.top/gtptpcpasy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hfpthk.cn/gtooswvwsh.html

[D11] 反转数组
来源：http://hz.52xcode.cn/gtftxopjwu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhiwuduotai.top/gtdmgghxlk.html

PHP:  array_reverse($arr);
来源：http://hz.tanke756.top/gtjoqbkklw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yonumen.top/gticsyvngm.html

TS:   [...arr].reverse();
来源：http://hz.zhongyouzk.top/gtakzenzry.html

Java: Collections.reverse(list);
来源：http://hz.jinyuanbaomall.cn/gtqcgxdupk.html

Go:   slices.Reverse(arr)
来源：http://hz.jinqigufen.top/gtaacryapn.html

Ruby: arr.reverse
来源：http://hz.hfpthk.cn/gtbhgrobce.html

C#:   list.Reverse();
来源：http://hz.hnxiangtu.top/gtejkazbrx.html

[D12] 查找元素下标
来源：http://hz.jyoumei.cn/gtdjrwsino.html

Py:   arr.index(x);  x in arr
来源：http://hz.fengsongda.top/gtusmtpsdn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.dashuyun.cn/gtuuuglwfy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnqzz.top/gteojkatas.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jiagoushi.top/gtdmrblwbi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhoulong.xyz/gtzasrplmb.html

Go:   slices.Index(arr, x)
来源：http://hz.hysaishi.cn/gtrcsifbmv.html

Ruby: arr.index(x)
来源：http://hz.0kj1m.cn/gtplhdkzrs.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangtech.top/gtojtqwdox.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sxryk.cn/gtzwqdprge.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenjidiqi.icu/gtqhamfmvm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.wangdashe.top/gtpakmkytu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangkeji.top/gtecfyqwyk.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhongyouzk.top/gtvodeafcp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ydjk.org.cn/gtucstyyas.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ydjk.org.cn/gtxqnkolfy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yongpay.top/gtwrsxbkny.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.feifeiyinyue.top/gtrfryajyb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tianlin.xyz/gtuwtmtssm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.redwolf501.top/gtplfxslpi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cheryme.top/gtycvhxfnu.html

JS:   arr.map(x => x * 2)
来源：http://hz.nanxuanxn.top/gtvhytwagg.html

TS:   arr.map(x => x * 2)
来源：http://hz.cdnleiting.top/gtjigahptr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xuetiantiany.cn/gtlplucmmb.html

Go:   // 手写循环
来源：http://hz.andypj.xyz/gtfapndklg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yj20258888.top/gtyafjktdp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yuanzhike.top/gtriczlhal.html

[D15] 去重
来源：http://hz.xziqi.cn/gtifaifmsb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sxryk.cn/gtzvokmfvg.html

PHP:  array_unique($arr);
来源：http://hz.yj202588.top/gttoydyijr.html

JS:   [...new Set(arr)]
来源：http://hz.vqdsnc.cn/gtrhedmytg.html

TS:   [...new Set(arr)]
来源：http://hz.fengsongda.top/gtpwtwaecm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cdnleiting.top/gtnhkqhpad.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.andypj.xyz/gtnrryocbp.html

Ruby: arr.uniq
来源：http://hz.yueranfly.top/gtbhhuoqee.html

C#:   list.Distinct().ToList()
来源：http://hz.zhoulong.xyz/gtavxozocd.html

[D16] 求和与平均值
来源：http://hz.jinyuanbaomall.cn/gtrjrcdmgm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtmhcocwmk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xuanzx.com/gtupnnhtsq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pycfn.com/gtnouusooq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ehwqpu.com/gthnibgkll.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sxryk.cn/gtsnnbucbs.html

Go:   // 手写循环累加
来源：http://hz.meibo888.top/gtxlmefgmj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hongshengwenyu.top/gtodituomn.html

C#:   list.Sum();  list.Average()
来源：http://hz.hongshengwenyu.top/gtnbpmgkdc.html

[D17] 最大值与最小值
来源：http://hz.mhx1999.top/gtqkkyeonb.html

Py:   max(arr);  min(arr)
来源：http://hz.shanyushiyangkeji.top/gtfffdvvsv.html

PHP:  max($arr);  min($arr);
来源：http://hz.guannengcc.top/gtyqrwehul.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.9152youxi.cn/gtkfuqfkrj.html

TS:   Math.max(...arr);
来源：http://hz.snrcjt.cn/gtbkoafapy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sysykeji.top/gtamgllcqo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinyuanbaomall.cn/gtbhbaxkcx.html

Ruby: arr.max;  arr.min
来源：http://hz.nwbrower.top/gtczrbrmlx.html

C#:   list.Max();  list.Min()
来源：http://hz.fzhhl.top/gtzhffrahh.html

[D18] 扁平化嵌套数组
来源：http://hz.jqgfzy.top/gtfjdsgaln.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.316326.xyz/gtedprqswf.html

PHP:  array_merge(...$nested);
来源：http://hz.jinghuilouyu.cn/gtihjlgzsf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sysykeji.top/gtmwtjsggp.html

TS:   nested.flat();
来源：http://hz.gzhubu.top/gtwgtpzlbh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nanxuanxn.top/gtbgpyftqf.html

Go:   // 手写双层循环
来源：http://hz.xylfe.cn/gtbnezobyj.html

Ruby: nested.flatten
来源：http://hz.yonumen.top/gtxsxzgevf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinghuilouyu.cn/gtmqhuxszh.html

[D19] 按字段分组
来源：http://hz.yvedp.cn/gtqdlltdpp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.kuanghao11.cn/gthkmosfea.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yangfankeji.com/gteiojrpia.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jlsjyb.cn/gtdhwwnvkk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ydjk.org.cn/gtmriarvvm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gotoacloud.top/gtupubxwzt.html

Go:   // 手写 map[string][]T
来源：http://hz.xuetiantiany.cn/gtbczfqtoz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.svipenyu.cn/gtzidamfkf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xziqi.cn/gtuuithdkp.html

[D20] 统计每个元素出现次数
来源：http://hz.smart0.xyz/gtumbpfwdk.html

Py:   Counter(arr)
来源：http://hz.shzxlz.cn/gtuvjjvqkf.html

PHP:  array_count_values($arr);
来源：http://hz.hongshengwenyu.top/gtfdaphblw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258888.top/gtipayojfr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sufxvd.cn/gtblaywkez.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.guowangkeji.top/gtzbfeefgd.html

Go:   // 手写 map[T]int
来源：http://hz.jlsjyb.cn/gtedvhvjfb.html

Ruby: arr.tally
来源：http://hz.ybcxt.top/gtvjgnitzc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.daxiang520.top/gtwgmwxzaf.html

[D21] 判断是否包含某元素
来源：http://hz.quarkkingdee.top/gtipsroeta.html

Py:   x in arr
来源：http://hz.shanyushiyangtech.top/gtxhbkkeri.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhaomingkeji.xyz/gtetwkffwo.html

JS:   arr.includes(x)
来源：http://hz.quarkkingdee.top/gtwsgoedej.html

TS:   arr.includes(x)
来源：http://hz.chenzaomai.com/gtighsedum.html

Java: list.contains(x)
来源：http://hz.snrcjt.cn/gthjcehyre.html

Go:   slices.Contains(arr, x)
来源：http://hz.meibo888.top/gtqzfypqpd.html

Ruby: arr.include?(x)
来源：http://hz.daxiang520.top/gtlcprekmy.html

C#:   list.Contains(x)
来源：http://hz.316326.xyz/gtxeiwzicj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yj20258.top/gtszelkhmu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yueranfly.top/gtrdrjvhjm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.snrcjt.cn/gtjbwkocee.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sysykeji.top/gtmgneogwr.html

TS:   [...arr];
来源：http://hz.shuidangran.top/gtoygsjdju.html

Java: new ArrayList<>(list);
来源：http://hz.yuanzhike.top/gtoajxnwck.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.quarkkingdee.top/gtfwrmpuwp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shangyingyoupin.top/gtzbasxqvp.html

C#:   new List<int>(list);
来源：http://hz.jinyuanbaomall.cn/gtteehgufm.html

[D23] reduce 累积计算
来源：http://hz.cdnleiting.top/gtyauiogbk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gaohongyu789.top/gtsiewsjsk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.kuanghao11.cn/gtxjiqfscm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guannengcc.top/gtlhyjzood.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxinkj.top/gtklheuabn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gogol.net.cn/gtxldvxdjx.html

Go:   // 手写循环
来源：http://hz.chenzaomai.com/gtubkdskfe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zycfv.cn/gtithmhnzj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.feifeiyinyue.top/gtcfjjyvgk.html

[D24] 字典 / Map 基本操作
来源：http://hz.sufxvd.cn/gtmkjtdblb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.feifeiyinyue.top/gtvuiurvgs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.pengpengdd.cyou/gtjxqgziwj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ywan-chungtsiang.top/gtsybejxgc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.feifeiyinyue.top/gtzfaxjlgv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenzaomai.com/gthjddzudw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ehwqpu.com/gtpfgwlszh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.andypj.xyz/gtwehblxii.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shanyushiyangtech.top/gtrodlmbqj.html

[D25] Set 集合去重与交并差
来源：http://hz.chenlongwang.top/gtatexhpit.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yonumen.top/gtyxzmenqs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xuanzx.com/gthtkaxaqp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sufxvd.cn/gtespgverh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jlsjyb.cn/gtjlzumpqu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shanyushiyangtech.top/gtgpunyfhn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.iojbl.cn/gtplkqpgwa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.0kj1m.cn/gtdmukmesr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hnqzz.top/gtsygreoku.html

[D26] 数组转字符串
来源：http://hz.zhijiandao.cn/gtrkyukfvz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.svipenyu.cn/gtndpdmemi.html

PHP:  implode(", ", $arr);
来源：http://hz.jiagoushi.top/gtjafpsuus.html

JS:   arr.join(", ")
来源：http://hz.zdqjudy.top/gtxdvlhiph.html

TS:   arr.join(", ")
来源：http://hz.tanke756.top/gttisekakg.html


<!-- 参考信息 -->