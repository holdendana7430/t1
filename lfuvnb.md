代发 wailian999

TS:   同 JS
来源：http://hz.wangdashe.top/gtjvjkmzub.html

Java: 方法内为块级作用域
来源：http://hz.ehwqpu.com/gtovrbhwft.html

Go:   花括号块级作用域
来源：http://hz.havefunace.top/gtskbqklew.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.havefunace.top/gthptbzdjx.html

C#:   块级作用域
来源：http://hz.yangfankeji.com/gttvfdmyjg.html

[C11] 模块导入与导出
来源：http://hz.fengsongda.top/gttzrlidwg.html

Py:   from module import func
来源：http://hz.yj20258.top/gtxujzpszg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.9152youxi.cn/gtkgxmonkj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.nanxuanxn.top/gtvwnkwfvc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.c1oappe.top/gtkrcqypbe.html

Java: import java.util.List;
来源：http://hz.xingfuxueyuan.xyz/gtcqpbmgsf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ywan-chungtsiang.top/gtvmcnqsyk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shzxlz.cn/gthldxokog.html

C#:   using System.Text;
来源：http://hz.iojbl.cn/gtftuamxhj.html

[C12] 立即执行函数 IIFE
来源：http://hz.yvedp.cn/gtessmifdq.html

Py:   (lambda: print("run"))()
来源：http://hz.chenlongwang.top/gtkdcmdgjy.html

PHP:  (function () { echo "run"; })();
来源：http://hz.feifeiyinyue.top/gticqhfyiq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangkeji.top/gttnhyshwj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yj20258.top/gtyjjhtvbj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.andypj.xyz/gtzjexmlub.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ydzc1.top/gtmevqgvay.html

Ruby: -> { puts "run" }.call
来源：http://hz.meibo888.top/gtjcutuhwp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yvedp.cn/gtvyxtqpet.html

[C13] 类型声明 / 类型注解
来源：http://hz.yuxming.cn/gtwgcymswh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jiagoushi.top/gtslygjfrc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.birdmap.top/gtpderwssg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.kuanghao11.cn/gtuagvpcbv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sweek.top/gtntcwnlki.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.tanke756.top/gtprpleayh.html

Go:   func add(a, b int) int
来源：http://hz.ivvv.top/gttxacyygj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hnxiangtu.top/gtniwebjek.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.nanxuanxn.top/gtjgzujwig.html

[C14] 泛型函数
来源：http://hz.kuanghao11.cn/gtmpbqocuo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.redwolf501.top/gtmaynlwqx.html

PHP:  // 无泛型
来源：http://hz.guannengcc.top/gtfwqaedee.html

JS:   // 无泛型
来源：http://hz.mhx1999.top/gtxstjvzfc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.nwbrower.top/gtawbhtden.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xinyue.icu/gtlbhcbdhg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.feifeiyinyue.top/gtolkespbr.html

Ruby: # 无泛型
来源：http://hz.shanyushiyangtech.top/gtyvnuqeai.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jiagoushi.top/gtnsfoidua.html

[C15] 解构 / 展开参数
来源：http://hz.andypj.xyz/gtmalnbmbw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zycfv.cn/gtwdvbbtrp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jqgufenzy.top/gtukngoijs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.feifeiyinyue.top/gtslkshhpa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinghuilouyu.cn/gtmwblchlb.html

Java: // 无解构
来源：http://hz.zhongyouzk.top/gtcpyiayxb.html

Go:   // 无解构
来源：http://hz.meibo888.top/gtrgomzady.html

Ruby: a, b = pair
来源：http://hz.jyoumei.cn/gtbsyyjnpo.html

C#:   var (a, b) = pair;
来源：http://hz.chenjidiqi.icu/gtvgykczir.html

[C16] 函数 / 方法重载
来源：http://hz.zdqjudy.top/gtvwuaatqk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.dianchejie.cn/gtjroabubb.html

PHP:  // 无重载
来源：http://hz.jqgfzy.top/gtszitbeai.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hysaishi.cn/gtntecqsbn.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yueranfly.top/gtqvmmoiia.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sufxvd.cn/gtunbtrsyg.html

Go:   // 无重载：用不同函数名
来源：http://hz.aizwys.cn/gtmkxyrkwa.html

Ruby: # 无重载：靠动态参数
来源：http://hz.pengpengdd.cyou/gtoxrjhszx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.wangshuangyany.cn/gtdyotxfkj.html

================================================================================
来源：http://hz.pycfn.com/gtvltusvfh.html

