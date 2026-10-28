代发 wailian999

[C10] 变量作用域
来源：http://hz.sxryk.cn/gttebujzuh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.vqdsnc.cn/gtpicrqsyl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ydzc1.top/gtqhjyjryw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.snrcjt.cn/gtlmcxqbcd.html

TS:   同 JS
来源：http://hz.nanxuanxn.top/gtlqxshkjo.html

Java: 方法内为块级作用域
来源：http://hz.yj20258.top/gtowrngsul.html

Go:   花括号块级作用域
来源：http://hz.pycfn.com/gtpptylmzi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinqigfzy.top/gtuynciarc.html

C#:   块级作用域
来源：http://hz.zycfv.cn/gtgaivrlse.html

[C11] 模块导入与导出
来源：http://hz.chenjidiqi.icu/gtuyypcrfa.html

Py:   from module import func
来源：http://hz.316326.xyz/gtdsyiglcg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhijiandao.cn/gtdxjiagve.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.fengsongda.top/gtatuuxbwe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ybcxt.top/gttymopgiy.html

Java: import java.util.List;
来源：http://hz.zhaomingkeji.xyz/gtzhzmwahz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ppjwa.cn/gtbjnlcnwy.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.andypj.xyz/gtlefbaexk.html

C#:   using System.Text;
来源：http://hz.yueranfly.top/gttybkxaug.html

[C12] 立即执行函数 IIFE
来源：http://hz.guowangkeji.top/gtiknomjdz.html

Py:   (lambda: print("run"))()
来源：http://hz.aizwys.cn/gtazqsucvt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zycfv.cn/gtdfpszpgx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.gotoacloud.top/gtvwthrzdt.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhaomingkeji.xyz/gtaujzmfrm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sxryk.cn/gtvzvdhapy.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhixingplan.top/gtdhtarznv.html

Ruby: -> { puts "run" }.call
来源：http://hz.smart0.xyz/gtxaitgsgo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.haohaochexian.top/gtobrdccpo.html

[C13] 类型声明 / 类型注解
来源：http://hz.yangfankeji.com/gtixdlzhtk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shzxlz.cn/gtzshtalpg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtrzykjkuy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yueranfly.top/gtfpdfjisz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnxiangtu.top/gtfjwresev.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hnqzz.top/gttnnvnagl.html

Go:   func add(a, b int) int
来源：http://hz.gotoacloud.top/gtxmhoapry.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hongshengwenyu.top/gtebzaovqc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.quarkkingdee.top/gtzuiktjnm.html

[C14] 泛型函数
来源：http://hz.sweek.top/gtgdkvjivw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.nanxinkj.top/gtagtfbpgo.html

PHP:  // 无泛型
来源：http://hz.yuxming.cn/gtynqqqjhb.html

JS:   // 无泛型
来源：http://hz.jiagoushi.top/gttrkhjsrr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.9152youxi.cn/gtkfnfssuh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yonumen.top/gtsisrcpkc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ppjwa.cn/gtmmbcwnzi.html

Ruby: # 无泛型
来源：http://hz.zhoulong.xyz/gtmlxypfiv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pengpengdd.cyou/gtsuvrgmig.html

[C15] 解构 / 展开参数
来源：http://hz.zhaomingkeji.xyz/gtnllbtojm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhixingplan.top/gtqaynpsum.html

PHP:  [$a, $b] = $pair;
来源：http://hz.aizwys.cn/gtboixgadz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.redwolf501.top/gtixnemynz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.vqdsnc.cn/gtzubrnwjy.html

Java: // 无解构
来源：http://hz.jinyuanbaomall.cn/gtkbaqywhz.html

Go:   // 无解构
来源：http://hz.nanxuanxn.top/gtenahoxqr.html

Ruby: a, b = pair
来源：http://hz.jinghuilouyu.cn/gtmwelwwjt.html

C#:   var (a, b) = pair;
来源：http://hz.zhongyouzk.top/gtpctzpvol.html

[C16] 函数 / 方法重载
来源：http://hz.zhixingplan.top/gtlhlwzzgo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.aizwys.cn/gthwpisedq.html

PHP:  // 无重载
来源：http://hz.daria6918.cn/gtmknmoesa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jqgfzy.top/gtscrflqqd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.haohaochexian.top/gtbcaaumvd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ehwqpu.com/gtsiibgkqg.html

