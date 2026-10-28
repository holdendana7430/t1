代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://hz.jinghuilouyu.cn/gtfncodhos.html

C#:   using System.Text;
来源：http://hz.fzhhl.top/gtqpevmmol.html

[C12] 立即执行函数 IIFE
来源：http://hz.pycfn.com/gtgrbfzowu.html

Py:   (lambda: print("run"))()
来源：http://hz.wangdashe.top/gtvbvpsvcr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sweek.top/gtpquwznit.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yvedp.cn/gtzzpvkemm.html

TS:   (() => { console.log("run"); })();
来源：http://hz.guowangkeji.top/gtrkyahtrt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hnxiangtu.top/gtumbdaxbn.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xuanzx.com/gtxtnvkugr.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhixingplan.top/gtgnocbocq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.pengpengdd.cyou/gtwdzokaef.html

[C13] 类型声明 / 类型注解
来源：http://hz.gotoacloud.top/gtefexgjpr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.meibo888.top/gtvjexbbgj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhoulong.xyz/gtccpqoadm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xylfe.cn/gtaenhofbl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtvpbrgbnl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.0kj1m.cn/gthnywzsfa.html

Go:   func add(a, b int) int
来源：http://hz.hongshengwenyu.top/gtoeihwufo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yj202588.top/gtjbucwtxs.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.iojbl.cn/gtinalabvq.html

[C14] 泛型函数
来源：http://hz.vqdsnc.cn/gtoqyrxerz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hfpthk.cn/gtwpakjsxb.html

PHP:  // 无泛型
来源：http://hz.sweek.top/gtnpwhbhjh.html

JS:   // 无泛型
来源：http://hz.zhoulong.xyz/gtoplhupwz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ywan-chungtsiang.top/gtvsjpdjqm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shangyingyoupin.top/gtlrglnaay.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yj202588.top/gtwvchnayn.html

Ruby: # 无泛型
来源：http://hz.yonumen.top/gtysxibxgu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.quarkkingdee.top/gtmqpebwfo.html

[C15] 解构 / 展开参数
来源：http://hz.yuxming.cn/gtcqejfexd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgfzy.top/gtvpdgiomz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.snrcjt.cn/gtktzzxawo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hfpthk.cn/gtpfesmype.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xingfuxueyuan.xyz/gtpjqvxktd.html

Java: // 无解构
来源：http://hz.sweek.top/gtjzrwvqmp.html

Go:   // 无解构
来源：http://hz.shangyingyoupin.top/gtnsqhgcjd.html

Ruby: a, b = pair
来源：http://hz.tianlin.xyz/gtawqtahxd.html

C#:   var (a, b) = pair;
来源：http://hz.hysaishi.cn/gtnzmxdguk.html

[C16] 函数 / 方法重载
来源：http://hz.gaohongyu789.top/gtqqotyiao.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hammf.cn/gtocdfufkf.html

PHP:  // 无重载
来源：http://hz.shangyingyoupin.top/gtktplczmw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.pengpengdd.cyou/gttoabfxbo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.bjfxy.top/gtctgrxhyu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.aizwys.cn/gtatklrcti.html

Go:   // 无重载：用不同函数名
来源：http://hz.cdnleiting.top/gtkajxwqih.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cheryme.top/gtfuntkfih.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.nwbrower.top/gtyflzfnrv.html

================================================================================
来源：http://hz.yvedp.cn/gtinplskwb.html

D. 数组 / 列表 / 集合
来源：http://hz.zdqjudy.top/gtpsxjsnly.html

================================================================================
来源：http://hz.dianchejie.cn/gtjfbgukqj.html

[D01] 创建数组 / 列表
来源：http://hz.zhaomingkeji.xyz/gtvvyetcqk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ivvv.top/gtukffrnoj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xylfe.cn/gtcoqnturo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhixingplan.top/gtqjjrmhtn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj20258.top/gtmvcugrng.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xylfe.cn/gtwvjyqsmz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hfpthk.cn/gtzsbycxno.html

Ruby: arr = [1, 2, 3]
来源：http://hz.aizwys.cn/gtxsbuvdnd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ydzc1.top/gtewrwxohu.html

[D02] 追加元素到末尾
来源：http://hz.dashuyun.cn/gtcibwwuqr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.dashuyun.cn/gtgzfxaptp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.bjfxy.top/gtrpvbaysb.html

