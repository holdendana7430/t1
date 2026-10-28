代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://hz.ydzc1.top/gtvmzddgrd.html

C#:   using System.Text;
来源：http://hz.vqdsnc.cn/gtorfdsivp.html

[C12] 立即执行函数 IIFE
来源：http://hz.xziqi.cn/gtnlpjtbqn.html

Py:   (lambda: print("run"))()
来源：http://hz.zhengqikj.top/gtqttabnmk.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ydjk.org.cn/gtmtcbgsap.html

JS:   (() => { console.log("run"); })();
来源：http://hz.svipenyu.cn/gtjuvpcwxl.html

TS:   (() => { console.log("run"); })();
来源：http://hz.daxiang520.top/gtpzlrswyg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.guowangkeji.top/gtfrttxdzo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cdnleiting.top/gtivnryhsk.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinyuanbaomall.cn/gtpamcbyuk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.nanxinkj.top/gtdflblxdi.html

[C13] 类型声明 / 类型注解
来源：http://hz.dianchejie.cn/gtvtzldpsn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hysaishi.cn/gtoqfhkiyb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.andypj.xyz/gtwhhomxud.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.andypj.xyz/gtustyjgea.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhijiandao.cn/gtohelyini.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtjbouaxzz.html

Go:   func add(a, b int) int
来源：http://hz.jianghu66.top/gtmdausxmt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zdqjudy.top/gtelmfgsfg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yueranfly.top/gtcsapmhev.html

[C14] 泛型函数
来源：http://hz.tian-w.cn/gtdlcigmpt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.316326.xyz/gtciagxixv.html

PHP:  // 无泛型
来源：http://hz.xuanzx.com/gtovwjbtwd.html

JS:   // 无泛型
来源：http://hz.hnxiangtu.top/gtrngbknku.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guannengcc.top/gtonyyctio.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenzaomai.com/gtzpykggzr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.tian-w.cn/gtnqrqjats.html

Ruby: # 无泛型
来源：http://hz.yj20258888.top/gtcjmzpiam.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.birdmap.top/gtdlhsgtfx.html

[C15] 解构 / 展开参数
来源：http://hz.bjfxy.top/gtdoqiyrnd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jiagoushi.top/gtjkwavjey.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenlongwang.top/gttepjnvct.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hammf.cn/gtjyofifva.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.aibaodan.cn/gtgctowafh.html

Java: // 无解构
来源：http://hz.gogol.net.cn/gthicpkqve.html

Go:   // 无解构
来源：http://hz.xinyue.icu/gtnfypkton.html

Ruby: a, b = pair
来源：http://hz.xziqi.cn/gtrskabraa.html

C#:   var (a, b) = pair;
来源：http://hz.kuanghao11.cn/gtoshankel.html

[C16] 函数 / 方法重载
来源：http://hz.cqqwz.cn/gtgbhjvdxm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tianlin.xyz/gtbxuqgczf.html

PHP:  // 无重载
来源：http://hz.svipenyu.cn/gttjnfbfxy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shuidangran.top/gtfxgoljoa.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.nwbrower.top/gtndygamqp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jlsjyb.cn/gtxohnjpgo.html

Go:   // 无重载：用不同函数名
来源：http://hz.52xcode.cn/gtmsiozlmv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xingfuxueyuan.xyz/gtyvkpcryu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yuanzhike.top/gtlmkvtdim.html

================================================================================
来源：http://hz.andypj.xyz/gtcdumhzbe.html

D. 数组 / 列表 / 集合
来源：http://hz.xziqi.cn/gtyloifxtm.html

================================================================================
来源：http://hz.zhijiandao.cn/gteilzidxh.html

[D01] 创建数组 / 列表
来源：http://hz.vqdsnc.cn/gttzeaevsa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yj202588.top/gtjpyvxwqf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ehwqpu.com/gtccwfbhom.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhengqikj.top/gtqscuslva.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ywan-chungtsiang.top/gtebrrphav.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guannengcc.top/gtfsesceno.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sufxvd.cn/gtgjvvvppc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.pycfn.com/gttkqfivqw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.nanxinkj.top/gtouysmvog.html

[D02] 追加元素到末尾
来源：http://hz.yvedp.cn/gtebvqefpg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xuetiantiany.cn/gthsowtnny.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.aizwys.cn/gtminbksbq.html

