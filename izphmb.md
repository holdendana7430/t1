代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://hz.wangdashe.top/gtkxoalmvw.html

C#:   using System.Text;
来源：http://hz.zhengqikj.top/gtatfnuxgy.html

[C12] 立即执行函数 IIFE
来源：http://hz.birdmap.top/gtlhxulhip.html

Py:   (lambda: print("run"))()
来源：http://hz.pengpengdd.cyou/gttphsjhmx.html

PHP:  (function () { echo "run"; })();
来源：http://hz.dianchejie.cn/gtmoypvgxg.html

JS:   (() => { console.log("run"); })();
来源：http://hz.vqdsnc.cn/gtmciakxku.html

TS:   (() => { console.log("run"); })();
来源：http://hz.dianchejie.cn/gthamoyqpv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.vqdsnc.cn/gttuwniqlh.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.0kj1m.cn/gtqhaewdsm.html

Ruby: -> { puts "run" }.call
来源：http://hz.feifeiyinyue.top/gtwoixjyvv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zycfv.cn/gtanbfdafp.html

[C13] 类型声明 / 类型注解
来源：http://hz.xinyue.icu/gtsjcekmbe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shanyushiyangtech.top/gtyyuuhevm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuetiantiany.cn/gtnqhnxipe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.svipenyu.cn/gtibczlzzy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgufenzy.top/gtcmpiuwei.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gteawytdxw.html

Go:   func add(a, b int) int
来源：http://hz.xziqi.cn/gtgttvkuwr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shangyingyoupin.top/gtedrzdkcc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.guannengcc.top/gtzrbnawij.html

[C14] 泛型函数
来源：http://hz.jinqigufen.top/gtybhvcdyr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.pycfn.com/gtqywmmgdg.html

PHP:  // 无泛型
来源：http://hz.sweek.top/gtxmodpamd.html

JS:   // 无泛型
来源：http://hz.jinqigfzy.top/gtpuamevmd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shuidangran.top/gtudgoosko.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.aibaodan.cn/gtdyuuopbq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.fengsongda.top/gtucqaksmd.html

Ruby: # 无泛型
来源：http://hz.vqdsnc.cn/gtxyjigekc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.tanke756.top/gtlmbopmdd.html

[C15] 解构 / 展开参数
来源：http://hz.ybcxt.top/gtqsorumgf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cqqwz.cn/gticbonxab.html

PHP:  [$a, $b] = $pair;
来源：http://hz.vqdsnc.cn/gtssuipjal.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinghuilouyu.cn/gtvhnhdtor.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhixingplan.top/gtsgmopgly.html

Java: // 无解构
来源：http://hz.andypj.xyz/gttjfahxtw.html

Go:   // 无解构
来源：http://hz.316326.xyz/gtjyaopwop.html

Ruby: a, b = pair
来源：http://hz.xuanzx.com/gtlexgadxk.html

C#:   var (a, b) = pair;
来源：http://hz.gzhubu.top/gtgxidsxmx.html

[C16] 函数 / 方法重载
来源：http://hz.iojbl.cn/gtrvdtfcdr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xinyue.icu/gtswjhfgsb.html

PHP:  // 无重载
来源：http://hz.xylfe.cn/gtlotjchya.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.daria6918.cn/gtnldykfkg.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.vqdsnc.cn/gtmxlnttqx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.havefunace.top/gthkgappze.html

Go:   // 无重载：用不同函数名
来源：http://hz.dianchejie.cn/gtdspqxcgv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhengqikj.top/gtucxlstzj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xinyue.icu/gtytkfqsxy.html

================================================================================
来源：http://hz.yueranfly.top/gtvvpfmsrm.html

D. 数组 / 列表 / 集合
来源：http://hz.yonumen.top/gtapvhwxdt.html

================================================================================
来源：http://hz.redwolf501.top/gtegksnetj.html

[D01] 创建数组 / 列表
来源：http://hz.nanxuanxn.top/gtgtfxatpn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.tianlin.xyz/gthnuxzlgr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.andypj.xyz/gtegwgtekq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.haohaochexian.top/gtecpcigsi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.gotoacloud.top/gtvwxtgbzx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.mhx1999.top/gtamxqlpeg.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinqigufen.top/gteoimctll.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jinqigfzy.top/gtzejlupri.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.tian-w.cn/gtqbyoymkh.html