D. 数组 / 列表 / 集合
来源：http://hz.yj20258888.top/gtahlodwte.html

================================================================================
来源：http://hz.pycfn.com/gtnokfcaqt.html

[D01] 创建数组 / 列表
来源：http://hz.hammf.cn/gtblmqurvc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenzaomai.com/gtgcwfmdgz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ehwqpu.com/gtuzmofxgq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hnqzz.top/gtihjfhavi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ppjwa.cn/gtonqvezlg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guowangkeji.top/gtaeqhuvef.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhixingplan.top/gtbhqnlouw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangshuangyany.cn/gtqrsexezs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gogol.net.cn/gtkcwgobsc.html

[D02] 追加元素到末尾
来源：http://hz.haohaochexian.top/gtxuhhgqua.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yvedp.cn/gtzrlalcwv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhijiandao.cn/gtxjoszhad.html

JS:   arr.push(4);
来源：http://hz.dianchejie.cn/gtdejvxpdf.html

TS:   arr.push(4);
来源：http://hz.316326.xyz/gtglkvcaay.html

Java: list.add(4);
来源：http://hz.xylfe.cn/gtlbsdchnb.html

Go:   arr = append(arr, 4)
来源：http://hz.0kj1m.cn/gtvrwqfoml.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.birdmap.top/gtpcszlmli.html

C#:   list.Add(4);
来源：http://hz.ehwqpu.com/gtnwmumxgy.html

[D03] 在指定位置插入元素
来源：http://hz.shangyingyoupin.top/gtoxsovxzm.html

Py:   arr.insert(0, 0)
来源：http://hz.shzxlz.cn/gtogyrnyji.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xinyue.icu/gtnbmkzdsh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.daxiang520.top/gtactfdxhr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cheryme.top/gtmvukgmig.html

Java: list.add(0, 0);
来源：http://hz.xuetiantiany.cn/gtgrqyhfhf.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinqigfzy.top/gtpqofqqlu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.wangshuangyany.cn/gtxaanofev.html

C#:   list.Insert(0, 0);
来源：http://hz.wangshuangyany.cn/gtdchczhuq.html

[D04] 删除元素
来源：http://hz.sysykeji.top/gtotzuetwe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hongshengwenyu.top/gthrjepnro.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.pycfn.com/gtlluukbru.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gotoacloud.top/gtcvhzojhi.html

TS:   arr.splice(0, 1);
来源：http://hz.sufxvd.cn/gtvvdpjmbl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.52xcode.cn/gtkmwfoahl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.pycfn.com/gtfkvqrbgo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.fengsongda.top/gttmpppuwb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shzxlz.cn/gtjrqntqnd.html

[D05] 访问与修改元素
来源：http://hz.nwbrower.top/gtiafzrsiw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtndlbqtbw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.iojbl.cn/gtswimvqbv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.nanxuanxn.top/gtmdsbpucx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.meibo888.top/gtxgudtqsw.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tian-w.cn/gtooaneczo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.chenzaomai.com/gtxaerncmf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxinkj.top/gtezuaxcdp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.guowangkeji.top/gtovogdhat.html

[D06] 数组长度
来源：http://hz.wangdashe.top/gtsxunqxdc.html

Py:   len(arr)
来源：http://hz.hammf.cn/gtnlmafaog.html

PHP:  count($arr);
来源：http://hz.yangfankeji.com/gtrlznxjwj.html

JS:   arr.length
来源：http://hz.tianlin.xyz/gtmykwfxuk.html

TS:   arr.length
来源：http://hz.redwolf501.top/gtejfwtsze.html

Java: list.size();
来源：http://hz.cdnleiting.top/gtxdtiauoi.html

Go:   len(arr)
来源：http://hz.xinyue.icu/gtybpoqrfz.html

Ruby: arr.length; arr.size
来源：http://hz.yongpay.top/gtlpftpvnj.html

C#:   list.Count;
来源：http://hz.vqdsnc.cn/gtbqhvksaz.html

[D07] 切片 / 取子数组
来源：http://hz.yj20258888.top/gtgnpufior.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xuetiantiany.cn/gtexgdclrw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.guannengcc.top/gtywzalqlc.html

JS:   arr.slice(1, 4);
来源：http://hz.kuanghao11.cn/gtnrggpyij.html

TS:   arr.slice(1, 4);
来源：http://hz.jinghuilouyu.cn/gtoworyrlq.html

Java: list.subList(1, 4);
来源：http://hz.mhx1999.top/gtrmgywdxe.html

