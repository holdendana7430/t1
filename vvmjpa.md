代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://hz.quarkkingdee.top/gtrlwjwvyj.html

C#:   using System.Text;
来源：http://hz.yvedp.cn/gtmrbaxfsh.html

[C12] 立即执行函数 IIFE
来源：http://hz.ywan-chungtsiang.top/gttujnzmfs.html

Py:   (lambda: print("run"))()
来源：http://hz.c1oappe.top/gtezljdbiv.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nanxuanxn.top/gtcnbwomej.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xinyue.icu/gtvbuqojve.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xuetiantiany.cn/gtuwmumlmg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ivvv.top/gtxdbgzszo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xylfe.cn/gtpiqiiqps.html

Ruby: -> { puts "run" }.call
来源：http://hz.wangshuangyany.cn/gtdltszijm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ppjwa.cn/gtijbwhhsi.html

[C13] 类型声明 / 类型注解
来源：http://hz.yvedp.cn/gtrsegtojj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cheryme.top/gtbketwcpe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yueranfly.top/gthupybulp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.dashuyun.cn/gtaizobynb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shuidangran.top/gtztbfglqt.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.c1oappe.top/gtmfsgtvmm.html

Go:   func add(a, b int) int
来源：http://hz.xuetiantiany.cn/gtvwmulcri.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ydzc1.top/gtnelujagy.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jianghu66.top/gtrrkntvji.html

[C14] 泛型函数
来源：http://hz.hnxiangtu.top/gtslilkgyp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ywan-chungtsiang.top/gtyubcypze.html

PHP:  // 无泛型
来源：http://hz.shangyingyoupin.top/gthlxcpnmi.html

JS:   // 无泛型
来源：http://hz.ppjwa.cn/gtafqdmwxx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guowangkeji.top/gttkbzwtfi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hnqzz.top/gtgzoldetv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.tianlin.xyz/gtrvrfcink.html

Ruby: # 无泛型
来源：http://hz.gzhubu.top/gtpgpmawma.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.wangshuangyany.cn/gtxiossqxz.html

[C15] 解构 / 展开参数
来源：http://hz.xinyue.icu/gtujmbbpry.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.smart0.xyz/gthnkxmdqy.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cucudq.cn/gtxtlyxoci.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.tian-w.cn/gthmgdceda.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.smart0.xyz/gthavqjcoi.html

Java: // 无解构
来源：http://hz.9152youxi.cn/gtekecdmdf.html

Go:   // 无解构
来源：http://hz.cashguo.top/gtvjuietbc.html

Ruby: a, b = pair
来源：http://hz.cdnleiting.top/gtjlyflowt.html

C#:   var (a, b) = pair;
来源：http://hz.316326.xyz/gttnmgfgmz.html

[C16] 函数 / 方法重载
来源：http://hz.yangfankeji.com/gtavwnlxmm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yuanzhike.top/gtlgjdtywt.html

PHP:  // 无重载
来源：http://hz.dashuyun.cn/gtqtzjmycw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yangfankeji.com/gtldaezmvr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hnqzz.top/gtgxtmnnip.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.gotoacloud.top/gtkmwbghtu.html

Go:   // 无重载：用不同函数名
来源：http://hz.kuanghao11.cn/gtrvqkuznd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hysaishi.cn/gtfguhwuto.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zdqjudy.top/gtifphdwer.html

================================================================================
来源：http://hz.mhx1999.top/gtdnxsllyf.html

D. 数组 / 列表 / 集合
来源：http://hz.fengsongda.top/gtxtxdgsum.html

================================================================================
来源：http://hz.ybcxt.top/gtvmszrapk.html

[D01] 创建数组 / 列表
来源：http://hz.yonumen.top/gtweqtnkga.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sysykeji.top/gtimyuuqbj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ehwqpu.com/gtemqwcoup.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cdnleiting.top/gtyvkbcgln.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.dianchejie.cn/gtveqiipkm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.sxryk.cn/gtmongthva.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhijiandao.cn/gtcwaenpku.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhengqikj.top/gtjjsvuswa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xingfuxueyuan.xyz/gtuuayablv.html

[D02] 追加元素到末尾
来源：http://hz.yanxiufei.cn/gtchxajwig.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shangyingyoupin.top/gthfmvsqlf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.daxiang520.top/gtimsddgwd.html

JS:   arr.push(4);
来源：http://hz.c1oappe.top/gttnwauurm.html

