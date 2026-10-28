代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://hz.xziqi.cn/gtogxsdmkl.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sysykeji.top/gthwzkwvoa.html

TS:   (() => { console.log("run"); })();
来源：http://hz.chenjidiqi.icu/gtitgevdxc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sysykeji.top/gthqneixbt.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.52xcode.cn/gteuodocxt.html

Ruby: -> { puts "run" }.call
来源：http://hz.cdnleiting.top/gtqaiyuono.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.haohaochexian.top/gtvhlutgxe.html

[C13] 类型声明 / 类型注解
来源：http://hz.havefunace.top/gtjvdqvkba.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.feifeiyinyue.top/gteugtrbrw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fzhhl.top/gtbqxkuyjr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhijiandao.cn/gtsgykttvb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenjidiqi.icu/gtwtrzswoc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gtldtzkjkx.html

Go:   func add(a, b int) int
来源：http://hz.pengpengdd.cyou/gtewwsbfbj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinqigfzy.top/gtnrbcgkwd.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yangfankeji.com/gtgksghgic.html

[C14] 泛型函数
来源：http://hz.shanyushiyangtech.top/gtayuimjqy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.daxiang520.top/gtgsmeqhns.html

PHP:  // 无泛型
来源：http://hz.guannengcc.top/gterlzgtmm.html

JS:   // 无泛型
来源：http://hz.guannengcc.top/gtlvnddzxs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xuanzx.com/gtrfliakji.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yj20258888.top/gttbhhupun.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinqigfzy.top/gtbetaxxjh.html

Ruby: # 无泛型
来源：http://hz.zhongyouzk.top/gticzsmlto.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xingfuxueyuan.xyz/gtmjdzborp.html

[C15] 解构 / 展开参数
来源：http://hz.shanyushiyangkeji.top/gtpptmsuxh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinqigufen.top/gtrllbhicm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gotoacloud.top/gtfhgrikgl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinqigfzy.top/gtzkyobcvd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhengqikj.top/gtiaegmove.html

Java: // 无解构
来源：http://hz.0kj1m.cn/gtkbrxvyxd.html

Go:   // 无解构
来源：http://hz.ehwqpu.com/gtisnbfdbe.html

Ruby: a, b = pair
来源：http://hz.shanyushiyangtech.top/gtsduomsvr.html

C#:   var (a, b) = pair;
来源：http://hz.kuanghao11.cn/gtbppfiawl.html

[C16] 函数 / 方法重载
来源：http://hz.redwolf501.top/gtefeumnlk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gotoacloud.top/gtezfpopab.html

PHP:  // 无重载
来源：http://hz.meibo888.top/gtohjgpgye.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yvedp.cn/gtvxlasdhn.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xylfe.cn/gtljqwodkx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.guannengcc.top/gtsmpkstol.html

Go:   // 无重载：用不同函数名
来源：http://hz.wangdashe.top/gtscrsqwjp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gogol.net.cn/gtwdluvbzf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhoulong.xyz/gtwrcyljhd.html

================================================================================
来源：http://hz.yvedp.cn/gtxsgijsrm.html

D. 数组 / 列表 / 集合
来源：http://hz.jinghuilouyu.cn/gtatzgxzcr.html

================================================================================
来源：http://hz.smart0.xyz/gtyikihcdg.html

[D01] 创建数组 / 列表
来源：http://hz.chenjidiqi.icu/gtcazslabz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yj202588.top/gthsevzior.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.aibaodan.cn/gtllkjaxeu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinqigufen.top/gtxstpusgw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jianghu66.top/gtqfwllhix.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.havefunace.top/gtqtcnsqhe.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shanyushiyangkeji.top/gtlsdrgqrn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xuanzx.com/gtbvruxggy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.pycfn.com/gtalgkuspn.html

[D02] 追加元素到末尾
来源：http://hz.jyoumei.cn/gtljhrjjzs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yj202588.top/gtxbxeoqbe.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.nanxinkj.top/gtaxzzwoai.html

JS:   arr.push(4);
来源：http://hz.sufxvd.cn/gtvzmngjyc.html

TS:   arr.push(4);
来源：http://hz.ybcxt.top/gttwbmnzqx.html

Java: list.add(4);
来源：http://hz.aibaodan.cn/gtusgoedzg.html

Go:   arr = append(arr, 4)
来源：http://hz.dashuyun.cn/gtoepctsfm.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jianghu66.top/gtfskppufc.html

