代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://hz.hfpthk.cn/gtabmbkbtb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.fzhhl.top/gtnyyltbvr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.nwbrower.top/gtekefsrkd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinyuanbaomall.cn/gtgzdqdgoc.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.fengsongda.top/gtxdaprthz.html

Ruby: -> { puts "run" }.call
来源：http://hz.shanyushiyangkeji.top/gtyunxbkjm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ydjk.org.cn/gtzbnubvnj.html

[C13] 类型声明 / 类型注解
来源：http://hz.chenzaomai.com/gtfvwzruhb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.svipenyu.cn/gtgctstnoo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtulercxbp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ivvv.top/gthhgtxhmt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jyoumei.cn/gtnpfapvam.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gogol.net.cn/gtyersgffc.html

Go:   func add(a, b int) int
来源：http://hz.jqgufenzy.top/gtdifjvuzr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.kuanghao11.cn/gtbbipofgq.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yangfankeji.com/gtojbeqmkd.html

[C14] 泛型函数
来源：http://hz.chenjidiqi.icu/gteejdrkme.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sxryk.cn/gthtujfttj.html

PHP:  // 无泛型
来源：http://hz.zhijiandao.cn/gtyrgnfium.html

JS:   // 无泛型
来源：http://hz.ivvv.top/gtklesxlft.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guowangkeji.top/gtdqolfqkl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.guowangkeji.top/gtekkkzukl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yueranfly.top/gthbvqjuoo.html

Ruby: # 无泛型
来源：http://hz.guannengcc.top/gtpxrdlemi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.c1oappe.top/gtirhwuwsh.html

[C15] 解构 / 展开参数
来源：http://hz.xinyue.icu/gtxuuopryf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hysaishi.cn/gtidywxynx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.dashuyun.cn/gtuvqnnczq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cashguo.top/gtxyczhdrl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yonumen.top/gtubwvkooe.html

Java: // 无解构
来源：http://hz.kuanghao11.cn/gtvwsnbabs.html

Go:   // 无解构
来源：http://hz.xuanzx.com/gtehfsnexk.html

Ruby: a, b = pair
来源：http://hz.ydjk.org.cn/gtddiwxpwm.html

C#:   var (a, b) = pair;
来源：http://hz.ywan-chungtsiang.top/gtidnicyzo.html

[C16] 函数 / 方法重载
来源：http://hz.sufxvd.cn/gtsdlyezcp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jlsjyb.cn/gtokjpykwd.html

PHP:  // 无重载
来源：http://hz.tianlin.xyz/gtzdljtijy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhixingplan.top/gtjcnkpmia.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jyoumei.cn/gtirycqxtg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.guowangkeji.top/gttmshtdja.html

Go:   // 无重载：用不同函数名
来源：http://hz.tian-w.cn/gtieztqvrl.html

Ruby: # 无重载：靠动态参数
来源：http://hz.guowangkeji.top/gtnhndvvkx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhijiandao.cn/gtrnigdhry.html

================================================================================
来源：http://hz.redwolf501.top/gtxtjccdbd.html

D. 数组 / 列表 / 集合
来源：http://hz.wangdashe.top/gtzwlnqzfd.html

================================================================================
来源：http://hz.hnxiangtu.top/gtymfoolvk.html

[D01] 创建数组 / 列表
来源：http://hz.jinghuilouyu.cn/gtomntrmdz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.smart0.xyz/gtssjoxvup.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.cucudq.cn/gtmmfxarat.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.feifeiyinyue.top/gtsickrqjw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.gaohongyu789.top/gtbnrzsdws.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.havefunace.top/gtgaveeofa.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xuetiantiany.cn/gtxvznxydb.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yonumen.top/gtjinxdlsd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yvedp.cn/gtdtkvxbvv.html

[D02] 追加元素到末尾
来源：http://hz.xuetiantiany.cn/gtqlrdlwng.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gaohongyu789.top/gtukyrzzlc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sxryk.cn/gtcayykalg.html

JS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gtqeckjthx.html

TS:   arr.push(4);
来源：http://hz.svipenyu.cn/gtgkosjmjo.html

Java: list.add(4);
来源：http://hz.ybcxt.top/gttbvfhrtk.html

Go:   arr = append(arr, 4)
来源：http://hz.cdnleiting.top/gtsfbbjsmy.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.sufxvd.cn/gtkhegyaio.html