Go:   // 无重载：用不同函数名
来源：http://hz.xuetiantiany.cn/gtiydxyxgi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hnqzz.top/gthuvcbmkv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.dianchejie.cn/gtvknkzwca.html

================================================================================
来源：http://hz.vqdsnc.cn/gtxnzyyguq.html

D. 数组 / 列表 / 集合
来源：http://hz.meibo888.top/gtystjtjya.html

================================================================================
来源：http://hz.birdmap.top/gtksnmeazd.html

[D01] 创建数组 / 列表
来源：http://hz.guowangkeji.top/gtixdntxeb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhengqikj.top/gtuhyojbss.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guowangkeji.top/gttbwfslwy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jlsjyb.cn/gtmppgmrcb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.feifeiyinyue.top/gtmomrepky.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.fzhhl.top/gtxcghqsmh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sufxvd.cn/gtsqqvzwvt.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhengqikj.top/gtzmgguxbu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gogol.net.cn/gtdluptrkm.html

[D02] 追加元素到末尾
来源：http://hz.ywan-chungtsiang.top/gtxhzikjdp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.feifeiyinyue.top/gthkruvmkc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.birdmap.top/gtvnjthste.html

JS:   arr.push(4);
来源：http://hz.hywenlv.cn/gtmjmdvrmh.html

TS:   arr.push(4);
来源：http://hz.kuanghao11.cn/gtwbjmnonj.html

Java: list.add(4);
来源：http://hz.yuanzhike.top/gtdpntterr.html

Go:   arr = append(arr, 4)
来源：http://hz.zhoulong.xyz/gtnbpmowle.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.andypj.xyz/gtdyomimcb.html

C#:   list.Add(4);
来源：http://hz.zhijiandao.cn/gtzytcydlk.html

[D03] 在指定位置插入元素
来源：http://hz.sxryk.cn/gtqhfcunhz.html

Py:   arr.insert(0, 0)
来源：http://hz.gaohongyu789.top/gtpvbpmruo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhijiandao.cn/gtgtzwxhzi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.meibo888.top/gtizvvmynh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.birdmap.top/gtzumfatjs.html

Java: list.add(0, 0);
来源：http://hz.316326.xyz/gtvvmkomrl.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yanxiufei.cn/gtvkqbrhhq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sysykeji.top/gtgvstqcjp.html

C#:   list.Insert(0, 0);
来源：http://hz.chenzaomai.com/gthjfgfcvt.html

[D04] 删除元素
来源：http://hz.yj202588.top/gtybtunsjv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sysykeji.top/gtwjtqcigr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.tianlin.xyz/gteyqslklb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shanyushiyangkeji.top/gtgqhchbde.html

TS:   arr.splice(0, 1);
来源：http://hz.jinyuanbaomall.cn/gtcpmlvfeg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.chenjidiqi.icu/gtpvquptuf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.smart0.xyz/gtywgbgmne.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinqigfzy.top/gtndyxwmcc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.nanxuanxn.top/gtxoxbvpcr.html

[D05] 访问与修改元素
来源：http://hz.hnxiangtu.top/gthezuxrns.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hammf.cn/gtfweolfop.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.tianlin.xyz/gtholenezo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.chenzaomai.com/gtnojpprqh.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cashguo.top/gtfdklulel.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.wangshuangyany.cn/gtrudnvnid.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.smart0.xyz/gtwxccrwnn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.snrcjt.cn/gtgzrfotud.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.kuanghao11.cn/gtowggiuyy.html

[D06] 数组长度
来源：http://hz.52xcode.cn/gtkurrcuqv.html

Py:   len(arr)
来源：http://hz.vqdsnc.cn/gtcpbrgbgv.html

PHP:  count($arr);
来源：http://hz.xuetiantiany.cn/gtkqnfvaxk.html

JS:   arr.length
来源：http://hz.meibo888.top/gtoaufqhfj.html

TS:   arr.length
来源：http://hz.hysaishi.cn/gtblziozbo.html

Java: list.size();
来源：http://hz.c1oappe.top/gtfcthhukm.html

Go:   len(arr)
来源：http://hz.yuanzhike.top/gtvwxrlwif.html

Ruby: arr.length; arr.size
来源：http://hz.daria6918.cn/gtqyekdbsp.html

C#:   list.Count;
来源：http://hz.shanyushiyangkeji.top/gtolixykus.html

