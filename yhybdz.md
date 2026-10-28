代发 wailian999

TS:   同 JS
来源：http://hz.yangfankeji.com/gtwkfxvnkw.html

Java: 方法内为块级作用域
来源：http://hz.daxiang520.top/gtybkyzlrt.html

Go:   花括号块级作用域
来源：http://hz.hnqzz.top/gtqoycphpo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hnxiangtu.top/gtuafcttak.html

C#:   块级作用域
来源：http://hz.fzhhl.top/gtouqlmrbr.html

[C11] 模块导入与导出
来源：http://hz.ydjk.org.cn/gtbqhorlwl.html

Py:   from module import func
来源：http://hz.jqgfzy.top/gtlzqfiouu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.9152youxi.cn/gtynpwtzty.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yueranfly.top/gtcssocivh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yj202588.top/gtbmxyesjz.html

Java: import java.util.List;
来源：http://hz.yangfankeji.com/gtzykgsepq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cqqwz.cn/gtutqrromc.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ywan-chungtsiang.top/gtxkzfhtmm.html

C#:   using System.Text;
来源：http://hz.c1oappe.top/gtxegglntp.html

[C12] 立即执行函数 IIFE
来源：http://hz.ppjwa.cn/gtmnflidez.html

Py:   (lambda: print("run"))()
来源：http://hz.pengpengdd.cyou/gteniupapn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shuidangran.top/gtmukcwknh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.redwolf501.top/gtxpqgcwpg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ppjwa.cn/gtnawmgtsd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.birdmap.top/gtqwjxakqo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.smart0.xyz/gtxhahlmsv.html

Ruby: -> { puts "run" }.call
来源：http://hz.pycfn.com/gteglygvnm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.quarkkingdee.top/gtfsuzdxwl.html

[C13] 类型声明 / 类型注解
来源：http://hz.daxiang520.top/gtbcdfaudd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shuidangran.top/gtchoxsqvp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fengsongda.top/gtedenlnqb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.svipenyu.cn/gtflvkncpw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhoulong.xyz/gtsgtetgcx.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.316326.xyz/gtvekvdwkv.html

Go:   func add(a, b int) int
来源：http://hz.yuxming.cn/gtjdosudsi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ydzc1.top/gtryxfoekx.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yuxming.cn/gtvjjerwtk.html

[C14] 泛型函数
来源：http://hz.shuidangran.top/gtcqqhqcsh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhengqikj.top/gtuvuwnavk.html

PHP:  // 无泛型
来源：http://hz.jiagoushi.top/gtnqnbeazc.html

JS:   // 无泛型
来源：http://hz.hysaishi.cn/gtqygkzjie.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yuanzhike.top/gtgsfjplst.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gotoacloud.top/gtooayinhj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gotoacloud.top/gtmayruhay.html

Ruby: # 无泛型
来源：http://hz.316326.xyz/gtqcjcacqv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.dashuyun.cn/gtezaqetzb.html

[C15] 解构 / 展开参数
来源：http://hz.fzhhl.top/gtgcgoqhln.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gotoacloud.top/gtfzobjghz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhiwuduotai.top/gtqvysqozp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.guannengcc.top/gthjzgntwx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.pengpengdd.cyou/gtitfllows.html

Java: // 无解构
来源：http://hz.sxryk.cn/gtglrbsxxs.html

Go:   // 无解构
来源：http://hz.xinyue.icu/gtvnksvfgf.html

Ruby: a, b = pair
来源：http://hz.52xcode.cn/gtadwjsgzv.html

C#:   var (a, b) = pair;
来源：http://hz.birdmap.top/gteynzaiqz.html

[C16] 函数 / 方法重载
来源：http://hz.zhixingplan.top/gtriziaucp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nwbrower.top/gtgcdyvgrq.html

PHP:  // 无重载
来源：http://hz.hysaishi.cn/gtcowpedzj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhixingplan.top/gtvfxbgtle.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gaohongyu789.top/gtrcjvjira.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.svipenyu.cn/gtiwpwircp.html

Go:   // 无重载：用不同函数名
来源：http://hz.snrcjt.cn/gtlgijknir.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yueranfly.top/gtyujgmffy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yj20258.top/gthqthqcpr.html

================================================================================
来源：http://hz.daxiang520.top/gtajzjpnbw.html

D. 数组 / 列表 / 集合
来源：http://hz.zhongyouzk.top/gtvkglocym.html