C#:   list.Add(4);
来源：http://hz.jqgfzy.top/gtbjsfbitu.html

[D03] 在指定位置插入元素
来源：http://hz.bjfxy.top/gtslblppeu.html

Py:   arr.insert(0, 0)
来源：http://hz.sweek.top/gtzmwbkemv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yvedp.cn/gtgfuaezem.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhengqikj.top/gtxghdogxr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xylfe.cn/gtweblnhon.html

Java: list.add(0, 0);
来源：http://hz.chenjidiqi.icu/gtwpiehcal.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ppjwa.cn/gttqvbgxjl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xinyue.icu/gtjimrmeex.html

C#:   list.Insert(0, 0);
来源：http://hz.guowangkeji.top/gtqxbrdacm.html

[D04] 删除元素
来源：http://hz.yongpay.top/gttxthgvqg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhengqikj.top/gtfmzzrgcv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.nanxinkj.top/gtvbqkjixw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yangfankeji.com/gtdsiktiej.html

TS:   arr.splice(0, 1);
来源：http://hz.jyoumei.cn/gtqayluqkr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hnxiangtu.top/gthyyjixxw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xingfuxueyuan.xyz/gtgplspazs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenjidiqi.icu/gtloeevqur.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hongshengwenyu.top/gtjtmogbul.html

[D05] 访问与修改元素
来源：http://hz.daxiang520.top/gtxhyllkuz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jlsjyb.cn/gtmckhanob.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj20258.top/gtidobjizw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhijiandao.cn/gtozinlpzw.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xuetiantiany.cn/gtdjfgslwz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fengsongda.top/gtfammlvvw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tianlin.xyz/gtjwrsagly.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydzc1.top/gtgsalimij.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.feifeiyinyue.top/gthgjittvt.html

[D06] 数组长度
来源：http://hz.andypj.xyz/gtrvbwdyzz.html

Py:   len(arr)
来源：http://hz.guannengcc.top/gtrclxtuag.html

PHP:  count($arr);
来源：http://hz.yuanzhike.top/gtiyejhbir.html

JS:   arr.length
来源：http://hz.yuxming.cn/gtqejjskyl.html

TS:   arr.length
来源：http://hz.quarkkingdee.top/gtvjbegdch.html

Java: list.size();
来源：http://hz.xuanzx.com/gttcceodpe.html

Go:   len(arr)
来源：http://hz.kuanghao11.cn/gtuhxjuiib.html

Ruby: arr.length; arr.size
来源：http://hz.shangyingyoupin.top/gtxmvlmjsb.html

C#:   list.Count;
来源：http://hz.jinyuanbaomall.cn/gtdcunitun.html

[D07] 切片 / 取子数组
来源：http://hz.yvedp.cn/gtkoocmjct.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shanyushiyangtech.top/gtxtvxihzs.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zycfv.cn/gtpdmlwdxf.html

JS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gtlgbwmuxe.html

TS:   arr.slice(1, 4);
来源：http://hz.xinyue.icu/gterdfaund.html

Java: list.subList(1, 4);
来源：http://hz.smart0.xyz/gtayhcojka.html

Go:   arr[1:4]
来源：http://hz.ivvv.top/gtwcwfyepa.html

Ruby: arr[1, 3]
来源：http://hz.zhijiandao.cn/gtewascnff.html

C#:   list.GetRange(1, 3);
来源：http://hz.wangdashe.top/gtsxbfltpa.html

[D08] 合并两个数组
来源：http://hz.birdmap.top/gttjkzvdle.html

Py:   a + b;  a.extend(b)
来源：http://hz.0kj1m.cn/gtrsqymkot.html

PHP:  array_merge($a, $b);
来源：http://hz.yangfankeji.com/gtqpmyfjht.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jyoumei.cn/gtwxpnlqbs.html

TS:   [...a, ...b];
来源：http://hz.ivvv.top/gtjuwvskin.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangtech.top/gtxxtmyusr.html

Go:   append(a, b...)
来源：http://hz.xylfe.cn/gtcowwybdk.html

Ruby: a + b;  a.concat(b)
来源：http://hz.fzhhl.top/gtqhzjvgld.html

C#:   a.Concat(b).ToList()
来源：http://hz.xuetiantiany.cn/gthhdcuvtl.html