TS:   arr.push(4);
来源：http://hz.nanxinkj.top/gtkhktzhxt.html

Java: list.add(4);
来源：http://hz.fzhhl.top/gtsbfmnlfh.html

Go:   arr = append(arr, 4)
来源：http://hz.wangshuangyany.cn/gtreciysee.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.bjfxy.top/gtktirkqmk.html

C#:   list.Add(4);
来源：http://hz.birdmap.top/gtonimwuhy.html

[D03] 在指定位置插入元素
来源：http://hz.shanyushiyangtech.top/gtskbjeihj.html

Py:   arr.insert(0, 0)
来源：http://hz.yueranfly.top/gtkrtfzmps.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.9152youxi.cn/gtluasvvmh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.svipenyu.cn/gtvrdhpqca.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sxryk.cn/gtbscbxzkx.html

Java: list.add(0, 0);
来源：http://hz.haohaochexian.top/gtgahsxefe.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.feifeiyinyue.top/gtutcchesm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.feifeiyinyue.top/gtofogseag.html

C#:   list.Insert(0, 0);
来源：http://hz.zhijiandao.cn/gtizrejqci.html

[D04] 删除元素
来源：http://hz.pengpengdd.cyou/gtviqunsva.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenzaomai.com/gtvgvvbmkn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hfpthk.cn/gtlzthlmtu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.havefunace.top/gtzkgfrelb.html

TS:   arr.splice(0, 1);
来源：http://hz.9152youxi.cn/gtuqlmisym.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.snrcjt.cn/gtlgcvslsp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ywan-chungtsiang.top/gtlsjqoyib.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.aizwys.cn/gtiaworwlj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.gotoacloud.top/gtkgxtddca.html

[D05] 访问与修改元素
来源：http://hz.zdqjudy.top/gtvglvdgkw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pycfn.com/gtfztnnlzu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jiagoushi.top/gtrmuokfie.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.feifeiyinyue.top/gttjgollnn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hnxiangtu.top/gtzyeypwkt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cashguo.top/gtehjgvoqf.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtezcxdcee.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yueranfly.top/gtxursrhxn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gogol.net.cn/gtqwmiljga.html

[D06] 数组长度
来源：http://hz.daxiang520.top/gtthmaxvdi.html

Py:   len(arr)
来源：http://hz.cqqwz.cn/gtepztadle.html

PHP:  count($arr);
来源：http://hz.tian-w.cn/gtosfpjodu.html

JS:   arr.length
来源：http://hz.zycfv.cn/gtffcpdjqp.html

TS:   arr.length
来源：http://hz.hysaishi.cn/gtbvrpgtvq.html

Java: list.size();
来源：http://hz.nwbrower.top/gtlqvstkfq.html

Go:   len(arr)
来源：http://hz.cdnleiting.top/gtqkxhkmun.html

Ruby: arr.length; arr.size
来源：http://hz.sufxvd.cn/gtpynfxhet.html

C#:   list.Count;
来源：http://hz.yuanzhike.top/gtzmyplymu.html

[D07] 切片 / 取子数组
来源：http://hz.nwbrower.top/gtdglvhpxs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.smart0.xyz/gtwulcemwe.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xinyue.icu/gtcemcftyz.html

JS:   arr.slice(1, 4);
来源：http://hz.hongshengwenyu.top/gtaynmeiaq.html

TS:   arr.slice(1, 4);
来源：http://hz.svipenyu.cn/gtdvoeqiau.html

Java: list.subList(1, 4);
来源：http://hz.shanyushiyangkeji.top/gtstjrfbkn.html

Go:   arr[1:4]
来源：http://hz.xuanzx.com/gthkjerffc.html

Ruby: arr[1, 3]
来源：http://hz.zhiwuduotai.top/gtrsjtmuon.html

C#:   list.GetRange(1, 3);
来源：http://hz.9152youxi.cn/gtdpmwpetz.html

[D08] 合并两个数组
来源：http://hz.shuidangran.top/gtgdivgmuw.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhaomingkeji.xyz/gtklxnbnfp.html

PHP:  array_merge($a, $b);
来源：http://hz.tianlin.xyz/gtfycyukkx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cucudq.cn/gtnvvlwoom.html

TS:   [...a, ...b];
来源：http://hz.fengsongda.top/gtriwgpyeu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gaohongyu789.top/gtyahpjpxf.html