[D02] 追加元素到末尾
来源：http://hz.tian-w.cn/gtmqgmukfy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.vqdsnc.cn/gtzzejzvji.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.kuanghao11.cn/gtjhjtnwsz.html

JS:   arr.push(4);
来源：http://hz.gotoacloud.top/gtgkfpwnjd.html

TS:   arr.push(4);
来源：http://hz.hywenlv.cn/gtfeqfuzid.html

Java: list.add(4);
来源：http://hz.sysykeji.top/gtafmsgltf.html

Go:   arr = append(arr, 4)
来源：http://hz.jiagoushi.top/gtrnbisnvq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.316326.xyz/gtjfiqltml.html

C#:   list.Add(4);
来源：http://hz.yuxming.cn/gtcxjnudcj.html

[D03] 在指定位置插入元素
来源：http://hz.316326.xyz/gtnhosxkmh.html

Py:   arr.insert(0, 0)
来源：http://hz.ydjk.org.cn/gtnwpiazjc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ehwqpu.com/gtpytuabaw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhiwuduotai.top/gtdkczehmp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xingfuxueyuan.xyz/gtzbiuxnrv.html

Java: list.add(0, 0);
来源：http://hz.xingfuxueyuan.xyz/gtdcjfeotj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.aibaodan.cn/gthaagfnlu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinqigufen.top/gtaqkstwwo.html

C#:   list.Insert(0, 0);
来源：http://hz.hnqzz.top/gtshbymfgo.html

[D04] 删除元素
来源：http://hz.jinqigfzy.top/gtjlodahbj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jianghu66.top/gtgmaiumnk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.bjfxy.top/gtgdyuzfjr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yj202588.top/gtpkrrddpq.html

TS:   arr.splice(0, 1);
来源：http://hz.gotoacloud.top/gtcwwyphkr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.meibo888.top/gtoarfcasn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.havefunace.top/gtzfhledjf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yongpay.top/gtmagwisus.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.wangdashe.top/gtsehbbcnv.html

[D05] 访问与修改元素
来源：http://hz.bjfxy.top/gtapznfbgt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ybcxt.top/gtqtohfvly.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.fzhhl.top/gtkqkhtbki.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.kuanghao11.cn/gtomxyarxf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yuxming.cn/gthvkhkcaq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.nanxuanxn.top/gtmntcpzgo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.meibo888.top/gtaiybmazf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xinyue.icu/gtriojejve.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hongshengwenyu.top/gtodyxgeom.html

[D06] 数组长度
来源：http://hz.pycfn.com/gtensisxxd.html

Py:   len(arr)
来源：http://hz.jyoumei.cn/gtdovdjarh.html

PHP:  count($arr);
来源：http://hz.zhaomingkeji.xyz/gtdwjpsldu.html

JS:   arr.length
来源：http://hz.guowangkeji.top/gtwfiuhlxj.html

TS:   arr.length
来源：http://hz.meibo888.top/gtzxmjhgza.html

Java: list.size();
来源：http://hz.snrcjt.cn/gtarvrixgd.html

Go:   len(arr)
来源：http://hz.yuanzhike.top/gtbrzobasf.html

Ruby: arr.length; arr.size
来源：http://hz.nwbrower.top/gttxpcaora.html

C#:   list.Count;
来源：http://hz.ydzc1.top/gtjjojsnmw.html

[D07] 切片 / 取子数组
来源：http://hz.iojbl.cn/gtrdwsbpog.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nanxinkj.top/gtfsxcxkna.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.iojbl.cn/gtwuxtbleh.html

JS:   arr.slice(1, 4);
来源：http://hz.smart0.xyz/gtyesunzua.html

TS:   arr.slice(1, 4);
来源：http://hz.xziqi.cn/gtjptdpity.html

Java: list.subList(1, 4);
来源：http://hz.hfpthk.cn/gtwtjzbjty.html

Go:   arr[1:4]
来源：http://hz.snrcjt.cn/gtpcwahxoy.html

Ruby: arr[1, 3]
来源：http://hz.zdqjudy.top/gtwcndsgfd.html

C#:   list.GetRange(1, 3);
来源：http://hz.yvedp.cn/gtwilnqhra.html

[D08] 合并两个数组
来源：http://hz.birdmap.top/gtynvrdhjv.html

Py:   a + b;  a.extend(b)
来源：http://hz.cdnleiting.top/gtxtexdxub.html

