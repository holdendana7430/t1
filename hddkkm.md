代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://hz.daxiang520.top/gtweqrdzwc.html

JS:   (() => { console.log("run"); })();
来源：http://hz.316326.xyz/gtgxkrnsyu.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yangfankeji.com/gtbdpyqkeh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jyoumei.cn/gthhgkswxk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.c1oappe.top/gtuoivalfm.html

Ruby: -> { puts "run" }.call
来源：http://hz.sufxvd.cn/gtwuzepave.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.havefunace.top/gtuyasrmxr.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhixingplan.top/gtugllhrdp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nanxinkj.top/gtnvdbjjws.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aibaodan.cn/gtelyrzect.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.havefunace.top/gteuciwzof.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xylfe.cn/gtqyxpdsaf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gtdovtdgnc.html

Go:   func add(a, b int) int
来源：http://hz.shanyushiyangtech.top/gtjscppjxh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.tianlin.xyz/gtnbjvicxa.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sufxvd.cn/gtvuphtzhu.html

[C14] 泛型函数
来源：http://hz.fzhhl.top/gtpaeiiakq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.bjfxy.top/gtrrhuybaa.html

PHP:  // 无泛型
来源：http://hz.redwolf501.top/gtasbmnkir.html

JS:   // 无泛型
来源：http://hz.cashguo.top/gteczxiwjs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sxryk.cn/gtkrjlmryu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shuidangran.top/gtnlsmejqm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhengqikj.top/gtsdicurxt.html

Ruby: # 无泛型
来源：http://hz.chenjidiqi.icu/gtyjpyvtji.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhaomingkeji.xyz/gtkubyxofj.html

[C15] 解构 / 展开参数
来源：http://hz.kuanghao11.cn/gtprfanoom.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.daxiang520.top/gteblgvcrm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jiagoushi.top/gtuianlbpw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhijiandao.cn/gtwzeftncu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cdnleiting.top/gtolxhrfki.html

Java: // 无解构
来源：http://hz.tian-w.cn/gtzrbbplrl.html

Go:   // 无解构
来源：http://hz.andypj.xyz/gtieofbbqv.html

Ruby: a, b = pair
来源：http://hz.jinyuanbaomall.cn/gtdpejczkh.html

C#:   var (a, b) = pair;
来源：http://hz.gotoacloud.top/gtciywhogn.html

[C16] 函数 / 方法重载
来源：http://hz.xziqi.cn/gtqgsppoge.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gogol.net.cn/gtqkiwclys.html

PHP:  // 无重载
来源：http://hz.sysykeji.top/gtdagjjdgu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigfzy.top/gtwgzmrngz.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hfpthk.cn/gtrmivqhqq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.iojbl.cn/gtpxqwphuu.html

Go:   // 无重载：用不同函数名
来源：http://hz.jqgfzy.top/gtrumqeeeq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ywan-chungtsiang.top/gtmiwqhwcu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cqqwz.cn/gthrripucm.html

================================================================================
来源：http://hz.316326.xyz/gtlkelysso.html

D. 数组 / 列表 / 集合
来源：http://hz.jqgfzy.top/gttirbckpq.html

================================================================================
来源：http://hz.hnxiangtu.top/gtvpbyofld.html

[D01] 创建数组 / 列表
来源：http://hz.pycfn.com/gtqssifssg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.daxiang520.top/gtlckypimx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hammf.cn/gtdjaaoeen.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.havefunace.top/gtuqlfwuuk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yueranfly.top/gtqkthuzvf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.gogol.net.cn/gtsqiuchie.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhixingplan.top/gtvwmstxmy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cdnleiting.top/gtqvubkxyi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuanzx.com/gtvtmrgkga.html

[D02] 追加元素到末尾
来源：http://hz.jqgfzy.top/gtkpehfkbz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xuanzx.com/gtfwiienig.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xinyue.icu/gtubwshxeq.html

JS:   arr.push(4);
来源：http://hz.dashuyun.cn/gtwdtixnil.html

TS:   arr.push(4);
来源：http://hz.zhijiandao.cn/gtdeqqsijm.html

Java: list.add(4);
来源：http://hz.xylfe.cn/gtpwjsdkav.html

Go:   arr = append(arr, 4)
来源：http://hz.gzhubu.top/gtcvkdvzrk.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hysaishi.cn/gthmqxnbsk.html