================================================================================
来源：http://hz.sufxvd.cn/gtbaungqme.html

[D01] 创建数组 / 列表
来源：http://hz.ydjk.org.cn/gtxopcdrba.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.birdmap.top/gtbyhfwbnt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ywan-chungtsiang.top/gtpmdzucpg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yj20258888.top/gtkcorgbop.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xinyue.icu/gtenuyeoyz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.chenzaomai.com/gtucottgpm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hfpthk.cn/gtvgfydvuu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.fzhhl.top/gtdstlgoqm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.meibo888.top/gtjyltsiyu.html

[D02] 追加元素到末尾
来源：http://hz.c1oappe.top/gtksjkxxic.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yuanzhike.top/gtszznukfu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jqgfzy.top/gtgeswuvns.html

JS:   arr.push(4);
来源：http://hz.0kj1m.cn/gtqihtnvwq.html

TS:   arr.push(4);
来源：http://hz.hysaishi.cn/gtsquoluad.html

Java: list.add(4);
来源：http://hz.cqqwz.cn/gtaictmxrj.html

Go:   arr = append(arr, 4)
来源：http://hz.aibaodan.cn/gtivalmqzp.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.smart0.xyz/gtbgfjluns.html

C#:   list.Add(4);
来源：http://hz.316326.xyz/gtnjfucztj.html

[D03] 在指定位置插入元素
来源：http://hz.jyoumei.cn/gtotysjbds.html

Py:   arr.insert(0, 0)
来源：http://hz.dianchejie.cn/gtqetnpjxi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.daxiang520.top/gtgfuchyxd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.mhx1999.top/gtabnvuyod.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhaomingkeji.xyz/gtmbnyhhlz.html

Java: list.add(0, 0);
来源：http://hz.pengpengdd.cyou/gtunszvnxi.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jqgfzy.top/gtukhcerbi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jianghu66.top/gtfjhmtuzl.html

C#:   list.Insert(0, 0);
来源：http://hz.chenlongwang.top/gtyvjzwnqk.html

[D04] 删除元素
来源：http://hz.aibaodan.cn/gtbaesgpnk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yuxming.cn/gtvgsswkms.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yj20258.top/gtcvoniphz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jianghu66.top/gtkvxiwzkh.html

TS:   arr.splice(0, 1);
来源：http://hz.pycfn.com/gtxbqyxfyf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinqigfzy.top/gtgyjoyxtk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.pengpengdd.cyou/gtdzwxacjs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinyuanbaomall.cn/gtfavjhirp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.guannengcc.top/gtlozpgjjo.html

[D05] 访问与修改元素
来源：http://hz.andypj.xyz/gtgdbsllzz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jqgfzy.top/gtwnaibmmp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtosrqhckb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.quarkkingdee.top/gtitlhyimn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yanxiufei.cn/gtgpfwdipz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.haohaochexian.top/gtkobdbnkz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.smart0.xyz/gtkaxgoybd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fzhhl.top/gtorjwgmcs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.vqdsnc.cn/gtelfsdapj.html

[D06] 数组长度
来源：http://hz.wangdashe.top/gtnkfggzrk.html

Py:   len(arr)
来源：http://hz.yvedp.cn/gtabtwfprn.html

PHP:  count($arr);
来源：http://hz.chenlongwang.top/gtujhpiips.html

JS:   arr.length
来源：http://hz.xuanzx.com/gtibzduhea.html

TS:   arr.length
来源：http://hz.yuanzhike.top/gtjszlydtc.html

Java: list.size();
来源：http://hz.yj20258888.top/gtidelfmri.html

Go:   len(arr)
来源：http://hz.gogol.net.cn/gtuqhxeyhm.html

Ruby: arr.length; arr.size
来源：http://hz.snrcjt.cn/gtzswoiqec.html

C#:   list.Count;
来源：http://hz.yuanzhike.top/gtxjmxbwjr.html

[D07] 切片 / 取子数组
来源：http://hz.xuanzx.com/gtpgwsohvq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yvedp.cn/gtzvbvpfpm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jinghuilouyu.cn/gtttphgmbg.html

JS:   arr.slice(1, 4);
来源：http://hz.dashuyun.cn/gttxpewfvs.html

TS:   arr.slice(1, 4);
来源：http://hz.gaohongyu789.top/gtxsyijqhk.html