C#:   list.Add(4);
来源：http://hz.wangshuangyany.cn/gtpsucyeqi.html

[D03] 在指定位置插入元素
来源：http://hz.havefunace.top/gtndaclrra.html

Py:   arr.insert(0, 0)
来源：http://hz.jinyuanbaomall.cn/gtmddltain.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.havefunace.top/gtwxboowxv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sxryk.cn/gtzsyffgnj.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sxryk.cn/gtfumgykbr.html

Java: list.add(0, 0);
来源：http://hz.pycfn.com/gtatscanzh.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.kuanghao11.cn/gtnyssgycx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.9152youxi.cn/gtqtgcfpvf.html

C#:   list.Insert(0, 0);
来源：http://hz.zhengqikj.top/gtnbshpamx.html

[D04] 删除元素
来源：http://hz.vqdsnc.cn/gtivebakkj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.vqdsnc.cn/gtmwkjyfaa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.daria6918.cn/gtjnhgwbsi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xziqi.cn/gtcqeornts.html

TS:   arr.splice(0, 1);
来源：http://hz.guowangkeji.top/gtecqzgcxg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yvedp.cn/gthhcqlspd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.guowangkeji.top/gtsmbqqibi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.snrcjt.cn/gtzadncsei.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.feifeiyinyue.top/gteuxdkpwh.html

[D05] 访问与修改元素
来源：http://hz.gotoacloud.top/gtefrrmxqp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtmqdxuldl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xinyue.icu/gtbtserwpd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.0kj1m.cn/gttgfuvzxi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xuanzx.com/gtermpmicv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guannengcc.top/gtjvkkidiz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.daria6918.cn/gtgagaklzf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hongshengwenyu.top/gtslvpalic.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hammf.cn/gtlkjcukds.html

[D06] 数组长度
来源：http://hz.shangyingyoupin.top/gtudtbcmyn.html

Py:   len(arr)
来源：http://hz.bjfxy.top/gtljiwhyfr.html

PHP:  count($arr);
来源：http://hz.jianghu66.top/gtpcrrgdul.html

JS:   arr.length
来源：http://hz.feifeiyinyue.top/gtvnmfvkxw.html

TS:   arr.length
来源：http://hz.tianlin.xyz/gteselatej.html

Java: list.size();
来源：http://hz.ywan-chungtsiang.top/gtkktswrub.html

Go:   len(arr)
来源：http://hz.xuanzx.com/gtjlmhjqfg.html

Ruby: arr.length; arr.size
来源：http://hz.hongshengwenyu.top/gtytokqycl.html

C#:   list.Count;
来源：http://hz.cashguo.top/gtyatoayzd.html

[D07] 切片 / 取子数组
来源：http://hz.jinghuilouyu.cn/gtvgvascrb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yuanzhike.top/gtzcnbbpsv.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yonumen.top/gtaywlgiuw.html

JS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gtogfcmysf.html

TS:   arr.slice(1, 4);
来源：http://hz.shangyingyoupin.top/gtomyahqgk.html

Java: list.subList(1, 4);
来源：http://hz.ybcxt.top/gtxsrtyivb.html

Go:   arr[1:4]
来源：http://hz.hammf.cn/gtzsxymsdr.html

Ruby: arr[1, 3]
来源：http://hz.smart0.xyz/gthzwtrnhm.html

C#:   list.GetRange(1, 3);
来源：http://hz.jlsjyb.cn/gtqufyelbx.html

[D08] 合并两个数组
来源：http://hz.tian-w.cn/gtaiyvjmvx.html

Py:   a + b;  a.extend(b)
来源：http://hz.yuxming.cn/gtwlxhfjhj.html

PHP:  array_merge($a, $b);
来源：http://hz.sxryk.cn/gtpuouuupj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhengqikj.top/gthzurnxha.html

TS:   [...a, ...b];
来源：http://hz.jiagoushi.top/gtktiozdeq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.pengpengdd.cyou/gtvonicboi.html

Go:   append(a, b...)
来源：http://hz.yangfankeji.com/gtagqhvyla.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinqigufen.top/gtjrsnxryv.html

C#:   a.Concat(b).ToList()
来源：http://hz.haohaochexian.top/gtldaswzgf.html

[D09] 排序（升序）
来源：http://hz.wangshuangyany.cn/gtkoqnjadj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydjk.org.cn/gtjkkpmwnp.html

