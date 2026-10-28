代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://hz.vqdsnc.cn/gtnrubswyp.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xylfe.cn/gtpwywjuar.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yueranfly.top/gtactjwaqz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cqqwz.cn/gtpwpdyasl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.svipenyu.cn/gtcmiciusk.html

Ruby: -> { puts "run" }.call
来源：http://hz.smart0.xyz/gttpbxqrft.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.kuanghao11.cn/gtipkvzcju.html

[C13] 类型声明 / 类型注解
来源：http://hz.52xcode.cn/gtanurtuah.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinqigufen.top/gtlzywnrbf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenzaomai.com/gtjhsyrrwb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cucudq.cn/gtlcmsqypz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.aibaodan.cn/gtmjtbplaz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtdkezniha.html

Go:   func add(a, b int) int
来源：http://hz.fengsongda.top/gtzdyxmcrf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jlsjyb.cn/gtsphuznul.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.0kj1m.cn/gtkkqxfxgd.html

[C14] 泛型函数
来源：http://hz.guowangkeji.top/gtvnrdiztt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jyoumei.cn/gtwkgjppru.html

PHP:  // 无泛型
来源：http://hz.52xcode.cn/gttckjruec.html

JS:   // 无泛型
来源：http://hz.shuidangran.top/gtdyvemhli.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.snrcjt.cn/gtwovvyqio.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.vqdsnc.cn/gtxgpyhtaz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.smart0.xyz/gtnaucpldv.html

Ruby: # 无泛型
来源：http://hz.xingfuxueyuan.xyz/gtaudaexcs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.wangshuangyany.cn/gtgfgfccfj.html

[C15] 解构 / 展开参数
来源：http://hz.gotoacloud.top/gtojymynii.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinghuilouyu.cn/gteeugaznr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yueranfly.top/gtzztistwj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xinyue.icu/gtmzlfjsfa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ppjwa.cn/gtuzzdlhba.html

Java: // 无解构
来源：http://hz.aizwys.cn/gtcalzcxrq.html

Go:   // 无解构
来源：http://hz.tian-w.cn/gtfuplemtx.html

Ruby: a, b = pair
来源：http://hz.bjfxy.top/gtgttersyo.html

C#:   var (a, b) = pair;
来源：http://hz.xuetiantiany.cn/gtihdujzkr.html

[C16] 函数 / 方法重载
来源：http://hz.zhoulong.xyz/gtfjspykbd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yongpay.top/gtcmdkbnvl.html

PHP:  // 无重载
来源：http://hz.xziqi.cn/gtbjwqlvtv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yangfankeji.com/gttfjrqgho.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhaomingkeji.xyz/gtmpdxdbcm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jianghu66.top/gtmadbqiri.html

Go:   // 无重载：用不同函数名
来源：http://hz.xinyue.icu/gtdxarldrc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.quarkkingdee.top/gtjvnrbchw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cqqwz.cn/gtvseqneoe.html

================================================================================
来源：http://hz.xylfe.cn/gtknfidede.html

D. 数组 / 列表 / 集合
来源：http://hz.iojbl.cn/gtrhaqothk.html

================================================================================
来源：http://hz.bjfxy.top/gtaxyypgaj.html

[D01] 创建数组 / 列表
来源：http://hz.fzhhl.top/gtamyjwcac.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.wangshuangyany.cn/gtyzeavpms.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.wangdashe.top/gtckhyrqfb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.haohaochexian.top/gtkqosvspz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hnxiangtu.top/gtswjchdtu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhixingplan.top/gtblmxmjnz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hysaishi.cn/gtspnsqzqv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ybcxt.top/gtarvmjlmm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hnqzz.top/gtsziwtaku.html

[D02] 追加元素到末尾
来源：http://hz.gaohongyu789.top/gthyjerlfa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.redwolf501.top/gturupbxvx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xingfuxueyuan.xyz/gtpwqnretq.html

JS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gtgfzcjriw.html

TS:   arr.push(4);
来源：http://hz.jqgufenzy.top/gtcepbklac.html

Java: list.add(4);
来源：http://hz.yangfankeji.com/gteiaiumjo.html

Go:   arr = append(arr, 4)
来源：http://hz.zhongyouzk.top/gtnhmybpjw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhixingplan.top/gtaiqcxscr.html