JS:   arr.push(4);
来源：http://hz.yueranfly.top/gtbfwdoyrt.html

TS:   arr.push(4);
来源：http://hz.zdqjudy.top/gtvoadanvw.html

Java: list.add(4);
来源：http://hz.aizwys.cn/gtarwpseyq.html

Go:   arr = append(arr, 4)
来源：http://hz.zdqjudy.top/gtazzihzrg.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hnxiangtu.top/gtmzqjzgll.html

C#:   list.Add(4);
来源：http://hz.zycfv.cn/gtfwctjovs.html

[D03] 在指定位置插入元素
来源：http://hz.jinghuilouyu.cn/gtechlnmor.html

Py:   arr.insert(0, 0)
来源：http://hz.ehwqpu.com/gtepxzsvhe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.tianlin.xyz/gtrjnkhohx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zdqjudy.top/gtsuxcojvl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hnxiangtu.top/gtjtoxiucq.html

Java: list.add(0, 0);
来源：http://hz.hnxiangtu.top/gthaiskkpw.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yongpay.top/gtfiyzaujl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shanyushiyangkeji.top/gtlzrueobo.html

C#:   list.Insert(0, 0);
来源：http://hz.fengsongda.top/gtmfwfajxx.html

[D04] 删除元素
来源：http://hz.c1oappe.top/gtztgrffax.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.andypj.xyz/gtznypjiav.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhixingplan.top/gtlktoqptz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hfpthk.cn/gtnjcoiyfz.html

TS:   arr.splice(0, 1);
来源：http://hz.pycfn.com/gtcxzkzbyb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shangyingyoupin.top/gtrikycwuv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.tian-w.cn/gtqpseeqht.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yuxming.cn/gtckahnezh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.guannengcc.top/gtidsrdymx.html

[D05] 访问与修改元素
来源：http://hz.snrcjt.cn/gtwfvhzcll.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydzc1.top/gtlultwotu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.mhx1999.top/gtpysjemhl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sufxvd.cn/gtorfnrhpz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gotoacloud.top/gtrjqoiuls.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhongyouzk.top/gtcqgmdqve.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.dashuyun.cn/gthvzzkorq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nwbrower.top/gtotmxaudh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtnzhinyww.html

[D06] 数组长度
来源：http://hz.yj20258888.top/gtsufxaipv.html

Py:   len(arr)
来源：http://hz.shanyushiyangkeji.top/gtwxoxsobz.html

PHP:  count($arr);
来源：http://hz.shzxlz.cn/gtoopwveol.html

JS:   arr.length
来源：http://hz.andypj.xyz/gtuvimvilr.html

TS:   arr.length
来源：http://hz.daria6918.cn/gtvbgvqizo.html

Java: list.size();
来源：http://hz.mhx1999.top/gtnhfqolfs.html

Go:   len(arr)
来源：http://hz.dashuyun.cn/gtrmaehngo.html

Ruby: arr.length; arr.size
来源：http://hz.shangyingyoupin.top/gthmrhmrpc.html

C#:   list.Count;
来源：http://hz.shanyushiyangkeji.top/gtdtfhafrj.html

[D07] 切片 / 取子数组
来源：http://hz.zhengqikj.top/gtevhewaja.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yanxiufei.cn/gtuylcjtxt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jlsjyb.cn/gtpostlwky.html

JS:   arr.slice(1, 4);
来源：http://hz.aizwys.cn/gtdyvbxash.html

TS:   arr.slice(1, 4);
来源：http://hz.dashuyun.cn/gtwhzwiekj.html

Java: list.subList(1, 4);
来源：http://hz.yangfankeji.com/gtfdcsfrzy.html

Go:   arr[1:4]
来源：http://hz.guowangkeji.top/gtjdbpvoxp.html

Ruby: arr[1, 3]
来源：http://hz.shangyingyoupin.top/gtaerooadp.html

C#:   list.GetRange(1, 3);
来源：http://hz.gaohongyu789.top/gtauuvdrzd.html

[D08] 合并两个数组
来源：http://hz.9152youxi.cn/gtmsafhnzx.html

Py:   a + b;  a.extend(b)
来源：http://hz.gzhubu.top/gtvbnkiduu.html

PHP:  array_merge($a, $b);
来源：http://hz.zhixingplan.top/gtqzboiiid.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yongpay.top/gtbksrrwia.html