Go:   arr[1:4]
来源：http://hz.shanyushiyangtech.top/gtjfuzajup.html

Ruby: arr[1, 3]
来源：http://hz.jinghuilouyu.cn/gtrwrnddvz.html

C#:   list.GetRange(1, 3);
来源：http://hz.feifeiyinyue.top/gtxrjghxmf.html

[D08] 合并两个数组
来源：http://hz.ivvv.top/gtpzpfijff.html

Py:   a + b;  a.extend(b)
来源：http://hz.hammf.cn/gtkwxcpahe.html

PHP:  array_merge($a, $b);
来源：http://hz.xuanzx.com/gtkxemnxnh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hammf.cn/gtfayxlgmx.html

TS:   [...a, ...b];
来源：http://hz.daxiang520.top/gtpojhbxsd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yj202588.top/gtfzekpfhk.html

Go:   append(a, b...)
来源：http://hz.jqgfzy.top/gtlczbmftx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.chenzaomai.com/gtrsybbxha.html

C#:   a.Concat(b).ToList()
来源：http://hz.haohaochexian.top/gtwuklsrbw.html

[D09] 排序（升序）
来源：http://hz.zycfv.cn/gtyhrmjrhx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hysaishi.cn/gtiegsnahu.html

PHP:  sort($arr);
来源：http://hz.shanyushiyangtech.top/gtyvbalanp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.andypj.xyz/gtfdnewvxr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xuanzx.com/gtnjlvshsd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.chenlongwang.top/gtaqdejvxa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jinyuanbaomall.cn/gtglroqlpb.html

Ruby: arr.sort
来源：http://hz.guowangkeji.top/gtbdbblvhd.html

C#:   list.Sort();
来源：http://hz.sysykeji.top/gtsbahygpe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xuanzx.com/gtblaibuhu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yj20258888.top/gtonsfcdmi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fengsongda.top/gtcyzsrcle.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cqqwz.cn/gtxoucnqfx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.9152youxi.cn/gtmbvrdzzb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xingfuxueyuan.xyz/gtmotamrkh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.bjfxy.top/gttfamqsej.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.9152youxi.cn/gtlvkezpfq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cashguo.top/gtbcjapwul.html

[D11] 反转数组
来源：http://hz.cucudq.cn/gtidyfwtqy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zdqjudy.top/gtbycguily.html

PHP:  array_reverse($arr);
来源：http://hz.yj20258888.top/gtrsbxbjgt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.aibaodan.cn/gtncwynuzc.html

TS:   [...arr].reverse();
来源：http://hz.chenzaomai.com/gtspiagkgu.html

Java: Collections.reverse(list);
来源：http://hz.52xcode.cn/gtxjjjwmfb.html

Go:   slices.Reverse(arr)
来源：http://hz.jqgufenzy.top/gtbhnbxmjr.html

Ruby: arr.reverse
来源：http://hz.jinqigufen.top/gtnjahgpjx.html

C#:   list.Reverse();
来源：http://hz.sysykeji.top/gtxzrzipfd.html

[D12] 查找元素下标
来源：http://hz.yj20258888.top/gtmfuxfoqq.html

Py:   arr.index(x);  x in arr
来源：http://hz.sufxvd.cn/gtxqkgpsgr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.svipenyu.cn/gtogubutpa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnqzz.top/gtlxiilnfd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sxryk.cn/gtnmybwduh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhengqikj.top/gtqqsnhfgh.html

Go:   slices.Index(arr, x)
来源：http://hz.shzxlz.cn/gtcfvbobvh.html

Ruby: arr.index(x)
来源：http://hz.jinqigfzy.top/gtjpjrpsyo.html

C#:   list.IndexOf(x);
来源：http://hz.guannengcc.top/gtxxgjsyia.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jqgfzy.top/gtfmyhjboz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.feifeiyinyue.top/gtwdlgvmjo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.bjfxy.top/gtfozgykev.html

JS:   arr.filter(x => x > 3)
来源：http://hz.cucudq.cn/gtwoomoelx.html

TS:   arr.filter(x => x > 3)
来源：http://hz.birdmap.top/gthpzboqkx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.snrcjt.cn/gtrjeiydzn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.wangshuangyany.cn/gtqblupnwu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jyoumei.cn/gtwjxabfjr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.kuanghao11.cn/gtcvttacov.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hysaishi.cn/gtsmfrjnij.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.0kj1m.cn/gtfqxxqbxn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yj20258.top/gtwvdyryfi.html