Java: list.subList(1, 4);
来源：http://hz.daxiang520.top/gtkuqmsodw.html

Go:   arr[1:4]
来源：http://hz.chenlongwang.top/gtqizchjrn.html

Ruby: arr[1, 3]
来源：http://hz.yonumen.top/gtkrmyrjce.html

C#:   list.GetRange(1, 3);
来源：http://hz.sysykeji.top/gtphfhxtvr.html

[D08] 合并两个数组
来源：http://hz.zdqjudy.top/gtllmgxeed.html

Py:   a + b;  a.extend(b)
来源：http://hz.jqgfzy.top/gtgkqrhglh.html

PHP:  array_merge($a, $b);
来源：http://hz.fengsongda.top/gtcawgukzb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ehwqpu.com/gtxmeptmqh.html

TS:   [...a, ...b];
来源：http://hz.xuanzx.com/gtsotcckkf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenzaomai.com/gtznyucfdf.html

Go:   append(a, b...)
来源：http://hz.chenjidiqi.icu/gtmrhtijmg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.meibo888.top/gtktzyeema.html

C#:   a.Concat(b).ToList()
来源：http://hz.cheryme.top/gtyzuxjwjm.html

[D09] 排序（升序）
来源：http://hz.jinghuilouyu.cn/gtpokiqsel.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtpjvydzhc.html

PHP:  sort($arr);
来源：http://hz.cqqwz.cn/gtxmfupbyf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.pengpengdd.cyou/gtcisexbzm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cheryme.top/gtxkbpgwpl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xylfe.cn/gtwjwxuwcu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj20258.top/gtahfbboqs.html

Ruby: arr.sort
来源：http://hz.ivvv.top/gtzqzbajxu.html

C#:   list.Sort();
来源：http://hz.shanyushiyangkeji.top/gtrskjnfcf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.vqdsnc.cn/gtmjrlmswe.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jyoumei.cn/gtxszrgfmd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.mhx1999.top/gtmwwyvgbu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuanzhike.top/gttoeipbge.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ivvv.top/gtdrewkubk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zycfv.cn/gtyznwgnke.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gogol.net.cn/gtmkzjycjm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hammf.cn/gtqwfelkso.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yanxiufei.cn/gtrhoasvwn.html

[D11] 反转数组
来源：http://hz.xuanzx.com/gtczanzbks.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cdnleiting.top/gtfkhrtakp.html

PHP:  array_reverse($arr);
来源：http://hz.jqgfzy.top/gteiozgtfq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhaomingkeji.xyz/gtvluzgmdw.html

TS:   [...arr].reverse();
来源：http://hz.hnxiangtu.top/gtgwjnigtf.html

Java: Collections.reverse(list);
来源：http://hz.svipenyu.cn/gtolhtasdk.html

Go:   slices.Reverse(arr)
来源：http://hz.jinghuilouyu.cn/gtmbdomdac.html

Ruby: arr.reverse
来源：http://hz.ydzc1.top/gtoifvhxah.html

C#:   list.Reverse();
来源：http://hz.yanxiufei.cn/gtjesoousx.html

[D12] 查找元素下标
来源：http://hz.haohaochexian.top/gtzawdffkg.html

Py:   arr.index(x);  x in arr
来源：http://hz.cdnleiting.top/gtnmfgsjvl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cashguo.top/gtjkxccryo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guannengcc.top/gthqvyumep.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenzaomai.com/gtfdcvncvu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinqigufen.top/gtvuctvwpd.html

Go:   slices.Index(arr, x)
来源：http://hz.hnqzz.top/gtzcpfsejy.html

Ruby: arr.index(x)
来源：http://hz.sweek.top/gtjhrqsvty.html

C#:   list.IndexOf(x);
来源：http://hz.jqgfzy.top/gtvdiindfm.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sysykeji.top/gtopkhdzra.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenjidiqi.icu/gtrezkaddr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cdnleiting.top/gtdukctkfq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xylfe.cn/gtqrpfefbg.html

TS:   arr.filter(x => x > 3)
来源：http://hz.quarkkingdee.top/gtewtodnbp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gotoacloud.top/gtooguousz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jlsjyb.cn/gtklwmtmnv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ivvv.top/gtuofrvrlg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.daria6918.cn/gtckyfgiow.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nanxuanxn.top/gthlyopwsv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ppjwa.cn/gtdxszutku.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.dashuyun.cn/gtmeghhjqy.html