C#:   list.Add(4);
来源：http://hz.pycfn.com/gtjayegqyv.html

[D03] 在指定位置插入元素
来源：http://hz.redwolf501.top/gtubetqeqc.html

Py:   arr.insert(0, 0)
来源：http://hz.jinqigufen.top/gtwbvgjhwe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xuanzx.com/gttdlkohlc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hywenlv.cn/gtwvgusuum.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hnqzz.top/gtrotpduaq.html

Java: list.add(0, 0);
来源：http://hz.hnqzz.top/gtmkrtxido.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hywenlv.cn/gtidhsltoc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shanyushiyangtech.top/gtbozfptiw.html

C#:   list.Insert(0, 0);
来源：http://hz.sysykeji.top/gtllhfvfsw.html

[D04] 删除元素
来源：http://hz.gaohongyu789.top/gtsmgpgyzi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.tian-w.cn/gtlnvfhrbt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zycfv.cn/gtxqbkeogx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shangyingyoupin.top/gtcfvjeonw.html

TS:   arr.splice(0, 1);
来源：http://hz.cashguo.top/gtvahbhhrh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.birdmap.top/gtuygflopb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cdnleiting.top/gtsjyqxtul.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ywan-chungtsiang.top/gtjdvcvmai.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.0kj1m.cn/gtfcbmzddd.html

[D05] 访问与修改元素
来源：http://hz.yanxiufei.cn/gtdsukfozu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yongpay.top/gtzrhatwwv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shangyingyoupin.top/gtgvamoylz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinqigfzy.top/gtenwywzkz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nanxinkj.top/gtssztoisd.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuxming.cn/gtpgfxjtzg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtwogekyuc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fengsongda.top/gtmizyfzsb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhixingplan.top/gtjpucdcqm.html

[D06] 数组长度
来源：http://hz.jinqigfzy.top/gticuqpkwh.html

Py:   len(arr)
来源：http://hz.yuxming.cn/gtfmodynse.html

PHP:  count($arr);
来源：http://hz.cqqwz.cn/gtyanppkqt.html

JS:   arr.length
来源：http://hz.fengsongda.top/gtcyusuwsj.html

TS:   arr.length
来源：http://hz.pengpengdd.cyou/gtepabofon.html

Java: list.size();
来源：http://hz.kuanghao11.cn/gtbucoplwa.html

Go:   len(arr)
来源：http://hz.yongpay.top/gtipmtoivd.html

Ruby: arr.length; arr.size
来源：http://hz.fengsongda.top/gtumyshxiq.html

C#:   list.Count;
来源：http://hz.hfpthk.cn/gtjwsvebqh.html

[D07] 切片 / 取子数组
来源：http://hz.chenlongwang.top/gtirqjuexj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.9152youxi.cn/gtjcfkaymv.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.iojbl.cn/gtrbmbfdru.html

JS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangtech.top/gtgxzwxnfs.html

TS:   arr.slice(1, 4);
来源：http://hz.zhiwuduotai.top/gtdlqtbfyy.html

Java: list.subList(1, 4);
来源：http://hz.tanke756.top/gtzbyubmzr.html

Go:   arr[1:4]
来源：http://hz.jqgfzy.top/gtnjjnwczy.html

Ruby: arr[1, 3]
来源：http://hz.shanyushiyangkeji.top/gtimvfiydm.html

C#:   list.GetRange(1, 3);
来源：http://hz.xziqi.cn/gtnehoesis.html

[D08] 合并两个数组
来源：http://hz.jinyuanbaomall.cn/gtnekjocyk.html

Py:   a + b;  a.extend(b)
来源：http://hz.cashguo.top/gtdpezisgb.html

PHP:  array_merge($a, $b);
来源：http://hz.ehwqpu.com/gtdznevbdc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gotoacloud.top/gtdovxektf.html

TS:   [...a, ...b];
来源：http://hz.redwolf501.top/gtwlipclxl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ybcxt.top/gtviyillly.html

Go:   append(a, b...)
来源：http://hz.316326.xyz/gthskltsln.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ywan-chungtsiang.top/gtgrgbocrr.html

C#:   a.Concat(b).ToList()
来源：http://hz.tianlin.xyz/gttsrzmaqu.html

[D09] 排序（升序）
来源：http://hz.sufxvd.cn/gtiqzentci.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aizwys.cn/gtdofdokcf.html