PHP:  array_merge($a, $b);
来源：http://hz.guowangkeji.top/gtlrpxtiki.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.vqdsnc.cn/gtasvpkjod.html

TS:   [...a, ...b];
来源：http://hz.chenlongwang.top/gtzledvjba.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.fengsongda.top/gtounhdzin.html

Go:   append(a, b...)
来源：http://hz.zhixingplan.top/gtirdawjgd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.haohaochexian.top/gtrxkxpqqb.html

C#:   a.Concat(b).ToList()
来源：http://hz.daxiang520.top/gtomrbqzim.html

[D09] 排序（升序）
来源：http://hz.yangfankeji.com/gtnqhplune.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hywenlv.cn/gtxabvaumr.html

PHP:  sort($arr);
来源：http://hz.hysaishi.cn/gtorovlwcv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.guannengcc.top/gtipnhjcxb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sysykeji.top/gtqlaetryg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.kuanghao11.cn/gtreizcwep.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jlsjyb.cn/gtgjbtoyjb.html

Ruby: arr.sort
来源：http://hz.bjfxy.top/gtvhrgrnnm.html

C#:   list.Sort();
来源：http://hz.havefunace.top/gtzhlgewcr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jqgufenzy.top/gtzzwddduh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.dashuyun.cn/gtjypsnscq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gtdzoizipd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hywenlv.cn/gtqnhphmsc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtmcqufmbo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shzxlz.cn/gtjuuecucf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gogol.net.cn/gtlwxtskvs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hammf.cn/gtwsedjouz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zdqjudy.top/gtyfvenwau.html

[D11] 反转数组
来源：http://hz.guannengcc.top/gtbzgoqico.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xinyue.icu/gticowesur.html

PHP:  array_reverse($arr);
来源：http://hz.zhoulong.xyz/gtylneahlx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.fengsongda.top/gthlcdopxh.html

TS:   [...arr].reverse();
来源：http://hz.yangfankeji.com/gtuupccwlo.html

Java: Collections.reverse(list);
来源：http://hz.zhengqikj.top/gtzmpwfqea.html

Go:   slices.Reverse(arr)
来源：http://hz.hywenlv.cn/gtogtyztld.html

Ruby: arr.reverse
来源：http://hz.jianghu66.top/gtxomeowjm.html

C#:   list.Reverse();
来源：http://hz.yj20258888.top/gtsgrrjqtc.html

[D12] 查找元素下标
来源：http://hz.yvedp.cn/gtgoltpynk.html

Py:   arr.index(x);  x in arr
来源：http://hz.feifeiyinyue.top/gtzaeuynwu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.guannengcc.top/gtsgwdvijj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.meibo888.top/gtjgwrytfl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jyoumei.cn/gtbtjsivir.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nanxuanxn.top/gtnvfqquxr.html

Go:   slices.Index(arr, x)
来源：http://hz.mhx1999.top/gtevprdrah.html

Ruby: arr.index(x)
来源：http://hz.xuanzx.com/gtrqjzxqov.html

C#:   list.IndexOf(x);
来源：http://hz.meibo888.top/gtfgxnqrfe.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhengqikj.top/gtcoyqqovt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.pengpengdd.cyou/gtahvdknds.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yj20258.top/gtmqelpxjf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.cdnleiting.top/gtazcadsau.html

TS:   arr.filter(x => x > 3)
来源：http://hz.haohaochexian.top/gtbqupercu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cashguo.top/gtzedmbvve.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.quarkkingdee.top/gtsmmiumrg.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ehwqpu.com/gtwvaasgzv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.birdmap.top/gtfaixadny.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cdnleiting.top/gtwmxvdchg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ydzc1.top/gturokjvjf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.dianchejie.cn/gtivnpwydt.html

JS:   arr.map(x => x * 2)
来源：http://hz.havefunace.top/gterjhjdab.html

TS:   arr.map(x => x * 2)
来源：http://hz.yongpay.top/gtgnrfgqtb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ybcxt.top/gtssejoqku.html

Go:   // 手写循环
来源：http://hz.daria6918.cn/gtqoyursla.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.wangdashe.top/gtnommlclh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinqigufen.top/gtlfucplbt.html

[D15] 去重
来源：http://hz.cheryme.top/gtjooujgpy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zycfv.cn/gtcwxrzhoo.html

PHP:  array_unique($arr);
来源：http://hz.guowangkeji.top/gtrfqhusfk.html