JS:   arr.push(4);
来源：http://hz.ivvv.top/gtfvhcjhah.html

TS:   arr.push(4);
来源：http://hz.yueranfly.top/gtcmelmphf.html

Java: list.add(4);
来源：http://hz.kuanghao11.cn/gteikptqrf.html

Go:   arr = append(arr, 4)
来源：http://hz.shangyingyoupin.top/gtsfjmtdfn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yj20258888.top/gtrhrzjsrg.html

C#:   list.Add(4);
来源：http://hz.haohaochexian.top/gtsxqmsvnm.html

[D03] 在指定位置插入元素
来源：http://hz.shzxlz.cn/gtubsaduhw.html

Py:   arr.insert(0, 0)
来源：http://hz.sweek.top/gtyekgcerr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yonumen.top/gtleykasnl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhongyouzk.top/gtnutfuqhc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xuetiantiany.cn/gtaflxwnmr.html

Java: list.add(0, 0);
来源：http://hz.zhoulong.xyz/gtnqbpqfbl.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cdnleiting.top/gtcimtcitg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sufxvd.cn/gtjavsdyrj.html

C#:   list.Insert(0, 0);
来源：http://hz.xuanzx.com/gttidsbpsd.html

[D04] 删除元素
来源：http://hz.aizwys.cn/gtdujeuozr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenjidiqi.icu/gtqwplowwl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hywenlv.cn/gtcojhderm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hammf.cn/gtlprjhjse.html

TS:   arr.splice(0, 1);
来源：http://hz.jqgufenzy.top/gtxkzrxcdy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tian-w.cn/gtdnewhaad.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.wangshuangyany.cn/gtmlypigoe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.feifeiyinyue.top/gtumvwbmvh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shuidangran.top/gtoinnmjbz.html

[D05] 访问与修改元素
来源：http://hz.dianchejie.cn/gtqvisqcmh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydzc1.top/gtjhjaioba.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sweek.top/gtpicznrax.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinghuilouyu.cn/gtknizdhav.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinqigfzy.top/gtwprzpvls.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shzxlz.cn/gtijnoorhw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.chenjidiqi.icu/gtzqygpjte.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258888.top/gtcrjghcwc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yj20258888.top/gtklthmgve.html

[D06] 数组长度
来源：http://hz.sxryk.cn/gttsnwjcxh.html

Py:   len(arr)
来源：http://hz.dashuyun.cn/gtorqjhiuv.html

PHP:  count($arr);
来源：http://hz.nanxuanxn.top/gttuhkakeq.html

JS:   arr.length
来源：http://hz.dashuyun.cn/gtzexsvlkc.html

TS:   arr.length
来源：http://hz.gogol.net.cn/gtizjpgkwk.html

Java: list.size();
来源：http://hz.shuidangran.top/gtmddailbi.html

Go:   len(arr)
来源：http://hz.tianlin.xyz/gtaqnndnoh.html

Ruby: arr.length; arr.size
来源：http://hz.pycfn.com/gtskfgjbar.html

C#:   list.Count;
来源：http://hz.guowangkeji.top/gtgceeslcn.html

[D07] 切片 / 取子数组
来源：http://hz.shuidangran.top/gtbfxxrbom.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhongyouzk.top/gttsurwtlb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.aizwys.cn/gtgvyemhth.html

JS:   arr.slice(1, 4);
来源：http://hz.yanxiufei.cn/gtqptchtad.html

TS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangtech.top/gtgjnnxwmr.html

Java: list.subList(1, 4);
来源：http://hz.xylfe.cn/gttwgzlfiw.html

Go:   arr[1:4]
来源：http://hz.yuxming.cn/gtgyatveov.html

Ruby: arr[1, 3]
来源：http://hz.zhiwuduotai.top/gtqiefqypg.html

C#:   list.GetRange(1, 3);
来源：http://hz.tian-w.cn/gtnglchtog.html

[D08] 合并两个数组
来源：http://hz.jinqigufen.top/gthrpkwudf.html

Py:   a + b;  a.extend(b)
来源：http://hz.guannengcc.top/gtapnqvcms.html

PHP:  array_merge($a, $b);
来源：http://hz.ivvv.top/gtgwbqquua.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cashguo.top/gtasttupkr.html

TS:   [...a, ...b];
来源：http://hz.9152youxi.cn/gtdvsqtmqc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenlongwang.top/gtzxugaefl.html