PHP:  sort($arr);
来源：http://hz.pycfn.com/gtkxqlqvtp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.daria6918.cn/gtprwdtuqf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ybcxt.top/gtllkedmnj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sufxvd.cn/gtbwimtuzs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.mhx1999.top/gtcjdojlee.html

Ruby: arr.sort
来源：http://hz.yuanzhike.top/gtvrjaoxcz.html

C#:   list.Sort();
来源：http://hz.ppjwa.cn/gtzdfqvzim.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.quarkkingdee.top/gtfbdnbllr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hongshengwenyu.top/gtgzyjfysg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.redwolf501.top/gtnywgljph.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuxming.cn/gtheipwccy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tian-w.cn/gtuinqpexs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yuanzhike.top/gtnqeofkot.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cdnleiting.top/gtutnsosgq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yanxiufei.cn/gtwnrgiqex.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhaomingkeji.xyz/gtvsqufoua.html

[D11] 反转数组
来源：http://hz.havefunace.top/gtkptqcglg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jqgufenzy.top/gtqzrnifiu.html

PHP:  array_reverse($arr);
来源：http://hz.zhongyouzk.top/gthezdgdil.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yuanzhike.top/gtwdqtuphv.html

TS:   [...arr].reverse();
来源：http://hz.sysykeji.top/gtedjyyqqd.html

Java: Collections.reverse(list);
来源：http://hz.haohaochexian.top/gtbmrciimk.html

Go:   slices.Reverse(arr)
来源：http://hz.0kj1m.cn/gtywfoaysb.html

Ruby: arr.reverse
来源：http://hz.shanyushiyangtech.top/gteayghvig.html

C#:   list.Reverse();
来源：http://hz.svipenyu.cn/gtxcqopoeq.html

[D12] 查找元素下标
来源：http://hz.meibo888.top/gtdewaqwor.html

Py:   arr.index(x);  x in arr
来源：http://hz.nanxinkj.top/gtguzgddth.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.dashuyun.cn/gtyfialang.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnqzz.top/gttxzncknh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xuetiantiany.cn/gtxyhbfcvp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sweek.top/gtgihgnovf.html

Go:   slices.Index(arr, x)
来源：http://hz.nwbrower.top/gttcyasjct.html

Ruby: arr.index(x)
来源：http://hz.shuidangran.top/gtkdtppday.html

C#:   list.IndexOf(x);
来源：http://hz.yuxming.cn/gtglryxleq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.pengpengdd.cyou/gtonvxfjmg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhengqikj.top/gtnavvmkri.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.nwbrower.top/gtidwghglo.html

JS:   arr.filter(x => x > 3)
来源：http://hz.quarkkingdee.top/gtorhfwsnm.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ppjwa.cn/gtkpycyvow.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.fengsongda.top/gtfbqudjxc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.svipenyu.cn/gtflzpaiyo.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jlsjyb.cn/gtmvrxrxdn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.wangshuangyany.cn/gteanigicr.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhiwuduotai.top/gtbaggjpxz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.wangdashe.top/gtnindbuhz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cheryme.top/gtklpuaqpi.html

JS:   arr.map(x => x * 2)
来源：http://hz.hysaishi.cn/gtlfudsexz.html

TS:   arr.map(x => x * 2)
来源：http://hz.daria6918.cn/gtgkfuimex.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.chenjidiqi.icu/gtwvijmsku.html

Go:   // 手写循环
来源：http://hz.hnxiangtu.top/gtuddouahf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.mhx1999.top/gtxsmbunwk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yuanzhike.top/gtosbpksbe.html

[D15] 去重
来源：http://hz.birdmap.top/gtbirkycpc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinqigfzy.top/gtxkhkwjtb.html

PHP:  array_unique($arr);
来源：http://hz.dashuyun.cn/gtwvvmbrld.html

JS:   [...new Set(arr)]
来源：http://hz.xuanzx.com/gtvdjklsyg.html

TS:   [...new Set(arr)]
来源：http://hz.aizwys.cn/gtohsahyzf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yangfankeji.com/gtfqivgccn.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinghuilouyu.cn/gtbkxqpqzl.html

Ruby: arr.uniq
来源：http://hz.feifeiyinyue.top/gttmxvrmwm.html