JS:   arr.map(x => x * 2)
来源：http://hz.gogol.net.cn/gtzwjphjhe.html

TS:   arr.map(x => x * 2)
来源：http://hz.sxryk.cn/gtmjtriaeb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.316326.xyz/gtrhkcqrap.html

Go:   // 手写循环
来源：http://hz.jqgufenzy.top/gtutzzftml.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xziqi.cn/gtzacayped.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.redwolf501.top/gteovdoxnt.html

[D15] 去重
来源：http://hz.kuanghao11.cn/gtrxdezebn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.quarkkingdee.top/gtmnloqqzn.html

PHP:  array_unique($arr);
来源：http://hz.hywenlv.cn/gtvwaygoyv.html

JS:   [...new Set(arr)]
来源：http://hz.jiagoushi.top/gtmjgfrqta.html

TS:   [...new Set(arr)]
来源：http://hz.ydjk.org.cn/gtqosxvyxi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.chenzaomai.com/gtuxmbntkg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pengpengdd.cyou/gtteilokth.html

Ruby: arr.uniq
来源：http://hz.cashguo.top/gtxpjneiwy.html

C#:   list.Distinct().ToList()
来源：http://hz.jinghuilouyu.cn/gtjliesduu.html

[D16] 求和与平均值
来源：http://hz.mhx1999.top/gtcgkzorsw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.tanke756.top/gtcchljour.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xinyue.icu/gtvmnlinpz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.mhx1999.top/gtfwfepupo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhijiandao.cn/gtbocdnjhc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shzxlz.cn/gtkcsjozdr.html

Go:   // 手写循环累加
来源：http://hz.hnxiangtu.top/gtoxbfbahx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shanyushiyangkeji.top/gtcweuwjyz.html

C#:   list.Sum();  list.Average()
来源：http://hz.shanyushiyangtech.top/gtbkbzzpbr.html

[D17] 最大值与最小值
来源：http://hz.zhengqikj.top/gtljbejnjy.html

Py:   max(arr);  min(arr)
来源：http://hz.yangfankeji.com/gtyakykoxb.html

PHP:  max($arr);  min($arr);
来源：http://hz.guannengcc.top/gtgekeprjc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.fengsongda.top/gtnyfgmfha.html

TS:   Math.max(...arr);
来源：http://hz.vqdsnc.cn/gtxidkinra.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.birdmap.top/gtuvgvilif.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.meibo888.top/gtrixwgiaa.html

Ruby: arr.max;  arr.min
来源：http://hz.tianlin.xyz/gtecghjgpq.html

C#:   list.Max();  list.Min()
来源：http://hz.zhaomingkeji.xyz/gtfmhyjnog.html

[D18] 扁平化嵌套数组
来源：http://hz.yj20258.top/gtatfsdycl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nanxinkj.top/gtjntwttsd.html

PHP:  array_merge(...$nested);
来源：http://hz.guannengcc.top/gtgydwhzkg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xingfuxueyuan.xyz/gtatpccznj.html

TS:   nested.flat();
来源：http://hz.xingfuxueyuan.xyz/gtyeolbuki.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zycfv.cn/gtcmhkhfdy.html

Go:   // 手写双层循环
来源：http://hz.gotoacloud.top/gtgbjlhpds.html

Ruby: nested.flatten
来源：http://hz.yuanzhike.top/gtwyexxyiu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gaohongyu789.top/gtmzpmdoni.html

[D19] 按字段分组
来源：http://hz.gaohongyu789.top/gtkfzcvajh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hnxiangtu.top/gtfbuelofy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jlsjyb.cn/gtaqkkwznm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinqigufen.top/gtqudmspaq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.haohaochexian.top/gtpmudfbbv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hnqzz.top/gtntmqhgfu.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgfzy.top/gtjjbajmyw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.chenjidiqi.icu/gtrawxsxjr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.chenjidiqi.icu/gtbrmhcopb.html

[D20] 统计每个元素出现次数
来源：http://hz.ydjk.org.cn/gtnksmwbrm.html

Py:   Counter(arr)
来源：http://hz.zhixingplan.top/gtxcumiqmm.html

PHP:  array_count_values($arr);
来源：http://hz.shuidangran.top/gtcrmtorwy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hongshengwenyu.top/gtmxomhppw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.feifeiyinyue.top/gtedljfauo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.nanxuanxn.top/gtrqfacjcm.html

Go:   // 手写 map[T]int
来源：http://hz.yuxming.cn/gtuimzwqfu.html