[D07] 切片 / 取子数组
来源：http://hz.jiagoushi.top/gthczrvszr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.gaohongyu789.top/gtiwxewrcx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jinghuilouyu.cn/gtulevnuyy.html

JS:   arr.slice(1, 4);
来源：http://hz.vqdsnc.cn/gttajzofzv.html

TS:   arr.slice(1, 4);
来源：http://hz.chenlongwang.top/gtnnaqvigh.html

Java: list.subList(1, 4);
来源：http://hz.feifeiyinyue.top/gteuudmmzz.html

Go:   arr[1:4]
来源：http://hz.xylfe.cn/gtadmeejmv.html

Ruby: arr[1, 3]
来源：http://hz.sysykeji.top/gtstnxcbbt.html

C#:   list.GetRange(1, 3);
来源：http://hz.cheryme.top/gtmncdcuxd.html

[D08] 合并两个数组
来源：http://hz.zhaomingkeji.xyz/gttcutwmwq.html

Py:   a + b;  a.extend(b)
来源：http://hz.shzxlz.cn/gtveoaofap.html

PHP:  array_merge($a, $b);
来源：http://hz.yuxming.cn/gtkvqbpjlq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.havefunace.top/gtezwcubiu.html

TS:   [...a, ...b];
来源：http://hz.yangfankeji.com/gtuferkajq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hysaishi.cn/gteldtdphp.html

Go:   append(a, b...)
来源：http://hz.yj202588.top/gteqaupsvh.html

Ruby: a + b;  a.concat(b)
来源：http://hz.gzhubu.top/gtewnzogvv.html

C#:   a.Concat(b).ToList()
来源：http://hz.cucudq.cn/gtgzloayev.html

[D09] 排序（升序）
来源：http://hz.birdmap.top/gtxbtbpycr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pycfn.com/gtzkvneyti.html

PHP:  sort($arr);
来源：http://hz.jinqigufen.top/gtojseeelb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yuanzhike.top/gtmobfavpo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shzxlz.cn/gtwgornhem.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.52xcode.cn/gtzanrezxd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.wangdashe.top/gtfcatupbe.html

Ruby: arr.sort
来源：http://hz.shanyushiyangkeji.top/gtbqaovdwy.html

C#:   list.Sort();
来源：http://hz.yanxiufei.cn/gtuatbygmw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.chenzaomai.com/gttviutwwe.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jqgufenzy.top/gtauibzqcs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigfzy.top/gtiehnakzu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cashguo.top/gtnseglvdc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hysaishi.cn/gtaqzdkmta.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgufenzy.top/gtkhrkiinp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhoulong.xyz/gtomlkcpdu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenjidiqi.icu/gtrsmtutnk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenzaomai.com/gtezveaiyz.html

[D11] 反转数组
来源：http://hz.havefunace.top/gtisbhicif.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gotoacloud.top/gtfzskvzlk.html

PHP:  array_reverse($arr);
来源：http://hz.nanxinkj.top/gthbenyhpm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhijiandao.cn/gtyidusmpc.html

TS:   [...arr].reverse();
来源：http://hz.jianghu66.top/gtlryvheve.html

Java: Collections.reverse(list);
来源：http://hz.yuxming.cn/gtqbhenbih.html

Go:   slices.Reverse(arr)
来源：http://hz.yj20258.top/gttbdbuomh.html

Ruby: arr.reverse
来源：http://hz.jinqigfzy.top/gtmnzsjmbe.html

C#:   list.Reverse();
来源：http://hz.nanxinkj.top/gtixyycfnb.html

[D12] 查找元素下标
来源：http://hz.daxiang520.top/gtwmounwqx.html

Py:   arr.index(x);  x in arr
来源：http://hz.tianlin.xyz/gtburoydoe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhijiandao.cn/gtrweqelvu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shzxlz.cn/gtyjmqxadd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tanke756.top/gtjoehqfft.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.bjfxy.top/gtacmzxqmv.html

Go:   slices.Index(arr, x)
来源：http://hz.jinqigfzy.top/gttcsfrjjt.html

Ruby: arr.index(x)
来源：http://hz.aibaodan.cn/gtiocstbit.html

C#:   list.IndexOf(x);
来源：http://hz.dianchejie.cn/gtparutkgd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yj20258888.top/gtssfjknkq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnxiangtu.top/gthtffdbsn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jianghu66.top/gtzhswyjwq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.chenlongwang.top/gtthfoutbn.html