PHP:  sort($arr);
来源：http://hz.yvedp.cn/gtqstmtqbl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cqqwz.cn/gtojzvczsc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gotoacloud.top/gtqrdztqrv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gaohongyu789.top/gtkjwbkinj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.tanke756.top/gtjpyuejsx.html

Ruby: arr.sort
来源：http://hz.sweek.top/gtrnummfcv.html

C#:   list.Sort();
来源：http://hz.smart0.xyz/gtjxrlgong.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ivvv.top/gtrthuwuyg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hywenlv.cn/gtmldrmmwu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zdqjudy.top/gtxmfuodnp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gzhubu.top/gtmierthrv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hywenlv.cn/gtkxealtmp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.iojbl.cn/gtokpdugjg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.nwbrower.top/gtlawdntlx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj20258.top/gtnluuxdbd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinqigfzy.top/gtpkcidajx.html

[D11] 反转数组
来源：http://hz.yongpay.top/gtugddvrpa.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.quarkkingdee.top/gtbjjjjpfp.html

PHP:  array_reverse($arr);
来源：http://hz.chenlongwang.top/gtgtffhpph.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tian-w.cn/gtseptraiz.html

TS:   [...arr].reverse();
来源：http://hz.gzhubu.top/gtkmnwauor.html

Java: Collections.reverse(list);
来源：http://hz.mhx1999.top/gtptbrjaqm.html

Go:   slices.Reverse(arr)
来源：http://hz.gotoacloud.top/gtcgznopyh.html

Ruby: arr.reverse
来源：http://hz.jyoumei.cn/gtptbkduhl.html

C#:   list.Reverse();
来源：http://hz.daria6918.cn/gtzielokic.html

[D12] 查找元素下标
来源：http://hz.chenzaomai.com/gtylehoevj.html

Py:   arr.index(x);  x in arr
来源：http://hz.hysaishi.cn/gtxrukmagz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenzaomai.com/gtsqhyzlxt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhongyouzk.top/gtccrbxsxb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.9152youxi.cn/gtreamvsra.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shzxlz.cn/gtpnfagang.html

Go:   slices.Index(arr, x)
来源：http://hz.gzhubu.top/gtynbrbmmr.html

Ruby: arr.index(x)
来源：http://hz.yuanzhike.top/gtdhkdxpvp.html

C#:   list.IndexOf(x);
来源：http://hz.yueranfly.top/gtynuzmusc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ivvv.top/gtdbtjevpf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xinyue.icu/gtgplvfqgx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.tianlin.xyz/gtwtovfvbh.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zycfv.cn/gtsjcgrlbg.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ehwqpu.com/gtmmjnnqiv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhengqikj.top/gtwnfmirog.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shanyushiyangtech.top/gtjdycmkeq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.wangdashe.top/gtoxqmfjlq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tianlin.xyz/gtqqnhdiru.html

[D14] 映射转换（每个元素变形）
来源：http://hz.guowangkeji.top/gtnyurbztj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tianlin.xyz/gttkjvgkiw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shanyushiyangtech.top/gtfjvrhhgr.html

JS:   arr.map(x => x * 2)
来源：http://hz.hnxiangtu.top/gtxjdwwbwm.html

TS:   arr.map(x => x * 2)
来源：http://hz.yj202588.top/gttocegaun.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gaohongyu789.top/gtfljozczz.html

Go:   // 手写循环
来源：http://hz.xuanzx.com/gtahurwlim.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xuetiantiany.cn/gtwsoonfcu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhaomingkeji.xyz/gtxlhygzbw.html

[D15] 去重
来源：http://hz.yueranfly.top/gtevdvvbyc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinqigufen.top/gteikucoap.html

PHP:  array_unique($arr);
来源：http://hz.yongpay.top/gtfganeofy.html

JS:   [...new Set(arr)]
来源：http://hz.yuanzhike.top/gtjkmxoatu.html

TS:   [...new Set(arr)]
来源：http://hz.cheryme.top/gtjkovhfzv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ydjk.org.cn/gtyzkozdsu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shangyingyoupin.top/gtaabyxixt.html

Ruby: arr.uniq
来源：http://hz.cheryme.top/gttaauvlpa.html

C#:   list.Distinct().ToList()
来源：http://hz.cheryme.top/gtdawqirqz.html