JS:   [...new Set(arr)]
来源：http://hz.jinghuilouyu.cn/gttrxmqwcy.html

TS:   [...new Set(arr)]
来源：http://hz.pycfn.com/gtmoipzflm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yueranfly.top/gtybdjudch.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hywenlv.cn/gtxifjxpek.html

Ruby: arr.uniq
来源：http://hz.ydzc1.top/gtgpanzkjv.html

C#:   list.Distinct().ToList()
来源：http://hz.aibaodan.cn/gtffrokwir.html

[D16] 求和与平均值
来源：http://hz.zdqjudy.top/gtaqcpmgno.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhiwuduotai.top/gtyrazyelr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fengsongda.top/gthrmmzfoy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gzhubu.top/gtkmnsagxm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhengqikj.top/gtdtmyaccl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.guannengcc.top/gtizpvpdzg.html

Go:   // 手写循环累加
来源：http://hz.iojbl.cn/gtxqvehzje.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhiwuduotai.top/gtvohvkuey.html

C#:   list.Sum();  list.Average()
来源：http://hz.ybcxt.top/gtwlhfjndh.html

[D17] 最大值与最小值
来源：http://hz.yj20258.top/gtlgmwxgip.html

Py:   max(arr);  min(arr)
来源：http://hz.chenlongwang.top/gttjzzjsdw.html

PHP:  max($arr);  min($arr);
来源：http://hz.shangyingyoupin.top/gtnzojsxte.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shzxlz.cn/gtrdtgacna.html

TS:   Math.max(...arr);
来源：http://hz.redwolf501.top/gtwupyyhaq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.havefunace.top/gtnsxlncmg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xinyue.icu/gtjltxzfci.html

Ruby: arr.max;  arr.min
来源：http://hz.zhixingplan.top/gtlcaxkhyj.html

C#:   list.Max();  list.Min()
来源：http://hz.jinqigufen.top/gtiqlajvgh.html

[D18] 扁平化嵌套数组
来源：http://hz.yueranfly.top/gtxapnsplm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenzaomai.com/gtxlufphxj.html

PHP:  array_merge(...$nested);
来源：http://hz.nwbrower.top/gtlnxdxewn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinyuanbaomall.cn/gtyaliblvs.html

TS:   nested.flat();
来源：http://hz.gotoacloud.top/gtbleuizks.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cdnleiting.top/gtheupnrow.html

Go:   // 手写双层循环
来源：http://hz.xylfe.cn/gtdyvrdxby.html

Ruby: nested.flatten
来源：http://hz.shanyushiyangkeji.top/gtyhiidpgn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jqgufenzy.top/gtecharfba.html

[D19] 按字段分组
来源：http://hz.chenlongwang.top/gtognnqbba.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.tian-w.cn/gtivgxklko.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhiwuduotai.top/gtyzpexfeg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ywan-chungtsiang.top/gtwwzyqktl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.mhx1999.top/gtlrnpouci.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.svipenyu.cn/gtddmwrunl.html

Go:   // 手写 map[string][]T
来源：http://hz.nanxuanxn.top/gtvwsqumvu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.nanxuanxn.top/gtcjrzeiny.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yuxming.cn/gtimvtfkks.html

[D20] 统计每个元素出现次数
来源：http://hz.svipenyu.cn/gtfnfifyfn.html

Py:   Counter(arr)
来源：http://hz.yj202588.top/gteptklhny.html

PHP:  array_count_values($arr);
来源：http://hz.zhijiandao.cn/gtiwzwcias.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pengpengdd.cyou/gthyduupth.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinyuanbaomall.cn/gtxcdpdkvp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jqgufenzy.top/gttdwsludt.html

Go:   // 手写 map[T]int
来源：http://hz.pengpengdd.cyou/gtzniosdss.html

Ruby: arr.tally
来源：http://hz.wangshuangyany.cn/gtlepmgrlx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hnxiangtu.top/gtljobasrn.html

[D21] 判断是否包含某元素
来源：http://hz.chenjidiqi.icu/gtqbkewqps.html

Py:   x in arr
来源：http://hz.sufxvd.cn/gtzxlvufan.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xuetiantiany.cn/gtrufuhfvm.html

JS:   arr.includes(x)
来源：http://hz.xinyue.icu/gtulxezwlt.html

TS:   arr.includes(x)
来源：http://hz.yuxming.cn/gtqwsufrmm.html