TS:   arr.filter(x => x > 3)
来源：http://hz.kuanghao11.cn/gtakyopdqr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cdnleiting.top/gtkofbiuku.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jianghu66.top/gtzpdoxdww.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.daria6918.cn/gtllgbwqwk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sysykeji.top/gtkiemdefc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.aibaodan.cn/gtopbfdfjl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tanke756.top/gtdywyyspw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.andypj.xyz/gtjvdtlbea.html

JS:   arr.map(x => x * 2)
来源：http://hz.chenlongwang.top/gtmtoiivba.html

TS:   arr.map(x => x * 2)
来源：http://hz.fengsongda.top/gtqiuvfamr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.chenlongwang.top/gthpzeuxtk.html

Go:   // 手写循环
来源：http://hz.jinghuilouyu.cn/gtnhvnayap.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cheryme.top/gtueefclgm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinyuanbaomall.cn/gthjyhokmc.html

[D15] 去重
来源：http://hz.jinyuanbaomall.cn/gtnumdkgxu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.birdmap.top/gtupwkosyk.html

PHP:  array_unique($arr);
来源：http://hz.jqgfzy.top/gtypyyozuw.html

JS:   [...new Set(arr)]
来源：http://hz.yuanzhike.top/gtilylrabq.html

TS:   [...new Set(arr)]
来源：http://hz.zhaomingkeji.xyz/gtethjocue.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yongpay.top/gtcbnevinc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.aizwys.cn/gtrugroptw.html

Ruby: arr.uniq
来源：http://hz.jyoumei.cn/gtnrqxlelv.html

C#:   list.Distinct().ToList()
来源：http://hz.yanxiufei.cn/gtqylcgigm.html

[D16] 求和与平均值
来源：http://hz.gzhubu.top/gtarifjkay.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.guowangkeji.top/gtemmqunsy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yonumen.top/gtukwouwmi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hammf.cn/gtcfvxwuka.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhongyouzk.top/gttlksyksp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.birdmap.top/gtnsvjwxks.html

Go:   // 手写循环累加
来源：http://hz.hywenlv.cn/gtbtdstyrf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.9152youxi.cn/gtmjuntpke.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj20258888.top/gtdtmeqijv.html

[D17] 最大值与最小值
来源：http://hz.feifeiyinyue.top/gtukoherzc.html

Py:   max(arr);  min(arr)
来源：http://hz.pycfn.com/gtqsowbdms.html

PHP:  max($arr);  min($arr);
来源：http://hz.gzhubu.top/gtxanwdkjt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.guowangkeji.top/gtchdmnwca.html

TS:   Math.max(...arr);
来源：http://hz.zhengqikj.top/gtbblqocbd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tianlin.xyz/gtgidtmpim.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.aizwys.cn/gtrwcymidl.html

Ruby: arr.max;  arr.min
来源：http://hz.316326.xyz/gtybafbeca.html

C#:   list.Max();  list.Min()
来源：http://hz.haohaochexian.top/gtdrazrxsc.html

[D18] 扁平化嵌套数组
来源：http://hz.bjfxy.top/gtsffjhafg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sysykeji.top/gtxtojztub.html

PHP:  array_merge(...$nested);
来源：http://hz.gotoacloud.top/gtfwbbeqch.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yuanzhike.top/gtubxevukz.html

TS:   nested.flat();
来源：http://hz.shzxlz.cn/gtzlsvnyjy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.9152youxi.cn/gtdtgpcyfo.html

Go:   // 手写双层循环
来源：http://hz.hywenlv.cn/gtjzycitea.html

Ruby: nested.flatten
来源：http://hz.ivvv.top/gtdmpkdoir.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hywenlv.cn/gtwqjcoktl.html

[D19] 按字段分组
来源：http://hz.52xcode.cn/gtabysrcwc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ydzc1.top/gtdbotoplf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhongyouzk.top/gtxcntpqqt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cucudq.cn/gtwfnpzssf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sufxvd.cn/gtivvjzvql.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.guowangkeji.top/gttkuecryx.html

Go:   // 手写 map[string][]T
来源：http://hz.ybcxt.top/gtncfrhlvv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yongpay.top/gtrqxkbxtn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.daxiang520.top/gtosuravvi.html

[D20] 统计每个元素出现次数
来源：http://hz.aizwys.cn/gtuuicnids.html

Py:   Counter(arr)
来源：http://hz.haohaochexian.top/gtuegnnsha.html