[D16] 求和与平均值
来源：http://hz.andypj.xyz/gtpynxuwxn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.pycfn.com/gtvmpwfada.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhaomingkeji.xyz/gtzbjzcxil.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.kuanghao11.cn/gtrnqzoqao.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jianghu66.top/gtnhcfzfkw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.birdmap.top/gttdiumisq.html

Go:   // 手写循环累加
来源：http://hz.jiagoushi.top/gtolfsbacw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zycfv.cn/gtgmnkzejt.html

C#:   list.Sum();  list.Average()
来源：http://hz.xuetiantiany.cn/gtatrwfsdr.html

[D17] 最大值与最小值
来源：http://hz.daria6918.cn/gthrmnbxxb.html

Py:   max(arr);  min(arr)
来源：http://hz.redwolf501.top/gtvositbkd.html

PHP:  max($arr);  min($arr);
来源：http://hz.jqgufenzy.top/gtuwmibptk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xuanzx.com/gtfjjtzwfh.html

TS:   Math.max(...arr);
来源：http://hz.chenzaomai.com/gtljghbmhm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yueranfly.top/gtihmdcupm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jlsjyb.cn/gtulnevhcw.html

Ruby: arr.max;  arr.min
来源：http://hz.shangyingyoupin.top/gtcjcbsrhs.html

C#:   list.Max();  list.Min()
来源：http://hz.bjfxy.top/gtegdionsb.html

[D18] 扁平化嵌套数组
来源：http://hz.yanxiufei.cn/gtxdhdrtcb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.9152youxi.cn/gtgssbymvf.html

PHP:  array_merge(...$nested);
来源：http://hz.zhiwuduotai.top/gtaumvfhce.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hnxiangtu.top/gtjjadjkwf.html

TS:   nested.flat();
来源：http://hz.zhiwuduotai.top/gtniqtnzuu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.iojbl.cn/gtjsdbmwlo.html

Go:   // 手写双层循环
来源：http://hz.andypj.xyz/gtjylbvlkj.html

Ruby: nested.flatten
来源：http://hz.jinyuanbaomall.cn/gtfrckjirq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pycfn.com/gtluinnzzs.html

[D19] 按字段分组
来源：http://hz.nwbrower.top/gthwhxtzfp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cdnleiting.top/gthsrqxxbh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhiwuduotai.top/gthnwkwxho.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.smart0.xyz/gtojwvuahk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xziqi.cn/gtcwjjcmsf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yj20258.top/gtlnuatgzo.html

Go:   // 手写 map[string][]T
来源：http://hz.sweek.top/gtcvilxjds.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.haohaochexian.top/gtamvrmham.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.bjfxy.top/gtlyqrgepx.html

[D20] 统计每个元素出现次数
来源：http://hz.sweek.top/gtvvbfspim.html

Py:   Counter(arr)
来源：http://hz.cashguo.top/gtglceumtn.html

PHP:  array_count_values($arr);
来源：http://hz.wangdashe.top/gtmtrxbmtx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pengpengdd.cyou/gtzkubqchx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cdnleiting.top/gtcotxhqtu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sysykeji.top/gtljjuztrl.html

Go:   // 手写 map[T]int
来源：http://hz.jyoumei.cn/gtyiyxdhet.html

Ruby: arr.tally
来源：http://hz.0kj1m.cn/gtuedijmov.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hnxiangtu.top/gtrgmgkhtp.html

[D21] 判断是否包含某元素
来源：http://hz.xingfuxueyuan.xyz/gtkyiaeage.html

Py:   x in arr
来源：http://hz.yj202588.top/gtswojotmw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yanxiufei.cn/gtptuzfadb.html

JS:   arr.includes(x)
来源：http://hz.kuanghao11.cn/gtrcadmcxg.html

TS:   arr.includes(x)
来源：http://hz.yj202588.top/gtyukjndle.html

Java: list.contains(x)
来源：http://hz.nanxinkj.top/gtjzigotgh.html

Go:   slices.Contains(arr, x)
来源：http://hz.meibo888.top/gtejhjonyp.html

Ruby: arr.include?(x)
来源：http://hz.c1oappe.top/gtmfcukaow.html

C#:   list.Contains(x)
来源：http://hz.xziqi.cn/gtkhvsjsjo.html

[D22] 复制数组（避免共享引用）
来源：http://hz.vqdsnc.cn/gtowznwqel.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhixingplan.top/gtcavwtiml.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinyuanbaomall.cn/gtnrklqmvl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.meibo888.top/gtcktxastt.html