Java: list.contains(x)
来源：http://hz.shzxlz.cn/gtnggsakyi.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuanzhike.top/gtpkdynluo.html

Ruby: arr.include?(x)
来源：http://hz.ivvv.top/gtviuzcbfv.html

C#:   list.Contains(x)
来源：http://hz.yongpay.top/gtjjfngiqu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shuidangran.top/gtudjjwdcd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yueranfly.top/gtcwuuhorp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.svipenyu.cn/gtufkzvnzb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinyuanbaomall.cn/gtqmwlurqy.html

TS:   [...arr];
来源：http://hz.nwbrower.top/gtaavpuyau.html

Java: new ArrayList<>(list);
来源：http://hz.yj20258888.top/gtmivczefi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.smart0.xyz/gtozcjpgvz.html

Ruby: arr.dup;  arr.clone
来源：http://hz.chenlongwang.top/gtcjhhjlbm.html

C#:   new List<int>(list);
来源：http://hz.xuanzx.com/gtlcvvwubb.html

[D23] reduce 累积计算
来源：http://hz.chenlongwang.top/gtpqlpuzjm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.andypj.xyz/gtnykvyezy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.chenlongwang.top/gtiasakgrq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.vqdsnc.cn/gtvffsnyal.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenzaomai.com/gtpgyubhme.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hywenlv.cn/gtjridhpnb.html

Go:   // 手写循环
来源：http://hz.hywenlv.cn/gtfxkgzewe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gzhubu.top/gtdrgkxqvt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.wangshuangyany.cn/gtztvwyovf.html

[D24] 字典 / Map 基本操作
来源：http://hz.ppjwa.cn/gtfuiwztes.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sweek.top/gtcricvidd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yj20258888.top/gtjksjbnsq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.andypj.xyz/gtjpewfzcm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.nanxuanxn.top/gthjjfxgmu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shanyushiyangkeji.top/gtfgdektmm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ydjk.org.cn/gtovsobcbr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yj20258.top/gtzotiaxlk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.wangdashe.top/gtwilajibf.html

[D25] Set 集合去重与交并差
来源：http://hz.tianlin.xyz/gtjpglzkru.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yonumen.top/gtczbjvtsd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.sysykeji.top/gthcipxagc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.52xcode.cn/gtvfxnhrni.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cdnleiting.top/gtfubvttge.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.chenlongwang.top/gtngfyxfhf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinghuilouyu.cn/gtnoxhlifj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgfzy.top/gtxzgvtixm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sweek.top/gtbajxsutw.html

[D26] 数组转字符串
来源：http://hz.zhongyouzk.top/gttggtoxlk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yuxming.cn/gtewzehqer.html

PHP:  implode(", ", $arr);
来源：http://hz.jinqigfzy.top/gtqmzotvjs.html

JS:   arr.join(", ")
来源：http://hz.svipenyu.cn/gtlkehkgsn.html

TS:   arr.join(", ")
来源：http://hz.cdnleiting.top/gtxpsnakgb.html

Java: String.join(", ", list)
来源：http://hz.aibaodan.cn/gtscdwcfcr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.andypj.xyz/gtnsuymtad.html

Ruby: arr.join(", ")
来源：http://hz.havefunace.top/gtetqfixvi.html

C#:   string.Join(", ", list)
来源：http://hz.jianghu66.top/gtsmysoggn.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtjooieffi.html

E. 字符串处理
来源：http://hz.kuanghao11.cn/gtxjqvdyue.html

================================================================================
来源：http://hz.meibo888.top/gtjanvvjvp.html

[E01] 拼接字符串
来源：http://hz.yvedp.cn/gtlowaepzn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.smart0.xyz/gtpuqwonyn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ppjwa.cn/gthagqbnrc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydzc1.top/gtwmnhyhkt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.0kj1m.cn/gtsowszzgs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.haohaochexian.top/gtgaulwbub.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yonumen.top/gtqgobhojz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ybcxt.top/gtdwoqsatm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ivvv.top/gtkfflffah.html

[E02] 重复字符串
来源：http://hz.ydzc1.top/gtqhtmmdud.html

Py:   "ab" * 3
来源：http://hz.gotoacloud.top/gtolberhga.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zycfv.cn/gtvymyyhgx.html

JS:   "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtdkqzyvmg.html


<!-- 参考信息 -->