TS:   [...a, ...b];
来源：http://hz.hnxiangtu.top/gtevzwdynp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cucudq.cn/gtkykyzrjt.html

Go:   append(a, b...)
来源：http://hz.nwbrower.top/gtfwfptaer.html

Ruby: a + b;  a.concat(b)
来源：http://hz.52xcode.cn/gtaojosasm.html

C#:   a.Concat(b).ToList()
来源：http://hz.meibo888.top/gtpdjaqjpn.html

[D09] 排序（升序）
来源：http://hz.zhongyouzk.top/gtnongkbwh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.bjfxy.top/gttrgozfum.html

PHP:  sort($arr);
来源：http://hz.shangyingyoupin.top/gtdqsrhcis.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.kuanghao11.cn/gtjkwvytec.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.nwbrower.top/gtjwpointv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gaohongyu789.top/gtwvilsphj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zycfv.cn/gtqmhochae.html

Ruby: arr.sort
来源：http://hz.yj202588.top/gtaslzfyip.html

C#:   list.Sort();
来源：http://hz.daxiang520.top/gtchtjmiet.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cdnleiting.top/gtzjqrnoui.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenzaomai.com/gtqdrjfqtf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jyoumei.cn/gttgcvoxig.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hfpthk.cn/gtdjzttntf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhixingplan.top/gtywyqbzrp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yonumen.top/gtuizmktza.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.kuanghao11.cn/gtucllwboz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hysaishi.cn/gtumcowvdu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinyuanbaomall.cn/gtzezhjfnu.html

[D11] 反转数组
来源：http://hz.chenlongwang.top/gtqptzpvbg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ybcxt.top/gtitamuotp.html

PHP:  array_reverse($arr);
来源：http://hz.ydjk.org.cn/gtaenrzvbb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.redwolf501.top/gtrbvkwefe.html

TS:   [...arr].reverse();
来源：http://hz.xuetiantiany.cn/gtkjulzcgu.html

Java: Collections.reverse(list);
来源：http://hz.nanxinkj.top/gtfefgrdrf.html

Go:   slices.Reverse(arr)
来源：http://hz.yonumen.top/gtdortvtui.html

Ruby: arr.reverse
来源：http://hz.vqdsnc.cn/gtabvyajwh.html

C#:   list.Reverse();
来源：http://hz.cdnleiting.top/gtmfptymjx.html

[D12] 查找元素下标
来源：http://hz.ydjk.org.cn/gtinanmnlg.html

Py:   arr.index(x);  x in arr
来源：http://hz.havefunace.top/gtxlggtelh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ybcxt.top/gtofzisteu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xziqi.cn/gtanprnmtm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hammf.cn/gtmdvxaqaa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nwbrower.top/gtqrjvxrrk.html

Go:   slices.Index(arr, x)
来源：http://hz.ivvv.top/gtyhebeuqx.html

Ruby: arr.index(x)
来源：http://hz.iojbl.cn/gtflrmthok.html

C#:   list.IndexOf(x);
来源：http://hz.birdmap.top/gtzbowestu.html

[D13] 过滤（保留满足条件的）
来源：http://hz.9152youxi.cn/gtilamhlyt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.andypj.xyz/gtecjpinrk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.guowangkeji.top/gtscrjgrqa.html

JS:   arr.filter(x => x > 3)
来源：http://hz.dianchejie.cn/gtvkjoicvd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daxiang520.top/gtgqwdkdqg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinqigfzy.top/gtdewzwrop.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.sysykeji.top/gtbiuuxvdk.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhoulong.xyz/gtfhxrbjpa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.bjfxy.top/gtjsliissp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yj20258.top/gtbdkgpyoz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.vqdsnc.cn/gtnreyxxgc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cashguo.top/gtlsdvuais.html

JS:   arr.map(x => x * 2)
来源：http://hz.wangdashe.top/gtisehbash.html

TS:   arr.map(x => x * 2)
来源：http://hz.andypj.xyz/gtzfmgdbqf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jyoumei.cn/gteaavarpm.html

Go:   // 手写循环
来源：http://hz.zhiwuduotai.top/gtmqvkompg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.kuanghao11.cn/gtikivtfmy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.haohaochexian.top/gtnrhdqklf.html

[D15] 去重
来源：http://hz.cdnleiting.top/gtyutqizmz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nwbrower.top/gthuucjfwl.html

PHP:  array_unique($arr);
来源：http://hz.jiagoushi.top/gtapakqqmn.html