Go:   append(a, b...)
来源：http://hz.zhongyouzk.top/gtbkzxgnsn.html

Ruby: a + b;  a.concat(b)
来源：http://hz.quarkkingdee.top/gtqrhicgar.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenlongwang.top/gtpdvcwuuo.html

[D09] 排序（升序）
来源：http://hz.zdqjudy.top/gtoavfsfmf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daxiang520.top/gtpnesgevc.html

PHP:  sort($arr);
来源：http://hz.guowangkeji.top/gtcxfnzobf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.tanke756.top/gtxyckppes.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gzhubu.top/gtvmvdydpm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zdqjudy.top/gtlwjgmzmo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hnxiangtu.top/gtsuvgtcmo.html

Ruby: arr.sort
来源：http://hz.yangfankeji.com/gtjxeszzpt.html

C#:   list.Sort();
来源：http://hz.zhengqikj.top/gtiotjnljf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.chenzaomai.com/gtqvacibna.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.wangshuangyany.cn/gttfpmmgbm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hysaishi.cn/gtphgkjsfu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxinkj.top/gtzvmfpeou.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.52xcode.cn/gtlccgrapk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhiwuduotai.top/gtcrochzky.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.nanxuanxn.top/gtleqtgnyd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yvedp.cn/gtpmpwpdhp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nanxinkj.top/gtredxfrwn.html

[D11] 反转数组
来源：http://hz.redwolf501.top/gtmlscbppp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.dianchejie.cn/gtqhkaqsff.html

PHP:  array_reverse($arr);
来源：http://hz.shangyingyoupin.top/gtjgxlcxic.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.daria6918.cn/gtnmqvziul.html

TS:   [...arr].reverse();
来源：http://hz.pengpengdd.cyou/gthpjgzhid.html

Java: Collections.reverse(list);
来源：http://hz.0kj1m.cn/gtdlsbuwmu.html

Go:   slices.Reverse(arr)
来源：http://hz.sufxvd.cn/gtybdiacvi.html

Ruby: arr.reverse
来源：http://hz.ppjwa.cn/gtbkhkqidt.html

C#:   list.Reverse();
来源：http://hz.yuxming.cn/gtoahsiytp.html

[D12] 查找元素下标
来源：http://hz.chenjidiqi.icu/gtckjifgpl.html

Py:   arr.index(x);  x in arr
来源：http://hz.ydjk.org.cn/gtidlvcfyt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zdqjudy.top/gtybmbwwdb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ywan-chungtsiang.top/gtkuscyemq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nwbrower.top/gtvmvaqfha.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cucudq.cn/gtumnjrfig.html

Go:   slices.Index(arr, x)
来源：http://hz.hysaishi.cn/gtgjuufape.html

Ruby: arr.index(x)
来源：http://hz.tianlin.xyz/gtioowwnku.html

C#:   list.IndexOf(x);
来源：http://hz.zdqjudy.top/gtgftjbhvg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.nanxuanxn.top/gtvtvksfwn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.redwolf501.top/gtlfpvkisj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.iojbl.cn/gtfuercoof.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jianghu66.top/gtmupcbsef.html

TS:   arr.filter(x => x > 3)
来源：http://hz.0kj1m.cn/gtghlljxhv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hnqzz.top/gtzlpcqhio.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.bjfxy.top/gtdrbqnuas.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shanyushiyangkeji.top/gtkkkvgxvc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ybcxt.top/gtkoproavl.html

[D14] 映射转换（每个元素变形）
来源：http://hz.pengpengdd.cyou/gtrleazsry.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinyuanbaomall.cn/gtdhwjpulh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shuidangran.top/gtotjsochb.html

JS:   arr.map(x => x * 2)
来源：http://hz.xylfe.cn/gtaebskntc.html

TS:   arr.map(x => x * 2)
来源：http://hz.hammf.cn/gtajnrspoa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yanxiufei.cn/gtxjlugkwl.html

Go:   // 手写循环
来源：http://hz.haohaochexian.top/gtedmumgjr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhaomingkeji.xyz/gtpladujup.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.meibo888.top/gtiirvlxlv.html

[D15] 去重
来源：http://hz.zhengqikj.top/gtupqwemsm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ehwqpu.com/gthlndewcr.html

PHP:  array_unique($arr);
来源：http://hz.zhongyouzk.top/gtnvldqgua.html

JS:   [...new Set(arr)]
来源：http://hz.jqgfzy.top/gtecfgxryz.html