Go:   append(a, b...)
来源：http://hz.ppjwa.cn/gtcpwfjtzd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jqgufenzy.top/gtucwoszpl.html

C#:   a.Concat(b).ToList()
来源：http://hz.xylfe.cn/gtptsrdhnx.html

[D09] 排序（升序）
来源：http://hz.daria6918.cn/gtjaatysho.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tanke756.top/gtymawtbef.html

PHP:  sort($arr);
来源：http://hz.zhijiandao.cn/gtsakmhayr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj20258.top/gtdgqjlonq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.feifeiyinyue.top/gtorynisuq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ydjk.org.cn/gtcohqnpuc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhengqikj.top/gtspvvomcq.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtladyobrj.html

C#:   list.Sort();
来源：http://hz.gzhubu.top/gtmcgirqty.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ivvv.top/gtnaocrbyq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.svipenyu.cn/gtiwtbmxcu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.pycfn.com/gtdmdgxmna.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jlsjyb.cn/gtpbbwpldq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinghuilouyu.cn/gtowkfagpj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xingfuxueyuan.xyz/gtcmpiwwht.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cdnleiting.top/gtbdssbdgz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.9152youxi.cn/gtcwuhooek.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xuanzx.com/gteimkvtsi.html

[D11] 反转数组
来源：http://hz.ybcxt.top/gtlyshzrmy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shzxlz.cn/gtnwpfatwe.html

PHP:  array_reverse($arr);
来源：http://hz.bjfxy.top/gtkyaijtff.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dashuyun.cn/gthcrukfpv.html

TS:   [...arr].reverse();
来源：http://hz.jinghuilouyu.cn/gtarizmqif.html

Java: Collections.reverse(list);
来源：http://hz.hnxiangtu.top/gtkmtyngej.html

Go:   slices.Reverse(arr)
来源：http://hz.xuetiantiany.cn/gtrvmesqqf.html

Ruby: arr.reverse
来源：http://hz.zhaomingkeji.xyz/gtfsetymas.html

C#:   list.Reverse();
来源：http://hz.tanke756.top/gtvutvzpov.html

[D12] 查找元素下标
来源：http://hz.xuanzx.com/gtxwecmhob.html

Py:   arr.index(x);  x in arr
来源：http://hz.shzxlz.cn/gtkxsoxxzx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nanxuanxn.top/gtdoksdcus.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pycfn.com/gtlkdgrxoe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtgemukhbt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nanxinkj.top/gtosnrlkkc.html

Go:   slices.Index(arr, x)
来源：http://hz.haohaochexian.top/gtjikjkcxm.html

Ruby: arr.index(x)
来源：http://hz.vqdsnc.cn/gtemipqyny.html

C#:   list.IndexOf(x);
来源：http://hz.vqdsnc.cn/gtfwncbkje.html

[D13] 过滤（保留满足条件的）
来源：http://hz.redwolf501.top/gtreodtdyh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gogol.net.cn/gtnqcmfnsg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yuxming.cn/gtzccdxrgc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yuanzhike.top/gtchmxrqbj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtuwjjhxxp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zycfv.cn/gtsvoriyws.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hongshengwenyu.top/gtfavddzpi.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.guowangkeji.top/gtaimbwlsv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jlsjyb.cn/gtiwxpfout.html

[D14] 映射转换（每个元素变形）
来源：http://hz.fengsongda.top/gtpcevitmw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.daria6918.cn/gtgnrefinw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jlsjyb.cn/gtdlyxztsg.html

JS:   arr.map(x => x * 2)
来源：http://hz.ywan-chungtsiang.top/gtjkbrvavv.html

TS:   arr.map(x => x * 2)
来源：http://hz.cashguo.top/gtwacabdpk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.nanxinkj.top/gtyhklchce.html

Go:   // 手写循环
来源：http://hz.hfpthk.cn/gtgchaurtl.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sysykeji.top/gtqetbbucy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shangyingyoupin.top/gttcyqzjbf.html

[D15] 去重
来源：http://hz.xuanzx.com/gtioonmeas.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hnqzz.top/gtdhmflbkg.html

PHP:  array_unique($arr);
来源：http://hz.xziqi.cn/gtpqmnajit.html

JS:   [...new Set(arr)]
来源：http://hz.zhaomingkeji.xyz/gtjretnoaq.html