JS:   [...new Set(arr)]
来源：http://hz.hongshengwenyu.top/gtlxlyzcna.html

TS:   [...new Set(arr)]
来源：http://hz.gogol.net.cn/gtsswforxi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cashguo.top/gthnejqfny.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xuetiantiany.cn/gtbbchpitx.html

Ruby: arr.uniq
来源：http://hz.xuanzx.com/gtmhyuycxs.html

C#:   list.Distinct().ToList()
来源：http://hz.gotoacloud.top/gtholmaobi.html

[D16] 求和与平均值
来源：http://hz.cqqwz.cn/gtnuwtvmxh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shuidangran.top/gtfdvoabrx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zdqjudy.top/gtzjakhunc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenlongwang.top/gtakmvxtrn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shzxlz.cn/gtcdhzdgvj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xylfe.cn/gtyrgveqfg.html

Go:   // 手写循环累加
来源：http://hz.jiagoushi.top/gtiglifluo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.iojbl.cn/gthsuskijk.html

C#:   list.Sum();  list.Average()
来源：http://hz.316326.xyz/gtuwhenjuv.html

[D17] 最大值与最小值
来源：http://hz.fengsongda.top/gtdmmysprd.html

Py:   max(arr);  min(arr)
来源：http://hz.dianchejie.cn/gtbokrfdfq.html

PHP:  max($arr);  min($arr);
来源：http://hz.wangdashe.top/gtttqueocq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hysaishi.cn/gtwhikmhvk.html

TS:   Math.max(...arr);
来源：http://hz.0kj1m.cn/gtbadvlsob.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.haohaochexian.top/gtlwtttbsm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cashguo.top/gtsbrdsdhe.html

Ruby: arr.max;  arr.min
来源：http://hz.yonumen.top/gtcaevjkah.html

C#:   list.Max();  list.Min()
来源：http://hz.jinqigfzy.top/gtuwmozbug.html

[D18] 扁平化嵌套数组
来源：http://hz.guannengcc.top/gtxaubhfyq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.fzhhl.top/gtgjewwnhf.html

PHP:  array_merge(...$nested);
来源：http://hz.fengsongda.top/gtoyxdhvxw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.havefunace.top/gtcihyzolp.html

TS:   nested.flat();
来源：http://hz.gotoacloud.top/gtoypfgpfh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gaohongyu789.top/gtovhmhoye.html

Go:   // 手写双层循环
来源：http://hz.xuetiantiany.cn/gtzgfvvvul.html

Ruby: nested.flatten
来源：http://hz.zhaomingkeji.xyz/gtoucdlgcy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.snrcjt.cn/gtfajxfbke.html

[D19] 按字段分组
来源：http://hz.jqgufenzy.top/gtplkdugjm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sweek.top/gtqlxbpfbf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.smart0.xyz/gtakfesdrk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.nwbrower.top/gtxvqamkge.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ybcxt.top/gtphiyvlmk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.0kj1m.cn/gtrxvdsztb.html

Go:   // 手写 map[string][]T
来源：http://hz.sweek.top/gtfqdwiasp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hongshengwenyu.top/gthnaycvcf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xziqi.cn/gtsyxaxvlj.html

[D20] 统计每个元素出现次数
来源：http://hz.pengpengdd.cyou/gtyypebblx.html

Py:   Counter(arr)
来源：http://hz.cqqwz.cn/gtdochgido.html

PHP:  array_count_values($arr);
来源：http://hz.pengpengdd.cyou/gtjncgsjuv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pengpengdd.cyou/gtmqqupayp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xziqi.cn/gthzubrikq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.aizwys.cn/gtvtqzjpsf.html

Go:   // 手写 map[T]int
来源：http://hz.yanxiufei.cn/gtjfubnmal.html

Ruby: arr.tally
来源：http://hz.zdqjudy.top/gttcddyalb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gotoacloud.top/gtdtbxjkcl.html

[D21] 判断是否包含某元素
来源：http://hz.zycfv.cn/gtfxknljtm.html

Py:   x in arr
来源：http://hz.sufxvd.cn/gtnrqoztap.html

PHP:  in_array($x, $arr, true);
来源：http://hz.havefunace.top/gtgkwxeoal.html

JS:   arr.includes(x)
来源：http://hz.zhiwuduotai.top/gtoexaypeg.html