C#:   list.Add(4);
来源：http://hz.shangyingyoupin.top/gtksmbwkxv.html

[D03] 在指定位置插入元素
来源：http://hz.hnxiangtu.top/gtlkzbphrp.html

Py:   arr.insert(0, 0)
来源：http://hz.sxryk.cn/gtxvxgujbm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xinyue.icu/gtgqftlosf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gotoacloud.top/gtgpxyzrav.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.kuanghao11.cn/gtyjvswavf.html

Java: list.add(0, 0);
来源：http://hz.gotoacloud.top/gtmgdkjevt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenzaomai.com/gtlgjxbmir.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.feifeiyinyue.top/gtjbgrmlcb.html

C#:   list.Insert(0, 0);
来源：http://hz.yuxming.cn/gtwcwopkxs.html

[D04] 删除元素
来源：http://hz.yongpay.top/gtecivujbs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.gogol.net.cn/gthktjhqgc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.nanxuanxn.top/gtcknbjnvu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.birdmap.top/gtvrhbctkb.html

TS:   arr.splice(0, 1);
来源：http://hz.haohaochexian.top/gttvlseiun.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cqqwz.cn/gtmygwpmdr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.havefunace.top/gttegvmgzq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.mhx1999.top/gtkzhitxao.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhoulong.xyz/gtoupldtoq.html

[D05] 访问与修改元素
来源：http://hz.yuanzhike.top/gtrlmdckqx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.vqdsnc.cn/gtoeoaezgw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhongyouzk.top/gtjdhznmqb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gotoacloud.top/gtmnyrabyy.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gzhubu.top/gtdhzaalcg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinyuanbaomall.cn/gthvcnhavd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.nanxuanxn.top/gtwoqleflg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ehwqpu.com/gtcybblbln.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.daxiang520.top/gtzoeoqwhp.html

[D06] 数组长度
来源：http://hz.pengpengdd.cyou/gtmfylqwyi.html

Py:   len(arr)
来源：http://hz.hammf.cn/gtfxcqydaj.html

PHP:  count($arr);
来源：http://hz.hammf.cn/gtmfgnnbqu.html

JS:   arr.length
来源：http://hz.hysaishi.cn/gtpoqlwlnm.html

TS:   arr.length
来源：http://hz.wangshuangyany.cn/gtrmwmmcqh.html

Java: list.size();
来源：http://hz.yvedp.cn/gtkkruliuo.html

Go:   len(arr)
来源：http://hz.jiagoushi.top/gtudaaevmg.html

Ruby: arr.length; arr.size
来源：http://hz.jinyuanbaomall.cn/gtgieopdfj.html

C#:   list.Count;
来源：http://hz.yanxiufei.cn/gtfcqjgimp.html

[D07] 切片 / 取子数组
来源：http://hz.ehwqpu.com/gtoqexdidg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.feifeiyinyue.top/gtszmlhgnq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.c1oappe.top/gtakqcfxhl.html

JS:   arr.slice(1, 4);
来源：http://hz.jiagoushi.top/gtqwtbomla.html

TS:   arr.slice(1, 4);
来源：http://hz.yongpay.top/gtzxrlghlg.html

Java: list.subList(1, 4);
来源：http://hz.andypj.xyz/gtgjpcvxzd.html

Go:   arr[1:4]
来源：http://hz.c1oappe.top/gtmxprhhjx.html

Ruby: arr[1, 3]
来源：http://hz.ppjwa.cn/gtcgvjdqnf.html

C#:   list.GetRange(1, 3);
来源：http://hz.andypj.xyz/gtphvoceqc.html

[D08] 合并两个数组
来源：http://hz.chenzaomai.com/gtauelkehn.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenlongwang.top/gtxfanhkzo.html

PHP:  array_merge($a, $b);
来源：http://hz.cheryme.top/gtoctxpolj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xuanzx.com/gtrptsnlbo.html

TS:   [...a, ...b];
来源：http://hz.sxryk.cn/gtejbzgkfv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xuetiantiany.cn/gtjdsalseh.html

Go:   append(a, b...)
来源：http://hz.jinqigfzy.top/gtzvnvpxsl.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sweek.top/gtqyprltxe.html

C#:   a.Concat(b).ToList()
来源：http://hz.aibaodan.cn/gtapcwxjck.html

[D09] 排序（升序）
来源：http://hz.gzhubu.top/gtnwokehvp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.havefunace.top/gtaclfqhsm.html