C#:   list.Distinct().ToList()
来源：http://hz.iojbl.cn/gtftpvjrsd.html

[D16] 求和与平均值
来源：http://hz.smart0.xyz/gtiumndakq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.kuanghao11.cn/gtapezwtoe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.9152youxi.cn/gtjhrmyoey.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtmdymwqlh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nwbrower.top/gtftsciqor.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.daxiang520.top/gtftqvfwcc.html

Go:   // 手写循环累加
来源：http://hz.havefunace.top/gtppishjjh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhoulong.xyz/gtmhksdlug.html

C#:   list.Sum();  list.Average()
来源：http://hz.hnqzz.top/gttcfkeovr.html

[D17] 最大值与最小值
来源：http://hz.aizwys.cn/gtgmeucomi.html

Py:   max(arr);  min(arr)
来源：http://hz.smart0.xyz/gtxghgbjvp.html

PHP:  max($arr);  min($arr);
来源：http://hz.316326.xyz/gtoatetfwe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jiagoushi.top/gterxzhklt.html

TS:   Math.max(...arr);
来源：http://hz.yangfankeji.com/gtitzuozol.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ehwqpu.com/gtpkvlfqot.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.meibo888.top/gtzryqgkds.html

Ruby: arr.max;  arr.min
来源：http://hz.smart0.xyz/gtaehqkcmi.html

C#:   list.Max();  list.Min()
来源：http://hz.jinqigfzy.top/gtslszqbho.html

[D18] 扁平化嵌套数组
来源：http://hz.guannengcc.top/gtfzncjyql.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jinyuanbaomall.cn/gtvgpbipdh.html

PHP:  array_merge(...$nested);
来源：http://hz.dianchejie.cn/gtnhcbjpbs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.redwolf501.top/gtiyegkaoe.html

TS:   nested.flat();
来源：http://hz.shzxlz.cn/gtnlmkwtdt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yanxiufei.cn/gtybojycou.html

Go:   // 手写双层循环
来源：http://hz.zhixingplan.top/gtknzvmydd.html

Ruby: nested.flatten
来源：http://hz.aizwys.cn/gtwxtkahoc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xuetiantiany.cn/gtoqiurror.html

[D19] 按字段分组
来源：http://hz.aibaodan.cn/gtsexnsjcj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xylfe.cn/gtygxxyuqf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.aizwys.cn/gtwmwdhxzf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.9152youxi.cn/gtbipfztoy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ydjk.org.cn/gtjwamlpbs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.c1oappe.top/gtaivskyyt.html

Go:   // 手写 map[string][]T
来源：http://hz.aibaodan.cn/gtszpgduvp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gzhubu.top/gtsvtqqcod.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.9152youxi.cn/gtstycomst.html

[D20] 统计每个元素出现次数
来源：http://hz.316326.xyz/gtihcwlckj.html

Py:   Counter(arr)
来源：http://hz.nanxinkj.top/gtyjpmimwb.html

PHP:  array_count_values($arr);
来源：http://hz.tianlin.xyz/gtrftqawyu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258.top/gturbyyvfn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnqzz.top/gttpumshdm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.andypj.xyz/gtzkgzfzua.html

Go:   // 手写 map[T]int
来源：http://hz.hysaishi.cn/gtlsbnpnyp.html

Ruby: arr.tally
来源：http://hz.gzhubu.top/gtvynvifds.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.quarkkingdee.top/gtlzpsryif.html

[D21] 判断是否包含某元素
来源：http://hz.316326.xyz/gtopirefac.html

Py:   x in arr
来源：http://hz.quarkkingdee.top/gtabyjiatd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yangfankeji.com/gtzgqvdtfi.html

JS:   arr.includes(x)
来源：http://hz.jinqigufen.top/gtqqlbwjzj.html

TS:   arr.includes(x)
来源：http://hz.ywan-chungtsiang.top/gtzvhbnmpm.html

Java: list.contains(x)
来源：http://hz.aibaodan.cn/gtuluvxgyq.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuxming.cn/gtflhtdlbx.html

Ruby: arr.include?(x)
来源：http://hz.hnqzz.top/gtndrnwtvu.html

C#:   list.Contains(x)
来源：http://hz.daxiang520.top/gtmxcowyii.html

[D22] 复制数组（避免共享引用）
来源：http://hz.mhx1999.top/gtapjkezqm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhijiandao.cn/gtjihtqion.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ybcxt.top/gtaxjcdfrh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yueranfly.top/gtyilqwkhd.html