[D09] 排序（升序）
来源：http://hz.0kj1m.cn/gtighgbjct.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jlsjyb.cn/gtuaqrvbgf.html

PHP:  sort($arr);
来源：http://hz.fzhhl.top/gthokvmiti.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gaohongyu789.top/gtieaubhlu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.nwbrower.top/gtvwapbkot.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.daxiang520.top/gtawffasuc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.sysykeji.top/gtvpwcyqdm.html

Ruby: arr.sort
来源：http://hz.yuxming.cn/gtwwbjqpec.html

C#:   list.Sort();
来源：http://hz.jiagoushi.top/gtjwpucazr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.316326.xyz/gtkhvvimxh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.pycfn.com/gtuxnktgla.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hywenlv.cn/gtlvdulvyd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtmrhqofph.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yongpay.top/gtywmttbgu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jlsjyb.cn/gtqjxlljnn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jqgufenzy.top/gtwnlmfwxu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xinyue.icu/gtfacjbhna.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nanxuanxn.top/gttiwuthbl.html

[D11] 反转数组
来源：http://hz.zycfv.cn/gtctmiwhnh.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhongyouzk.top/gtaurvxrzg.html

PHP:  array_reverse($arr);
来源：http://hz.ywan-chungtsiang.top/gtirnticqh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.birdmap.top/gtmamjifyv.html

TS:   [...arr].reverse();
来源：http://hz.tian-w.cn/gtxjkwmgkc.html

Java: Collections.reverse(list);
来源：http://hz.hnqzz.top/gtnkxleaye.html

Go:   slices.Reverse(arr)
来源：http://hz.jinghuilouyu.cn/gtnzdplvkg.html

Ruby: arr.reverse
来源：http://hz.chenzaomai.com/gtmerxdcek.html

C#:   list.Reverse();
来源：http://hz.52xcode.cn/gtllulkkpd.html

[D12] 查找元素下标
来源：http://hz.chenzaomai.com/gtcwqvcmtf.html

Py:   arr.index(x);  x in arr
来源：http://hz.guowangkeji.top/gtmiecxqon.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ybcxt.top/gtuaqupeud.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hongshengwenyu.top/gtrbngrakv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.svipenyu.cn/gttvzqdpga.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ywan-chungtsiang.top/gtfmombzrl.html

Go:   slices.Index(arr, x)
来源：http://hz.0kj1m.cn/gtgryjadwz.html

Ruby: arr.index(x)
来源：http://hz.ehwqpu.com/gtrsyxtqxp.html

C#:   list.IndexOf(x);
来源：http://hz.9152youxi.cn/gtsihobnjf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinyuanbaomall.cn/gtyvbhhtsb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zdqjudy.top/gtrdhdgkdx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.quarkkingdee.top/gtmlioqoge.html

JS:   arr.filter(x => x > 3)
来源：http://hz.dashuyun.cn/gtqnbjvjgu.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hfpthk.cn/gthhuurqqq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ywan-chungtsiang.top/gtxcfjpxej.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.smart0.xyz/gtmubsancx.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.daria6918.cn/gtmewggsrm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.havefunace.top/gtzgmzjtgg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nwbrower.top/gtbfmrnieb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.dashuyun.cn/gtkppxbzgt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xylfe.cn/gtvbebwsru.html

JS:   arr.map(x => x * 2)
来源：http://hz.dashuyun.cn/gthnicxnsb.html

TS:   arr.map(x => x * 2)
来源：http://hz.daxiang520.top/gtznmombxf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hfpthk.cn/gtkhxpdihv.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gtwdqlcdzg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yonumen.top/gtagpsmlvm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.pycfn.com/gtwpbnsybl.html

[D15] 去重
来源：http://hz.yvedp.cn/gtmurwvyok.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nwbrower.top/gtqwlpbqtf.html

PHP:  array_unique($arr);
来源：http://hz.cucudq.cn/gtqjgzirso.html

JS:   [...new Set(arr)]
来源：http://hz.xziqi.cn/gtcdfypvsv.html

TS:   [...new Set(arr)]
来源：http://hz.jqgfzy.top/gtbllfogdb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shzxlz.cn/gtdeptnooe.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.sysykeji.top/gtvcbojdhi.html

Ruby: arr.uniq
来源：http://hz.redwolf501.top/gtllouqyxy.html

C#:   list.Distinct().ToList()
来源：http://hz.dianchejie.cn/gtrhcklmip.html