PHP:  sort($arr);
来源：http://hz.xuanzx.com/gtbcwrxfit.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.chenzaomai.com/gtgxesghiz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.bjfxy.top/gtbphqjmfq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ppjwa.cn/gtlmsbknok.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nanxinkj.top/gtbqggyrwz.html

Ruby: arr.sort
来源：http://hz.jinghuilouyu.cn/gteetjgthl.html

C#:   list.Sort();
来源：http://hz.wangshuangyany.cn/gtffitxjfh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gogol.net.cn/gtpjzoamel.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sufxvd.cn/gtseqjhbww.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenzaomai.com/gtsmjnkulj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgufenzy.top/gtomhtepnf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gaohongyu789.top/gtrpsrmqeq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cdnleiting.top/gtwfnkplhe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.chenlongwang.top/gtilpiqdde.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhaomingkeji.xyz/gtgnkujsru.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhixingplan.top/gtjfpfltqn.html

[D11] 反转数组
来源：http://hz.chenjidiqi.icu/gtqbmyedra.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.316326.xyz/gtugnyzsyh.html

PHP:  array_reverse($arr);
来源：http://hz.iojbl.cn/gtkezfkyss.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.52xcode.cn/gtsbcvclid.html

TS:   [...arr].reverse();
来源：http://hz.jqgfzy.top/gtkcoajhvf.html

Java: Collections.reverse(list);
来源：http://hz.jinqigfzy.top/gtpanykimx.html

Go:   slices.Reverse(arr)
来源：http://hz.svipenyu.cn/gtkahailar.html

Ruby: arr.reverse
来源：http://hz.shanyushiyangkeji.top/gtljrjwvdw.html

C#:   list.Reverse();
来源：http://hz.birdmap.top/gtpflcbexi.html

[D12] 查找元素下标
来源：http://hz.zhoulong.xyz/gtrsutyiem.html

Py:   arr.index(x);  x in arr
来源：http://hz.sweek.top/gtepginkyq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.smart0.xyz/gtlvktcqli.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gogol.net.cn/gtyojrhfoy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pycfn.com/gtfkwanoto.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.pengpengdd.cyou/gtzxnltdlg.html

Go:   slices.Index(arr, x)
来源：http://hz.hnqzz.top/gtrinfzulf.html

Ruby: arr.index(x)
来源：http://hz.hysaishi.cn/gtnuzucctb.html

C#:   list.IndexOf(x);
来源：http://hz.sweek.top/gtbjlxioxl.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yangfankeji.com/gtbfvkwcvt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.svipenyu.cn/gtivaxsdma.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ydjk.org.cn/gtwzqrsizs.html

JS:   arr.filter(x => x > 3)
来源：http://hz.mhx1999.top/gtgjbbgvcs.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangkeji.top/gtmxhuxbdq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ppjwa.cn/gtfbalyoyn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.feifeiyinyue.top/gttivpwwlx.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xylfe.cn/gtdrxhjghc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinghuilouyu.cn/gtvsndsrkc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hywenlv.cn/gtvfykhcei.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xinyue.icu/gtojfppgcm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.9152youxi.cn/gtphcbqide.html

JS:   arr.map(x => x * 2)
来源：http://hz.cdnleiting.top/gtvvhqfxrw.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhongyouzk.top/gtzbdaxmqz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jqgfzy.top/gttqokfbif.html

Go:   // 手写循环
来源：http://hz.bjfxy.top/gtztuzajgg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cqqwz.cn/gtjjppqqzl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xinyue.icu/gtffyrrdrl.html

[D15] 去重
来源：http://hz.yanxiufei.cn/gtnjkdaqlb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.316326.xyz/gtjbxstabm.html

PHP:  array_unique($arr);
来源：http://hz.hywenlv.cn/gtwxqbecvf.html

JS:   [...new Set(arr)]
来源：http://hz.gaohongyu789.top/gtpmohtrdn.html

TS:   [...new Set(arr)]
来源：http://hz.fzhhl.top/gtfyqypmhx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cucudq.cn/gtbjhocalh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ybcxt.top/gtkxzeqmye.html

Ruby: arr.uniq
来源：http://hz.chenlongwang.top/gtangasqzc.html

C#:   list.Distinct().ToList()
来源：http://hz.zhaomingkeji.xyz/gtogwpinwo.html