TS:   [...new Set(arr)]
来源：http://hz.smart0.xyz/gtnjjlkdfk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.gotoacloud.top/gthqfefmje.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.haohaochexian.top/gtgxvrxufe.html

Ruby: arr.uniq
来源：http://hz.havefunace.top/gtvqrljbvu.html

C#:   list.Distinct().ToList()
来源：http://hz.0kj1m.cn/gtuepxrjbt.html

[D16] 求和与平均值
来源：http://hz.chenlongwang.top/gtqqtbbjll.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hysaishi.cn/gtdbixerwz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fzhhl.top/gtptphvsng.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jyoumei.cn/gtchteacdu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.haohaochexian.top/gtpvemvczh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zdqjudy.top/gtqdxfbaij.html

Go:   // 手写循环累加
来源：http://hz.haohaochexian.top/gtvpmsffot.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shangyingyoupin.top/gtxiwkkmpe.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhongyouzk.top/gtwldgadvc.html

[D17] 最大值与最小值
来源：http://hz.daria6918.cn/gtcyteqhej.html

Py:   max(arr);  min(arr)
来源：http://hz.cucudq.cn/gtjvxvvwbp.html

PHP:  max($arr);  min($arr);
来源：http://hz.sufxvd.cn/gtiwbbqoxr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shanyushiyangkeji.top/gtoscmfxwi.html

TS:   Math.max(...arr);
来源：http://hz.guowangkeji.top/gtagceojii.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.0kj1m.cn/gtcqdjjphz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.pycfn.com/gtzxlgcnxy.html

Ruby: arr.max;  arr.min
来源：http://hz.haohaochexian.top/gtdgtwsenj.html

C#:   list.Max();  list.Min()
来源：http://hz.sxryk.cn/gtdsrxjalc.html

[D18] 扁平化嵌套数组
来源：http://hz.zycfv.cn/gthinkqawi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.dashuyun.cn/gtmzucbidc.html

PHP:  array_merge(...$nested);
来源：http://hz.fengsongda.top/gtawcycbcs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinqigfzy.top/gtybobsuzn.html

TS:   nested.flat();
来源：http://hz.ywan-chungtsiang.top/gtfcmujfor.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj20258.top/gtqvvslbgx.html

Go:   // 手写双层循环
来源：http://hz.nanxinkj.top/gtplmdkcxy.html

Ruby: nested.flatten
来源：http://hz.hammf.cn/gtetdajzqu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.guannengcc.top/gtqpmzwekx.html

[D19] 按字段分组
来源：http://hz.sweek.top/gtiszhmpeh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.316326.xyz/gtcympldpn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.feifeiyinyue.top/gtiktoqwyq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenlongwang.top/gtuknxwttw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.nanxuanxn.top/gtplfobhch.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhaomingkeji.xyz/gtaglbfdwc.html

Go:   // 手写 map[string][]T
来源：http://hz.aibaodan.cn/gtvajyiunh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cucudq.cn/gtzwaxlvre.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yanxiufei.cn/gtfgxwacfq.html

[D20] 统计每个元素出现次数
来源：http://hz.bjfxy.top/gtenrgzqwz.html

Py:   Counter(arr)
来源：http://hz.quarkkingdee.top/gttincfeww.html

PHP:  array_count_values($arr);
来源：http://hz.redwolf501.top/gtvozfkttm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangtech.top/gtviambsnu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aibaodan.cn/gtcsftblse.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhaomingkeji.xyz/gtzqvgmjws.html

Go:   // 手写 map[T]int
来源：http://hz.yanxiufei.cn/gtddmkjdoj.html

Ruby: arr.tally
来源：http://hz.cheryme.top/gtcqswixev.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.c1oappe.top/gtbewxqllq.html

[D21] 判断是否包含某元素
来源：http://hz.tian-w.cn/gtjedbsiyq.html

Py:   x in arr
来源：http://hz.sysykeji.top/gtfkggpezt.html

PHP:  in_array($x, $arr, true);
来源：http://hz.havefunace.top/gtofcgmhag.html

JS:   arr.includes(x)
来源：http://hz.yj20258.top/gthdbybzep.html

TS:   arr.includes(x)
来源：http://hz.sysykeji.top/gtamosufbj.html

Java: list.contains(x)
来源：http://hz.ywan-chungtsiang.top/gtqbqcaauz.html