PHP:  array_count_values($arr);
来源：http://hz.ivvv.top/gtxegmealb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhijiandao.cn/gtthrfqamu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.feifeiyinyue.top/gtioacgkio.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinqigufen.top/gtrhebepoz.html

Go:   // 手写 map[T]int
来源：http://hz.nanxinkj.top/gtsdxgifzi.html

Ruby: arr.tally
来源：http://hz.dashuyun.cn/gtcoytokfo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sysykeji.top/gtcmcoalmu.html

[D21] 判断是否包含某元素
来源：http://hz.zhoulong.xyz/gtheczqlps.html

Py:   x in arr
来源：http://hz.xinyue.icu/gtqzzrhhja.html

PHP:  in_array($x, $arr, true);
来源：http://hz.redwolf501.top/gtlnxpmnlp.html

JS:   arr.includes(x)
来源：http://hz.havefunace.top/gtojdbjbvh.html

TS:   arr.includes(x)
来源：http://hz.snrcjt.cn/gtgmazxtkq.html

Java: list.contains(x)
来源：http://hz.nanxinkj.top/gtvrqyoihj.html

Go:   slices.Contains(arr, x)
来源：http://hz.ehwqpu.com/gtmndfqeyd.html

Ruby: arr.include?(x)
来源：http://hz.gotoacloud.top/gtgrqrmdvu.html

C#:   list.Contains(x)
来源：http://hz.daxiang520.top/gtvpustcza.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tian-w.cn/gtwmgvoqol.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhaomingkeji.xyz/gtdlgpaeha.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.nwbrower.top/gtfedyakbc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yvedp.cn/gtrcgnfvzj.html

TS:   [...arr];
来源：http://hz.hfpthk.cn/gtnpiciqiz.html

Java: new ArrayList<>(list);
来源：http://hz.hnxiangtu.top/gtuxwkqouu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinghuilouyu.cn/gtydufutks.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nanxuanxn.top/gtoqpneawi.html

C#:   new List<int>(list);
来源：http://hz.havefunace.top/gthxcxkssx.html

[D23] reduce 累积计算
来源：http://hz.xuanzx.com/gtzklbfnpv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hammf.cn/gtjrzudyib.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yonumen.top/gtwssyytxr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ivvv.top/gtuasjyxvc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuxming.cn/gtwrazkosw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnqzz.top/gtdreffhwc.html

Go:   // 手写循环
来源：http://hz.andypj.xyz/gtlbtksruj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.guowangkeji.top/gtnmtrscqe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenjidiqi.icu/gtewhgvhym.html

[D24] 字典 / Map 基本操作
来源：http://hz.jyoumei.cn/gtszailbja.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ppjwa.cn/gtjmquyizy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xziqi.cn/gtcfxwaxlz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shanyushiyangkeji.top/gtmkvxphjd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.0kj1m.cn/gtmovqieii.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenlongwang.top/gtiocwwpeu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.wangdashe.top/gtbppyvxgv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yvedp.cn/gtdqnvfjqa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shuidangran.top/gtzccyzacl.html

[D25] Set 集合去重与交并差
来源：http://hz.hnxiangtu.top/gtgdcbucot.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.chenjidiqi.icu/gteoiuxnyr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.feifeiyinyue.top/gtpgvjvqgw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhixingplan.top/gtoqzppilz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hfpthk.cn/gtuptfauhu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.kuanghao11.cn/gtxnqbgkad.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jlsjyb.cn/gtfhfhbjho.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xinyue.icu/gtwmqdykhs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhijiandao.cn/gtgwufrjkh.html

[D26] 数组转字符串
来源：http://hz.sxryk.cn/gtoftqewwu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xinyue.icu/gthytthplr.html

PHP:  implode(", ", $arr);
来源：http://hz.snrcjt.cn/gtuegudscj.html

JS:   arr.join(", ")
来源：http://hz.sysykeji.top/gtkjzgaqmc.html

TS:   arr.join(", ")
来源：http://hz.yangfankeji.com/gtjgwtmwwd.html

Java: String.join(", ", list)
来源：http://hz.gaohongyu789.top/gtgvnkwevv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinghuilouyu.cn/gtrjcswkci.html

Ruby: arr.join(", ")
来源：http://hz.xinyue.icu/gtwiczqfuo.html

C#:   string.Join(", ", list)
来源：http://hz.dianchejie.cn/gtdoejxejd.html


<!-- 参考信息 -->