[D16] 求和与平均值
来源：http://hz.hongshengwenyu.top/gtcffsvjup.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.fengsongda.top/gtgkbyyzjp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ppjwa.cn/gtqyphqqwg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtyfgtxoiw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtdkdqupvx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinqigfzy.top/gtornjsvll.html

Go:   // 手写循环累加
来源：http://hz.shzxlz.cn/gtglfbitkk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ivvv.top/gtpxtdmxoy.html

C#:   list.Sum();  list.Average()
来源：http://hz.gogol.net.cn/gtkkwdjilm.html

[D17] 最大值与最小值
来源：http://hz.yvedp.cn/gtsumbsnba.html

Py:   max(arr);  min(arr)
来源：http://hz.hfpthk.cn/gtvproexuo.html

PHP:  max($arr);  min($arr);
来源：http://hz.svipenyu.cn/gtfcoylzxo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.fzhhl.top/gtnrgqcgbi.html

TS:   Math.max(...arr);
来源：http://hz.birdmap.top/gtfpftwnkb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hywenlv.cn/gtedmselyo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.aibaodan.cn/gtirpplyhm.html

Ruby: arr.max;  arr.min
来源：http://hz.nwbrower.top/gtysvielqf.html

C#:   list.Max();  list.Min()
来源：http://hz.quarkkingdee.top/gttmmkzkho.html

[D18] 扁平化嵌套数组
来源：http://hz.daxiang520.top/gtwtbxxxnj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenlongwang.top/gtwmluwzko.html

PHP:  array_merge(...$nested);
来源：http://hz.c1oappe.top/gtehxfpwuk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shuidangran.top/gtcrchtlau.html

TS:   nested.flat();
来源：http://hz.dianchejie.cn/gtgoeqxflv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhijiandao.cn/gtxwzrqinj.html

Go:   // 手写双层循环
来源：http://hz.snrcjt.cn/gtqslkcizg.html

Ruby: nested.flatten
来源：http://hz.ydzc1.top/gtnnnfmzrg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.daria6918.cn/gtxobnxjnm.html

[D19] 按字段分组
来源：http://hz.shuidangran.top/gtheysfsqy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hysaishi.cn/gtnbaapnji.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj202588.top/gtkizecxbu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hywenlv.cn/gtkgwywfig.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.wangshuangyany.cn/gtxrcrtkgj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.andypj.xyz/gtebirbypd.html

Go:   // 手写 map[string][]T
来源：http://hz.yuxming.cn/gtnycwjapq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cdnleiting.top/gtzrpbdwqq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jiagoushi.top/gtfyiqtgqx.html

[D20] 统计每个元素出现次数
来源：http://hz.pengpengdd.cyou/gtjojneolx.html

Py:   Counter(arr)
来源：http://hz.bjfxy.top/gtirpnfkgk.html

PHP:  array_count_values($arr);
来源：http://hz.c1oappe.top/gteunqhvku.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jlsjyb.cn/gtxhcisscq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hysaishi.cn/gtkbdukxhu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tanke756.top/gtoujprjht.html

Go:   // 手写 map[T]int
来源：http://hz.yj202588.top/gtpebimcdu.html

Ruby: arr.tally
来源：http://hz.feifeiyinyue.top/gtrdrrvnsq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj20258888.top/gtiyjnkzwx.html

[D21] 判断是否包含某元素
来源：http://hz.xuanzx.com/gtpfegynnx.html

Py:   x in arr
来源：http://hz.sxryk.cn/gtfoisfpbe.html

PHP:  in_array($x, $arr, true);
来源：http://hz.kuanghao11.cn/gtjqivudgs.html

JS:   arr.includes(x)
来源：http://hz.aizwys.cn/gtvnuyppys.html

TS:   arr.includes(x)
来源：http://hz.quarkkingdee.top/gtmodjkzcx.html

Java: list.contains(x)
来源：http://hz.xylfe.cn/gtytmciyfw.html

Go:   slices.Contains(arr, x)
来源：http://hz.hnxiangtu.top/gtkhwlczxx.html

Ruby: arr.include?(x)
来源：http://hz.tanke756.top/gtppghzhld.html

C#:   list.Contains(x)
来源：http://hz.316326.xyz/gtccqfzjzn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.wangdashe.top/gtwdbpzoej.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.meibo888.top/gtikhcsqdy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daxiang520.top/gtjvlazgdd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yangfankeji.com/gteuoudiqz.html