[D16] 求和与平均值
来源：http://hz.cqqwz.cn/gtwtmcqggt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jqgfzy.top/gtbqqnuzpw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhengqikj.top/gtbqmzuafj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cdnleiting.top/gtvjbhsprf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtsnergqfs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.aibaodan.cn/gtgfbxtceu.html

Go:   // 手写循环累加
来源：http://hz.hfpthk.cn/gtkgtqsjef.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gogol.net.cn/gtfcuiqpny.html

C#:   list.Sum();  list.Average()
来源：http://hz.hysaishi.cn/gtjcogndos.html

[D17] 最大值与最小值
来源：http://hz.sufxvd.cn/gtnkmasjee.html

Py:   max(arr);  min(arr)
来源：http://hz.cashguo.top/gtzvoqwolz.html

PHP:  max($arr);  min($arr);
来源：http://hz.yueranfly.top/gtscruixdi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shanyushiyangkeji.top/gtyvvhyryv.html

TS:   Math.max(...arr);
来源：http://hz.yanxiufei.cn/gtadggluqx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zdqjudy.top/gtmhcdrbki.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cucudq.cn/gtdkgyxbgv.html

Ruby: arr.max;  arr.min
来源：http://hz.guowangkeji.top/gttbwpnrsr.html

C#:   list.Max();  list.Min()
来源：http://hz.ybcxt.top/gtptbgiyuk.html

[D18] 扁平化嵌套数组
来源：http://hz.dianchejie.cn/gtlxykwott.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hnxiangtu.top/gtipmnuvoz.html

PHP:  array_merge(...$nested);
来源：http://hz.xingfuxueyuan.xyz/gtwykndjdf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.9152youxi.cn/gtkpwedmdn.html

TS:   nested.flat();
来源：http://hz.nwbrower.top/gtrrpkhirg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.wangdashe.top/gtwfmyhplp.html

Go:   // 手写双层循环
来源：http://hz.quarkkingdee.top/gtkkfuzmno.html

Ruby: nested.flatten
来源：http://hz.jinqigufen.top/gtsjtvdvey.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yueranfly.top/gtbirlssjg.html

[D19] 按字段分组
来源：http://hz.yvedp.cn/gtpfelcwun.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.iojbl.cn/gtntupmmzs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.guowangkeji.top/gtwnaviuwv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.quarkkingdee.top/gtjxxmfudw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ywan-chungtsiang.top/gtaxthvzxc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ivvv.top/gtzowqriul.html

Go:   // 手写 map[string][]T
来源：http://hz.redwolf501.top/gthxtlkzfv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.nanxinkj.top/gtrjxdpjxv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ydjk.org.cn/gtxzjmyvhb.html

[D20] 统计每个元素出现次数
来源：http://hz.tianlin.xyz/gtexhloxda.html

Py:   Counter(arr)
来源：http://hz.zhaomingkeji.xyz/gtpstzsegf.html

PHP:  array_count_values($arr);
来源：http://hz.guannengcc.top/gtpudbybbf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hammf.cn/gtymrkzjdm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ppjwa.cn/gtkgtttgpo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hysaishi.cn/gtuiszrtdn.html

Go:   // 手写 map[T]int
来源：http://hz.shanyushiyangtech.top/gtoxkoblax.html

Ruby: arr.tally
来源：http://hz.xylfe.cn/gtwkhpcjdn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.wangdashe.top/gtnignusjm.html

[D21] 判断是否包含某元素
来源：http://hz.zycfv.cn/gtxfgfhtmm.html

Py:   x in arr
来源：http://hz.zhixingplan.top/gtjharihfh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xingfuxueyuan.xyz/gtvawjnhef.html

JS:   arr.includes(x)
来源：http://hz.gaohongyu789.top/gtgegtuibl.html

TS:   arr.includes(x)
来源：http://hz.hnqzz.top/gtudcugdmi.html

Java: list.contains(x)
来源：http://hz.c1oappe.top/gtpwwbxild.html

Go:   slices.Contains(arr, x)
来源：http://hz.xuanzx.com/gtdizcswvh.html

Ruby: arr.include?(x)
来源：http://hz.zycfv.cn/gtdbkhtjls.html

C#:   list.Contains(x)
来源：http://hz.mhx1999.top/gtyqbeyafn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hywenlv.cn/gtemyyhgbv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jlsjyb.cn/gtifmrvuvu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yj202588.top/gtpieavrmb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xuetiantiany.cn/gtxduzadkt.html