JS:   arr.map(x => x * 2)
来源：http://hz.cucudq.cn/gtemgijclw.html

TS:   arr.map(x => x * 2)
来源：http://hz.nwbrower.top/gtzbxhsrre.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.sxryk.cn/gtqzhwweiq.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gtwdtmcbqj.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ppjwa.cn/gtmgqmbxbs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.nwbrower.top/gtaigvxjdl.html

[D15] 去重
来源：http://hz.yj202588.top/gtyctzhgdd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.guowangkeji.top/gtbznhbilk.html

PHP:  array_unique($arr);
来源：http://hz.aizwys.cn/gtthvvuqbk.html

JS:   [...new Set(arr)]
来源：http://hz.yj202588.top/gtbskhhsvi.html

TS:   [...new Set(arr)]
来源：http://hz.yonumen.top/gtqebptlex.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.smart0.xyz/gtgyljwxyg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shuidangran.top/gtsbpqvjbu.html

Ruby: arr.uniq
来源：http://hz.gogol.net.cn/gttwlrpyes.html

C#:   list.Distinct().ToList()
来源：http://hz.zdqjudy.top/gtdhxnmrjg.html

[D16] 求和与平均值
来源：http://hz.pycfn.com/gtyhelkhak.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.snrcjt.cn/gtyrgjzyql.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shanyushiyangkeji.top/gtlvisypqi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gaohongyu789.top/gtjhbvffdw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtbkmntsnc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xuanzx.com/gtfxlyxuew.html

Go:   // 手写循环累加
来源：http://hz.yj20258.top/gtpozhueyk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sysykeji.top/gtayzgbmry.html

C#:   list.Sum();  list.Average()
来源：http://hz.yanxiufei.cn/gtzdeifvni.html

[D17] 最大值与最小值
来源：http://hz.sufxvd.cn/gtllqqxqhu.html

Py:   max(arr);  min(arr)
来源：http://hz.yangfankeji.com/gtcocwteyy.html

PHP:  max($arr);  min($arr);
来源：http://hz.smart0.xyz/gtqvkskajv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dianchejie.cn/gtqwiarxop.html

TS:   Math.max(...arr);
来源：http://hz.52xcode.cn/gtcsbvrmbm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigufen.top/gtgugjldvl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangdashe.top/gtjmviwzwd.html

Ruby: arr.max;  arr.min
来源：http://hz.hywenlv.cn/gtutdvplut.html

C#:   list.Max();  list.Min()
来源：http://hz.hywenlv.cn/gtrvkfjrgh.html

[D18] 扁平化嵌套数组
来源：http://hz.xziqi.cn/gtskwvzpnh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenjidiqi.icu/gthqcepjru.html

PHP:  array_merge(...$nested);
来源：http://hz.zhaomingkeji.xyz/gtcxjjzwiz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinghuilouyu.cn/gtdinlomnw.html

TS:   nested.flat();
来源：http://hz.nwbrower.top/gtsqprmjru.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ivvv.top/gtmtdkzlxh.html

Go:   // 手写双层循环
来源：http://hz.jqgufenzy.top/gtdixmrnpc.html

Ruby: nested.flatten
来源：http://hz.hfpthk.cn/gtaoxcvxlc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yonumen.top/gtokllvstc.html

[D19] 按字段分组
来源：http://hz.tanke756.top/gtzevecsma.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.birdmap.top/gtzsdbhsbg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dashuyun.cn/gtmvslezni.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenzaomai.com/gtrnvqayor.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sweek.top/gtkrjaozua.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.tianlin.xyz/gtufontyxw.html

Go:   // 手写 map[string][]T
来源：http://hz.yongpay.top/gtygwphmzj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.pengpengdd.cyou/gtxkbhbbeu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hnqzz.top/gtddvztwee.html

[D20] 统计每个元素出现次数
来源：http://hz.guowangkeji.top/gtrknoqxjd.html

Py:   Counter(arr)
来源：http://hz.shuidangran.top/gtxdffjxmp.html

PHP:  array_count_values($arr);
来源：http://hz.wangshuangyany.cn/gtspdhgqlo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigufen.top/gtljxcazxn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuetiantiany.cn/gteufmxdry.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shzxlz.cn/gtkztqlsfq.html

Go:   // 手写 map[T]int
来源：http://hz.cdnleiting.top/gthrygcqsc.html