TS:   [...arr];
来源：http://hz.svipenyu.cn/gtdazqtpmb.html

Java: new ArrayList<>(list);
来源：http://hz.yanxiufei.cn/gtcfdqfcdp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinghuilouyu.cn/gthlglgrzp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.feifeiyinyue.top/gtuzdawcre.html

C#:   new List<int>(list);
来源：http://hz.kuanghao11.cn/gtwfntwxzj.html

[D23] reduce 累积计算
来源：http://hz.zhixingplan.top/gthrbhpdwp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.mhx1999.top/gtysvmydwm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xylfe.cn/gtktjsvkeq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhixingplan.top/gtvvhigeuw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.c1oappe.top/gtcyacsgxu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jqgufenzy.top/gtqmiwnfgq.html

Go:   // 手写循环
来源：http://hz.yangfankeji.com/gtqffmlhco.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.dianchejie.cn/gtecvxiydz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jqgfzy.top/gtbshcoffz.html

[D24] 字典 / Map 基本操作
来源：http://hz.pengpengdd.cyou/gtpcxftiss.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jlsjyb.cn/gtwzskgags.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.nwbrower.top/gthiruhgwq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hongshengwenyu.top/gttrcraucg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yonumen.top/gtskwyczbu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.iojbl.cn/gtvhtiwnuz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shzxlz.cn/gtotsnbzhe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sysykeji.top/gtzfvdlbig.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.aibaodan.cn/gtsdjskzqx.html

[D25] Set 集合去重与交并差
来源：http://hz.yonumen.top/gtwfaqdswb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhijiandao.cn/gtdhcxixjr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.daxiang520.top/gtxvqpevws.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ivvv.top/gtanqegxbg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gzhubu.top/gtbbhaxoki.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinghuilouyu.cn/gtsamtnjpz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xuetiantiany.cn/gtpkddhhqn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yj202588.top/gtbvbpquwi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.9152youxi.cn/gttwxzyhge.html

[D26] 数组转字符串
来源：http://hz.ywan-chungtsiang.top/gtwnagcaxg.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinqigufen.top/gtukguqhes.html

PHP:  implode(", ", $arr);
来源：http://hz.jiagoushi.top/gtsvmmjroz.html

JS:   arr.join(", ")
来源：http://hz.jqgufenzy.top/gtfwiyxmbd.html

TS:   arr.join(", ")
来源：http://hz.jinqigufen.top/gttqjiirnk.html

Java: String.join(", ", list)
来源：http://hz.tianlin.xyz/gtaqgmtykd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hongshengwenyu.top/gtjduoqivr.html

Ruby: arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gttjoffoez.html

C#:   string.Join(", ", list)
来源：http://hz.hywenlv.cn/gtbwboutxw.html

================================================================================
来源：http://hz.havefunace.top/gtmswwfkyp.html

E. 字符串处理
来源：http://hz.andypj.xyz/gtugzulqne.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtrcgjbfzy.html

[E01] 拼接字符串
来源：http://hz.yj202588.top/gtoghdzzye.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhiwuduotai.top/gtcthvrhci.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xingfuxueyuan.xyz/gtggssymcm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shanyushiyangtech.top/gtbdyaysay.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.dashuyun.cn/gthvbsijyr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.kuanghao11.cn/gtwgizmmvu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.9152youxi.cn/gtrlbrpiby.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jqgfzy.top/gtrpnivbea.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.nwbrower.top/gtuuosqkib.html

[E02] 重复字符串
来源：http://hz.shzxlz.cn/gtjmreouta.html

Py:   "ab" * 3
来源：http://hz.gotoacloud.top/gtlcbkbdzm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.pengpengdd.cyou/gtircksnra.html

JS:   "ab".repeat(3)
来源：http://hz.fzhhl.top/gtkpnwnege.html

TS:   "ab".repeat(3)
来源：http://hz.guannengcc.top/gtqoslzuhe.html

Java: "ab".repeat(3)
来源：http://hz.xingfuxueyuan.xyz/gtkxxjvfqo.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xinyue.icu/gtlvqjzikt.html

Ruby: "ab" * 3
来源：http://hz.sxryk.cn/gtzlofhwza.html


<!-- 参考信息 -->