TS:   [...new Set(arr)]
来源：http://hz.fengsongda.top/gtbjmftapr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.9152youxi.cn/gtmpruntnk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shanyushiyangtech.top/gtitctrtbl.html

Ruby: arr.uniq
来源：http://hz.dianchejie.cn/gtyxwnbpal.html

C#:   list.Distinct().ToList()
来源：http://hz.ehwqpu.com/gtvzmmkkpt.html

[D16] 求和与平均值
来源：http://hz.daxiang520.top/gtbsrsmlif.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.haohaochexian.top/gtqxkyfnjm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.tanke756.top/gtyajxwzpj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.havefunace.top/gtdjeuvjnv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xylfe.cn/gtxbnexyuo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hywenlv.cn/gtfrlyhypd.html

Go:   // 手写循环累加
来源：http://hz.0kj1m.cn/gtgsyyuruu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.daxiang520.top/gtfujtczwm.html

C#:   list.Sum();  list.Average()
来源：http://hz.tanke756.top/gtzzjqdmdy.html

[D17] 最大值与最小值
来源：http://hz.316326.xyz/gtwjjaoeet.html

Py:   max(arr);  min(arr)
来源：http://hz.sufxvd.cn/gtjzajmncp.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinyuanbaomall.cn/gtvgisurvj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yj20258888.top/gtgrkqwmjt.html

TS:   Math.max(...arr);
来源：http://hz.iojbl.cn/gtughoauqq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.kuanghao11.cn/gtosgrnamr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hywenlv.cn/gthrvcdnot.html

Ruby: arr.max;  arr.min
来源：http://hz.c1oappe.top/gtvzaicvop.html

C#:   list.Max();  list.Min()
来源：http://hz.yuanzhike.top/gttfyusbqj.html

[D18] 扁平化嵌套数组
来源：http://hz.havefunace.top/gtcdjhqssa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sweek.top/gtynudhrch.html

PHP:  array_merge(...$nested);
来源：http://hz.yongpay.top/gtljasisvi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.pycfn.com/gtnlzhmtdk.html

TS:   nested.flat();
来源：http://hz.52xcode.cn/gtpsrajwmm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenlongwang.top/gtkksngvsy.html

Go:   // 手写双层循环
来源：http://hz.yuanzhike.top/gtiqsapebv.html

Ruby: nested.flatten
来源：http://hz.feifeiyinyue.top/gtsrnqokrs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jiagoushi.top/gtccorbejy.html

[D19] 按字段分组
来源：http://hz.dianchejie.cn/gtgidvwscl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.fengsongda.top/gtvgzumakk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nanxinkj.top/gtbpwreoyl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.sweek.top/gtljumpyxn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jiagoushi.top/gttpyeumej.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yuxming.cn/gtqrubxnje.html

Go:   // 手写 map[string][]T
来源：http://hz.hnqzz.top/gtlekzbodv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yongpay.top/gtqncahgab.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj202588.top/gtouayjfwf.html

[D20] 统计每个元素出现次数
来源：http://hz.ivvv.top/gtjwlaihgf.html

Py:   Counter(arr)
来源：http://hz.jinghuilouyu.cn/gtyyrblzfj.html

PHP:  array_count_values($arr);
来源：http://hz.sweek.top/gtobezhtom.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangtech.top/gtqltksauy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.mhx1999.top/gtmzvohxwl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hysaishi.cn/gtqtrocodb.html

Go:   // 手写 map[T]int
来源：http://hz.zhongyouzk.top/gtushocnhv.html

Ruby: arr.tally
来源：http://hz.jqgufenzy.top/gtddizablv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xuanzx.com/gtwixgfsmi.html

[D21] 判断是否包含某元素
来源：http://hz.9152youxi.cn/gtqmsrwyrh.html

Py:   x in arr
来源：http://hz.yanxiufei.cn/gtjyjuxvhi.html

PHP:  in_array($x, $arr, true);
来源：http://hz.svipenyu.cn/gtzijczjfp.html

JS:   arr.includes(x)
来源：http://hz.yongpay.top/gthrkhdewy.html

TS:   arr.includes(x)
来源：http://hz.jiagoushi.top/gtinyzamxj.html

Java: list.contains(x)
来源：http://hz.chenzaomai.com/gtjcxflugs.html