Ruby: arr.tally
来源：http://hz.xuanzx.com/gtrymxmhzv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.aizwys.cn/gtohhniolv.html

[D21] 判断是否包含某元素
来源：http://hz.316326.xyz/gtdtwgzukm.html

Py:   x in arr
来源：http://hz.jinghuilouyu.cn/gtzkaxzsva.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tianlin.xyz/gtoacoagmc.html

JS:   arr.includes(x)
来源：http://hz.jinyuanbaomall.cn/gtzlwsbyti.html

TS:   arr.includes(x)
来源：http://hz.jinqigfzy.top/gtqjmiprnw.html

Java: list.contains(x)
来源：http://hz.sweek.top/gtyaazptuj.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtuqnzcmdi.html

Ruby: arr.include?(x)
来源：http://hz.yonumen.top/gtvypxkgwz.html

C#:   list.Contains(x)
来源：http://hz.zhixingplan.top/gtjgpauscc.html

[D22] 复制数组（避免共享引用）
来源：http://hz.guannengcc.top/gtdwohfoom.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yuxming.cn/gtapdngzxz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.fengsongda.top/gtjbohclgh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.kuanghao11.cn/gthqgjmhcc.html

TS:   [...arr];
来源：http://hz.jinyuanbaomall.cn/gtduhjvacr.html

Java: new ArrayList<>(list);
来源：http://hz.yj202588.top/gtetbyslqv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.fzhhl.top/gtcxaxmfmz.html

Ruby: arr.dup;  arr.clone
来源：http://hz.pycfn.com/gtrgsecmsd.html

C#:   new List<int>(list);
来源：http://hz.jinqigufen.top/gtkwqhnpil.html

[D23] reduce 累积计算
来源：http://hz.yueranfly.top/gtnyedzark.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yuanzhike.top/gtksuosgcq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.dianchejie.cn/gtudanwmcm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hywenlv.cn/gtdkqdtamy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenlongwang.top/gtbbhvdmst.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xuetiantiany.cn/gtoritvjfu.html

Go:   // 手写循环
来源：http://hz.xingfuxueyuan.xyz/gtjsvogzha.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.mhx1999.top/gthquwikha.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhixingplan.top/gteccxxlel.html

[D24] 字典 / Map 基本操作
来源：http://hz.kuanghao11.cn/gtkufoudgb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.chenzaomai.com/gtuxsfxqxy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.316326.xyz/gtewewktqr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ybcxt.top/gtzbtpumco.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.daxiang520.top/gtqrxctyyg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shanyushiyangkeji.top/gtielmdxwi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jiagoushi.top/gtmlnmhxdy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sufxvd.cn/gtknukpiem.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.fzhhl.top/gtlfnuyqor.html

[D25] Set 集合去重与交并差
来源：http://hz.ybcxt.top/gtlpxajbcp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hammf.cn/gthoouudme.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xylfe.cn/gtjfkwdrvl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.bjfxy.top/gtiapbwtst.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yangfankeji.com/gtdxositsx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gzhubu.top/gtfagmgsgc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hysaishi.cn/gtjefixfni.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zdqjudy.top/gtczsbyfzi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.fengsongda.top/gtaywvkxgc.html

[D26] 数组转字符串
来源：http://hz.jinqigufen.top/gtanszrsfn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinqigfzy.top/gtjjxpwwgp.html

PHP:  implode(", ", $arr);
来源：http://hz.cdnleiting.top/gtcjilaosr.html

JS:   arr.join(", ")
来源：http://hz.gogol.net.cn/gtxgpvielq.html

TS:   arr.join(", ")
来源：http://hz.iojbl.cn/gtottunmcw.html

Java: String.join(", ", list)
来源：http://hz.chenjidiqi.icu/gttctggwnb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ydzc1.top/gtldlwuqgy.html

Ruby: arr.join(", ")
来源：http://hz.chenjidiqi.icu/gtylpwidkx.html

C#:   string.Join(", ", list)
来源：http://hz.shuidangran.top/gtqyjtndcz.html

================================================================================
来源：http://hz.sweek.top/gtpznvpsbk.html

E. 字符串处理
来源：http://hz.bjfxy.top/gttjtcxiup.html

================================================================================
来源：http://hz.hywenlv.cn/gtfzsgtasq.html

[E01] 拼接字符串
来源：http://hz.yj20258.top/gtmidobofc.html


<!-- 参考信息 -->