Go:   slices.Contains(arr, x)
来源：http://hz.pengpengdd.cyou/gtvjpvfpha.html

Ruby: arr.include?(x)
来源：http://hz.xylfe.cn/gtiyssndct.html

C#:   list.Contains(x)
来源：http://hz.ywan-chungtsiang.top/gtgvpgnhph.html

[D22] 复制数组（避免共享引用）
来源：http://hz.meibo888.top/gtimbgdmov.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cheryme.top/gtegbprelz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shanyushiyangkeji.top/gtnjeyjhaw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhiwuduotai.top/gttpfbfjhs.html

TS:   [...arr];
来源：http://hz.jyoumei.cn/gtqhpzismd.html

Java: new ArrayList<>(list);
来源：http://hz.jinqigfzy.top/gtdqozhdnm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.guannengcc.top/gtlqbsurdu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.dianchejie.cn/gtkpbxtqlw.html

C#:   new List<int>(list);
来源：http://hz.jqgfzy.top/gtozpbwheu.html

[D23] reduce 累积计算
来源：http://hz.ydzc1.top/gthaofnlwt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.snrcjt.cn/gtjavwrixk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.fzhhl.top/gtrvzzfvqw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aibaodan.cn/gtnfououtn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxuanxn.top/gtdpoxrshb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jyoumei.cn/gtgiaowwet.html

Go:   // 手写循环
来源：http://hz.fzhhl.top/gtzjblhxgj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shangyingyoupin.top/gtdfxmtljn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.aizwys.cn/gtushbrlec.html

[D24] 字典 / Map 基本操作
来源：http://hz.gotoacloud.top/gthvlprmjr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gotoacloud.top/gtifshncna.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xylfe.cn/gtyseketpr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.meibo888.top/gthduvcxiw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jinghuilouyu.cn/gtrmjqvwvo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenjidiqi.icu/gtwavdebtm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cucudq.cn/gtisyrvlsz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hywenlv.cn/gtnixnstha.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.daxiang520.top/gtagaebgcy.html

[D25] Set 集合去重与交并差
来源：http://hz.smart0.xyz/gtjsfwrobb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sufxvd.cn/gtdhfavaxe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhongyouzk.top/gtvabgzrsq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yuanzhike.top/gtfkzdlnmv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.fengsongda.top/gtxmbsldjs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.wangshuangyany.cn/gtesoeocau.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.pycfn.com/gtzlhkutmf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hysaishi.cn/gtsiptiprv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.fzhhl.top/gtmlurspio.html

[D26] 数组转字符串
来源：http://hz.birdmap.top/gtjcjtlxsq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinghuilouyu.cn/gtiqttpuxi.html

PHP:  implode(", ", $arr);
来源：http://hz.shuidangran.top/gtvrcfbtpu.html

JS:   arr.join(", ")
来源：http://hz.sufxvd.cn/gtnhmflxeh.html

TS:   arr.join(", ")
来源：http://hz.cashguo.top/gttyscvrtm.html

Java: String.join(", ", list)
来源：http://hz.aizwys.cn/gtdzhyywil.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daxiang520.top/gthyctovec.html

Ruby: arr.join(", ")
来源：http://hz.jinqigufen.top/gtxzzyavrq.html

C#:   string.Join(", ", list)
来源：http://hz.316326.xyz/gtykpsdlfi.html

================================================================================
来源：http://hz.hnxiangtu.top/gtcwibgrvn.html

E. 字符串处理
来源：http://hz.yangfankeji.com/gthpqxqllv.html

================================================================================
来源：http://hz.jiagoushi.top/gtyuhjaezt.html

[E01] 拼接字符串
来源：http://hz.chenzaomai.com/gtijfgourr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ehwqpu.com/gtvgyaaotf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ydjk.org.cn/gtcvvrsvhf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shzxlz.cn/gtmyhacewf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.kuanghao11.cn/gtptxpplqw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ppjwa.cn/gtowdgrefg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenzaomai.com/gtysevhvlw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jianghu66.top/gtvakmqsiq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gzhubu.top/gtayjweypv.html

[E02] 重复字符串
来源：http://hz.jqgufenzy.top/gtptgnndow.html

Py:   "ab" * 3
来源：http://hz.jinqigufen.top/gtcytdxfua.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenlongwang.top/gtkwfufbbr.html

JS:   "ab".repeat(3)
来源：http://hz.zhiwuduotai.top/gtelsoknxc.html


<!-- 参考信息 -->