TS:   [...arr];
来源：http://hz.bjfxy.top/gtekhqbbam.html

Java: new ArrayList<>(list);
来源：http://hz.pengpengdd.cyou/gtchigedge.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hongshengwenyu.top/gtjqlcwblj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sweek.top/gtruiayosu.html

C#:   new List<int>(list);
来源：http://hz.xuetiantiany.cn/gtitqlfspk.html

[D23] reduce 累积计算
来源：http://hz.guannengcc.top/gtkihokzlv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhengqikj.top/gtaypyjdzv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cheryme.top/gtxddjihyk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jyoumei.cn/gtfoqoevnr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jyoumei.cn/gtckxdtxuf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.daxiang520.top/gtfvwfyulz.html

Go:   // 手写循环
来源：http://hz.daria6918.cn/gtahbzjgsm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.fzhhl.top/gtgcnvhxal.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.guowangkeji.top/gtmxyfysdo.html

[D24] 字典 / Map 基本操作
来源：http://hz.sxryk.cn/gtbmzgwiqi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ehwqpu.com/gtsknavbiy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.bjfxy.top/gtwtwfcpvn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jiagoushi.top/gtrnldpkil.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cheryme.top/gtkwmuxksw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.meibo888.top/gtaunikjna.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.meibo888.top/gtleeborcg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhoulong.xyz/gtyzgfgacs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cqqwz.cn/gtmrnqtfld.html

[D25] Set 集合去重与交并差
来源：http://hz.cucudq.cn/gtdjotvkrm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.smart0.xyz/gtircxlsjt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.tanke756.top/gtfcvfcljv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhengqikj.top/gtdrfhcnxd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sweek.top/gtgqxwzdzd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cashguo.top/gtylfzxnnp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jlsjyb.cn/gtmmwnnuqa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ehwqpu.com/gtcassshsp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.tian-w.cn/gtennsgobz.html

[D26] 数组转字符串
来源：http://hz.jyoumei.cn/gtghdzlgle.html

Py:   ", ".join(map(str, arr))
来源：http://hz.daxiang520.top/gtgfurfhww.html

PHP:  implode(", ", $arr);
来源：http://hz.daria6918.cn/gtvmhoubbf.html

JS:   arr.join(", ")
来源：http://hz.havefunace.top/gtfrmzdbuf.html

TS:   arr.join(", ")
来源：http://hz.xuetiantiany.cn/gtijyxqqfp.html

Java: String.join(", ", list)
来源：http://hz.ivvv.top/gtreilurkn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.redwolf501.top/gtyyhtndek.html

Ruby: arr.join(", ")
来源：http://hz.guannengcc.top/gtxlmqhras.html

C#:   string.Join(", ", list)
来源：http://hz.vqdsnc.cn/gttjlrilfh.html

================================================================================
来源：http://hz.tanke756.top/gtzefdxtuc.html

E. 字符串处理
来源：http://hz.feifeiyinyue.top/gtglkuexjh.html

================================================================================
来源：http://hz.meibo888.top/gtpazvfphv.html

[E01] 拼接字符串
来源：http://hz.tianlin.xyz/gtzzdeovfk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.pycfn.com/gtxzoywlhk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cucudq.cn/gtgfggqftl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.mhx1999.top/gtexekxjml.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnxiangtu.top/gtksowblgr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.dashuyun.cn/gtcrcujqaa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xuetiantiany.cn/gtuzsvrzgs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.pycfn.com/gtnisnuagb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yangfankeji.com/gtrlrasxrq.html

[E02] 重复字符串
来源：http://hz.shuidangran.top/gtroovicot.html

Py:   "ab" * 3
来源：http://hz.zdqjudy.top/gtpidqagjv.html

PHP:  str_repeat("ab", 3);
来源：http://hz.vqdsnc.cn/gtzagdirbo.html

JS:   "ab".repeat(3)
来源：http://hz.gaohongyu789.top/gtqgepshax.html

TS:   "ab".repeat(3)
来源：http://hz.shzxlz.cn/gtrxlpvzxl.html

Java: "ab".repeat(3)
来源：http://hz.hnqzz.top/gtealdasdd.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.c1oappe.top/gtyqaefmmr.html

Ruby: "ab" * 3
来源：http://hz.0kj1m.cn/gtlvrygedz.html


<!-- 参考信息 -->