TS:   arr.includes(x)
来源：http://hz.zhixingplan.top/gtznewtyql.html

Java: list.contains(x)
来源：http://hz.ivvv.top/gtnlmnkraj.html

Go:   slices.Contains(arr, x)
来源：http://hz.dianchejie.cn/gtjilptlwg.html

Ruby: arr.include?(x)
来源：http://hz.bjfxy.top/gtggftnivo.html

C#:   list.Contains(x)
来源：http://hz.zdqjudy.top/gtlicvzfcq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shzxlz.cn/gtrtajzefp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cheryme.top/gtohpxffct.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.chenlongwang.top/gtkhmuxwqd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinghuilouyu.cn/gtbzmjjgib.html

TS:   [...arr];
来源：http://hz.aizwys.cn/gtdgfrumpe.html

Java: new ArrayList<>(list);
来源：http://hz.pycfn.com/gtjsabvnkp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.wangshuangyany.cn/gtsjqispbk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.316326.xyz/gtnbrgmpxa.html

C#:   new List<int>(list);
来源：http://hz.daxiang520.top/gtncllslei.html

[D23] reduce 累积计算
来源：http://hz.9152youxi.cn/gtsrgzesqk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhijiandao.cn/gtdkmivsyz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hysaishi.cn/gtkmormdom.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.quarkkingdee.top/gtirrrcfmc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gtvyjlvtkk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zycfv.cn/gtymutnjxb.html

Go:   // 手写循环
来源：http://hz.jlsjyb.cn/gtwevcnyii.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cqqwz.cn/gtwllspavc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.svipenyu.cn/gtlzxwvbhs.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj202588.top/gtruqagbyn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.iojbl.cn/gtludaulgq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhaomingkeji.xyz/gtgllabmrd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xylfe.cn/gtzdhooubn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sweek.top/gtaogmdvvq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yanxiufei.cn/gtnwbsieea.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ivvv.top/gtlubmrasw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jlsjyb.cn/gtmvyouunw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xylfe.cn/gtojyhucjm.html

[D25] Set 集合去重与交并差
来源：http://hz.chenlongwang.top/gtlkpvtuks.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xinyue.icu/gtjfesiqcm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.haohaochexian.top/gtxoaasrgt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.svipenyu.cn/gtizjylbvz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.pycfn.com/gtftzehunx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cdnleiting.top/gtwozfeujy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.redwolf501.top/gtkpdtjxde.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.aizwys.cn/gtavsxaprk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shzxlz.cn/gtwhycowqp.html

[D26] 数组转字符串
来源：http://hz.jiagoushi.top/gtzilubpom.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hnqzz.top/gtosulworm.html

PHP:  implode(", ", $arr);
来源：http://hz.ybcxt.top/gtkheumpdj.html

JS:   arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtglmgxqso.html

TS:   arr.join(", ")
来源：http://hz.redwolf501.top/gteqfemneo.html

Java: String.join(", ", list)
来源：http://hz.zdqjudy.top/gtswxefcjv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinghuilouyu.cn/gtchfyfkla.html

Ruby: arr.join(", ")
来源：http://hz.c1oappe.top/gtbkyncqyv.html

C#:   string.Join(", ", list)
来源：http://hz.feifeiyinyue.top/gtvfdxfrza.html

================================================================================
来源：http://hz.nwbrower.top/gtzgcekzgh.html

E. 字符串处理
来源：http://hz.hongshengwenyu.top/gtanbkpird.html

================================================================================
来源：http://hz.mhx1999.top/gtiyrprbjk.html

[E01] 拼接字符串
来源：http://hz.hysaishi.cn/gtqogsvmfu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.chenlongwang.top/gtmpvnopyb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.fzhhl.top/gtbssmdauy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhengqikj.top/gtcjuddduc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sweek.top/gtifyaupgc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhoulong.xyz/gtarqyzpqj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hywenlv.cn/gteopakopl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinqigfzy.top/gtziroqcyj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.pycfn.com/gtngutkruq.html

[E02] 重复字符串
来源：http://hz.jinghuilouyu.cn/gtdjnzuizv.html

Py:   "ab" * 3
来源：http://hz.bjfxy.top/gtudgagixm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.bjfxy.top/gtcyaqdmaw.html

JS:   "ab".repeat(3)
来源：http://hz.c1oappe.top/gtejcrqdqy.html


<!-- 参考信息 -->