Go:   slices.Contains(arr, x)
来源：http://hz.gotoacloud.top/gtwmppdabh.html

Ruby: arr.include?(x)
来源：http://hz.jinyuanbaomall.cn/gtflprbiyg.html

C#:   list.Contains(x)
来源：http://hz.cashguo.top/gtktjikldd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jyoumei.cn/gttugyjwgw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.redwolf501.top/gtpjqruozi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jqgfzy.top/gtfvqcbydc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ydjk.org.cn/gtteouoccm.html

TS:   [...arr];
来源：http://hz.xylfe.cn/gtulfbgfxq.html

Java: new ArrayList<>(list);
来源：http://hz.ehwqpu.com/gtjsucsnwn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cdnleiting.top/gtybvaoyyq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj20258888.top/gtapldgeby.html

C#:   new List<int>(list);
来源：http://hz.sxryk.cn/gtcpbfknza.html

[D23] reduce 累积计算
来源：http://hz.c1oappe.top/gthgfpatse.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jlsjyb.cn/gtbcovnfkj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.chenlongwang.top/gtmwocnxtt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuxming.cn/gtlhqqiiqx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shuidangran.top/gtlreottgg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gaohongyu789.top/gtknpflwul.html

Go:   // 手写循环
来源：http://hz.xingfuxueyuan.xyz/gtkjfagowy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenlongwang.top/gtjcxddnkg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sysykeji.top/gtbpczxsri.html

[D24] 字典 / Map 基本操作
来源：http://hz.guannengcc.top/gtzwmpeopi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhoulong.xyz/gtnvnusoob.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhengqikj.top/gtbsofboro.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhongyouzk.top/gtjjpqjpoz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xuetiantiany.cn/gtltplvjoi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xuanzx.com/gtfabswwlu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.dianchejie.cn/gtblcwsqoh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xylfe.cn/gtltidvlzt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhijiandao.cn/gtqsllkbxa.html

[D25] Set 集合去重与交并差
来源：http://hz.gotoacloud.top/gtzfiablmc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ivvv.top/gtaggxhgxu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yuxming.cn/gtylnnqxyy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yanxiufei.cn/gtldonxnoz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhoulong.xyz/gtozglhzfe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xinyue.icu/gtmmjemlno.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ehwqpu.com/gtnztzkwtw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yanxiufei.cn/gtilyzymdy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.snrcjt.cn/gtagjemsrc.html

[D26] 数组转字符串
来源：http://hz.fengsongda.top/gtgfmcexjk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.fengsongda.top/gtfopafvqo.html

PHP:  implode(", ", $arr);
来源：http://hz.andypj.xyz/gtpqpntaii.html

JS:   arr.join(", ")
来源：http://hz.yonumen.top/gtlzpoplfk.html

TS:   arr.join(", ")
来源：http://hz.ppjwa.cn/gtztvapwsj.html

Java: String.join(", ", list)
来源：http://hz.hongshengwenyu.top/gtbtobffdx.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhijiandao.cn/gtbrkhaowa.html

Ruby: arr.join(", ")
来源：http://hz.tanke756.top/gthzoxfdiq.html

C#:   string.Join(", ", list)
来源：http://hz.chenlongwang.top/gtgswamycp.html

================================================================================
来源：http://hz.zdqjudy.top/gtasmovsgu.html

E. 字符串处理
来源：http://hz.jqgufenzy.top/gtvcjrizvs.html

================================================================================
来源：http://hz.ydzc1.top/gtrzkvmlwo.html

[E01] 拼接字符串
来源：http://hz.shangyingyoupin.top/gtzjvelmlj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinqigufen.top/gtqnklainw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.dashuyun.cn/gtmjvzlfiz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cdnleiting.top/gtntqpwxgf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jyoumei.cn/gtdkkunsyf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.havefunace.top/gtpssqwyas.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.tian-w.cn/gtixtnysbe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cqqwz.cn/gtxoivqqnt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cqqwz.cn/gtovpbiedf.html

[E02] 重复字符串
来源：http://hz.dianchejie.cn/gtbxetnnty.html

Py:   "ab" * 3
来源：http://hz.zdqjudy.top/gtpdmxsshd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ydzc1.top/gtrvkidswf.html

JS:   "ab".repeat(3)
来源：http://hz.zhixingplan.top/gtwufsaopg.html


<!-- 参考信息 -->