TS:   [...arr];
来源：http://hz.9152youxi.cn/gtoxslfmlb.html

Java: new ArrayList<>(list);
来源：http://hz.smart0.xyz/gtqloxyyam.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.smart0.xyz/gtzkqkjqff.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jianghu66.top/gterkqpouf.html

C#:   new List<int>(list);
来源：http://hz.gotoacloud.top/gtcrtxzyvh.html

[D23] reduce 累积计算
来源：http://hz.sxryk.cn/gtwxpdypdq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jyoumei.cn/gtprlaqlof.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tian-w.cn/gtfzajgzzq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ybcxt.top/gtlrfbvzjk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fengsongda.top/gtbrrkgmxo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.birdmap.top/gtnyznxdlo.html

Go:   // 手写循环
来源：http://hz.xuetiantiany.cn/gttyqgnklc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ydjk.org.cn/gtdzifmwel.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhoulong.xyz/gttvgccazb.html

[D24] 字典 / Map 基本操作
来源：http://hz.iojbl.cn/gtsakpbgoj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yongpay.top/gtrlqsfonv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.chenlongwang.top/gtmrwrdcca.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yonumen.top/gtigliptpa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhoulong.xyz/gtbwroyeem.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gzhubu.top/gtsincnhtq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhijiandao.cn/gtbflmmrkt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.aibaodan.cn/gtzxqpucev.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jlsjyb.cn/gtkufmbldc.html

[D25] Set 集合去重与交并差
来源：http://hz.birdmap.top/gtnzeufdmk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ywan-chungtsiang.top/gtdrfetwrl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhixingplan.top/gtcfrpjstp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cqqwz.cn/gtrlsqymuu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yongpay.top/gtiiqgqdvc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hywenlv.cn/gtplouiiei.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.havefunace.top/gtxwdwgogc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jianghu66.top/gtjpdfnzpb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zdqjudy.top/gtncovxgqc.html

[D26] 数组转字符串
来源：http://hz.zhengqikj.top/gtxqsjkllm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tianlin.xyz/gtddnbjavi.html

PHP:  implode(", ", $arr);
来源：http://hz.pengpengdd.cyou/gtnqodpuzw.html

JS:   arr.join(", ")
来源：http://hz.yuanzhike.top/gtpwzveuaw.html

TS:   arr.join(", ")
来源：http://hz.yvedp.cn/gtydfkwaue.html

Java: String.join(", ", list)
来源：http://hz.tanke756.top/gtrzaspiql.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhongyouzk.top/gtbnzjgoau.html

Ruby: arr.join(", ")
来源：http://hz.xziqi.cn/gtolklrfyv.html

C#:   string.Join(", ", list)
来源：http://hz.hongshengwenyu.top/gtzddxbgbt.html

================================================================================
来源：http://hz.zhoulong.xyz/gtssqhuzui.html

E. 字符串处理
来源：http://hz.svipenyu.cn/gtxkdukhdx.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtoghjjovk.html

[E01] 拼接字符串
来源：http://hz.52xcode.cn/gteardvygh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gaohongyu789.top/gtkafbfphf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.chenjidiqi.icu/gtnjmpvzsd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fengsongda.top/gtmjhpoglf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.wangdashe.top/gtkmzuppon.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hnqzz.top/gtekalkmgj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj20258888.top/gtzbgcegfk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yongpay.top/gtgrmyiphz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.iojbl.cn/gtfwcfunig.html

[E02] 重复字符串
来源：http://hz.haohaochexian.top/gtydooopkk.html

Py:   "ab" * 3
来源：http://hz.jinqigfzy.top/gtrffgmxcb.html

PHP:  str_repeat("ab", 3);
来源：http://hz.shzxlz.cn/gtratkqstk.html

JS:   "ab".repeat(3)
来源：http://hz.havefunace.top/gttaneqvtz.html

TS:   "ab".repeat(3)
来源：http://hz.tianlin.xyz/gtkebzekcy.html

Java: "ab".repeat(3)
来源：http://hz.zhoulong.xyz/gtznwwulfu.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shuidangran.top/gtgescwbjf.html

Ruby: "ab" * 3
来源：http://hz.zhengqikj.top/gtahomvfrc.html


<!-- 参考信息 -->