Ruby: arr.tally
来源：http://hz.jinqigufen.top/gtvyhaltgd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nwbrower.top/gtfbgdbvwa.html

[D21] 判断是否包含某元素
来源：http://hz.ppjwa.cn/gtcmlxpgel.html

Py:   x in arr
来源：http://hz.tanke756.top/gtwwkyarpj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yj20258.top/gtvikjabba.html

JS:   arr.includes(x)
来源：http://hz.hnxiangtu.top/gtriwqrzcr.html

TS:   arr.includes(x)
来源：http://hz.zycfv.cn/gtqdywoxtu.html

Java: list.contains(x)
来源：http://hz.aibaodan.cn/gticyhczet.html

Go:   slices.Contains(arr, x)
来源：http://hz.zycfv.cn/gtbvvzzyco.html

Ruby: arr.include?(x)
来源：http://hz.zhixingplan.top/gtuzxvqmgc.html

C#:   list.Contains(x)
来源：http://hz.hysaishi.cn/gtdmzqbjcd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinqigfzy.top/gtqwkcxkwl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ppjwa.cn/gtnoegeosv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jqgufenzy.top/gtvljojngm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ivvv.top/gtvjsmmoof.html

TS:   [...arr];
来源：http://hz.zycfv.cn/gtghqhiknh.html

Java: new ArrayList<>(list);
来源：http://hz.0kj1m.cn/gtpikrwcrg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.wangdashe.top/gtgclvpruu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.pengpengdd.cyou/gtazeutbwt.html

C#:   new List<int>(list);
来源：http://hz.jianghu66.top/gthkrwlbvz.html

[D23] reduce 累积计算
来源：http://hz.gzhubu.top/gtbonowzbi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.feifeiyinyue.top/gtkmqgdtiu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hfpthk.cn/gtsqcvxwjy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shangyingyoupin.top/gtlxlcmzwr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ppjwa.cn/gtahysnykz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnqzz.top/gtaebvhlww.html

Go:   // 手写循环
来源：http://hz.feifeiyinyue.top/gtecubabrn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.9152youxi.cn/gtfinquphy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xuanzx.com/gtwzbyvjvc.html

[D24] 字典 / Map 基本操作
来源：http://hz.mhx1999.top/gtybdmzdcp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.tianlin.xyz/gtivdkdnpt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yanxiufei.cn/gtqlrflkjk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gaohongyu789.top/gtcmdlpqqq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shanyushiyangkeji.top/gtlqdonjls.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gzhubu.top/gtolokyimi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jlsjyb.cn/gtudpfvvxz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jyoumei.cn/gtdpdbvkaj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yuanzhike.top/gtntircyrj.html

[D25] Set 集合去重与交并差
来源：http://hz.nanxuanxn.top/gtmnkljaea.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cashguo.top/gtuyrqnvav.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.aibaodan.cn/gtmdztqkgi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.bjfxy.top/gtnqfwyjkb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhijiandao.cn/gtgsucsgje.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.wangdashe.top/gtkwhuvlii.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xylfe.cn/gtovwqrngt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.havefunace.top/gtbupavhxd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.chenlongwang.top/gtpzxsuogz.html

[D26] 数组转字符串
来源：http://hz.quarkkingdee.top/gtamrnaxis.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sxryk.cn/gtlbolknee.html

PHP:  implode(", ", $arr);
来源：http://hz.yonumen.top/gtxyhyqnlp.html

JS:   arr.join(", ")
来源：http://hz.xuanzx.com/gtqiaotujk.html

TS:   arr.join(", ")
来源：http://hz.cqqwz.cn/gtxnfoztxs.html

Java: String.join(", ", list)
来源：http://hz.zycfv.cn/gtpqopmjca.html

Go:   strings.Join(strs, ", ")
来源：http://hz.kuanghao11.cn/gtnxjkqhhl.html

Ruby: arr.join(", ")
来源：http://hz.gogol.net.cn/gtxbsnnblu.html

C#:   string.Join(", ", list)
来源：http://hz.yj20258888.top/gtpjijudyc.html

================================================================================
来源：http://hz.yj20258.top/gtscodahav.html

E. 字符串处理
来源：http://hz.aizwys.cn/gtrgcfmrpq.html

================================================================================
来源：http://hz.fengsongda.top/gttembdwqq.html

[E01] 拼接字符串
来源：http://hz.aibaodan.cn/gtsrldvpyw.html


<!-- 参考信息 -->