TS:   [...arr];
来源：http://hz.jyoumei.cn/gtqrwtkvtp.html

Java: new ArrayList<>(list);
来源：http://hz.aibaodan.cn/gtewaorylb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj20258888.top/gtmmkpetme.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zdqjudy.top/gtsjzflimj.html

C#:   new List<int>(list);
来源：http://hz.sxryk.cn/gtyvbggssy.html

[D23] reduce 累积计算
来源：http://hz.bjfxy.top/gtfaasqbfy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daria6918.cn/gticggfobg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.snrcjt.cn/gttnxyiwpc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnqzz.top/gtcisyknyh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fzhhl.top/gtagotwsty.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnxiangtu.top/gtypcvodyz.html

Go:   // 手写循环
来源：http://hz.hnqzz.top/gterdhsopj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ywan-chungtsiang.top/gtqkkxuqbh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.snrcjt.cn/gttxzzxixy.html

[D24] 字典 / Map 基本操作
来源：http://hz.haohaochexian.top/gtpurbttoz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhoulong.xyz/gttulnbcfg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ydjk.org.cn/gtzzxxfdke.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.snrcjt.cn/gtszmdswgp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.316326.xyz/gtvgzjqxwi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxinkj.top/gtewmpdlko.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.meibo888.top/gtgtqavjdj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.0kj1m.cn/gtmbfrcpmp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhixingplan.top/gthxrkicsx.html

[D25] Set 集合去重与交并差
来源：http://hz.yj20258888.top/gtfypzpgwf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gotoacloud.top/gtlfgjermp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cdnleiting.top/gtbaynkgxz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shangyingyoupin.top/gtpbxlvgrs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shanyushiyangkeji.top/gtbrdlxfin.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.9152youxi.cn/gtuxcewozj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xylfe.cn/gtlnemnail.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yuanzhike.top/gtzxgkwzhg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.dashuyun.cn/gtzuqrryxc.html

[D26] 数组转字符串
来源：http://hz.chenzaomai.com/gtlawprfzy.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gogol.net.cn/gtycxerlnh.html

PHP:  implode(", ", $arr);
来源：http://hz.hywenlv.cn/gtobgubevf.html

JS:   arr.join(", ")
来源：http://hz.havefunace.top/gtoorlnveo.html

TS:   arr.join(", ")
来源：http://hz.jlsjyb.cn/gtpbsvwcsa.html

Java: String.join(", ", list)
来源：http://hz.zhoulong.xyz/gtztmurvsf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.kuanghao11.cn/gtlabdcxyb.html

Ruby: arr.join(", ")
来源：http://hz.zdqjudy.top/gtoyolivje.html

C#:   string.Join(", ", list)
来源：http://hz.zhixingplan.top/gtvaaizldx.html

================================================================================
来源：http://hz.zhixingplan.top/gtodrluxtw.html

E. 字符串处理
来源：http://hz.gzhubu.top/gtkizcaeie.html

================================================================================
来源：http://hz.shzxlz.cn/gtdpqugxws.html

[E01] 拼接字符串
来源：http://hz.yuxming.cn/gtjiyqtwdn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.chenzaomai.com/gtjitrvuko.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yangfankeji.com/gtlcdzbvep.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.52xcode.cn/gtiznwnnek.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nwbrower.top/gtfrlaqhjc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yj20258.top/gthzrwsbrw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.daxiang520.top/gtlniqrlxz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhongyouzk.top/gtqrziqvvi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hnxiangtu.top/gtqqjjctzc.html

[E02] 重复字符串
来源：http://hz.yuxming.cn/gttqyctsac.html

Py:   "ab" * 3
来源：http://hz.xziqi.cn/gtjgiacdpq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zycfv.cn/gtotpibjah.html

JS:   "ab".repeat(3)
来源：http://hz.sufxvd.cn/gtgowoeeqb.html

TS:   "ab".repeat(3)
来源：http://hz.hnqzz.top/gtlhuooson.html

Java: "ab".repeat(3)
来源：http://hz.zhongyouzk.top/gtubjncblg.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jqgfzy.top/gtzdjjwlfh.html

Ruby: "ab" * 3
来源：http://hz.zhiwuduotai.top/gtkniynloa.html


<!-- 参考信息 -->