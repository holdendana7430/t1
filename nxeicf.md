代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nwbrower.top/gtkeutsuzi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhaomingkeji.xyz/gtsobjzupz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.vqdsnc.cn/gtadljyojk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.kuanghao11.cn/gtawxabcio.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.fzhhl.top/gtwgibwnat.html

Go:   func add(a, b int) int
来源：http://hz.iojbl.cn/gtpssaogny.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.bjfxy.top/gtnxwpeplf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sweek.top/gtsknxgrjx.html

[C14] 泛型函数
来源：http://hz.meibo888.top/gtrhocyiax.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sysykeji.top/gttjnslhzm.html

PHP:  // 无泛型
来源：http://hz.sysykeji.top/gtvwrrtiap.html

JS:   // 无泛型
来源：http://hz.jinqigfzy.top/gtlmyqxrbv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shangyingyoupin.top/gtwqdizuga.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shuidangran.top/gtdymrfebe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.0kj1m.cn/gtwrckrovb.html

Ruby: # 无泛型
来源：http://hz.shzxlz.cn/gtwsrthuoi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.birdmap.top/gtnwvhphts.html

[C15] 解构 / 展开参数
来源：http://hz.yj20258888.top/gtiwtkwcjv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shuidangran.top/gtelfxjnkw.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xziqi.cn/gtbtnhojlc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.tianlin.xyz/gtqoneovyo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.c1oappe.top/gtraosffpz.html

Java: // 无解构
来源：http://hz.gzhubu.top/gtimoufuoh.html

Go:   // 无解构
来源：http://hz.chenjidiqi.icu/gtmieidpud.html

Ruby: a, b = pair
来源：http://hz.nwbrower.top/gthvxjczrp.html

C#:   var (a, b) = pair;
来源：http://hz.sysykeji.top/gtwypiynaz.html

[C16] 函数 / 方法重载
来源：http://hz.zhongyouzk.top/gtizxahtfp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.0kj1m.cn/gtlidsambg.html

PHP:  // 无重载
来源：http://hz.dianchejie.cn/gtxmvvbcqr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gogol.net.cn/gtbxhjjdag.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj20258.top/gttxrzmzoi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.snrcjt.cn/gtesbfgiwx.html

Go:   // 无重载：用不同函数名
来源：http://hz.haohaochexian.top/gtgzquofnx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hnqzz.top/gtuojmcwfb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.meibo888.top/gtaivzftku.html

================================================================================
来源：http://hz.vqdsnc.cn/gthwfzlzti.html

D. 数组 / 列表 / 集合
来源：http://hz.gzhubu.top/gtdxfvwfmh.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtxgiknhce.html

[D01] 创建数组 / 列表
来源：http://hz.xingfuxueyuan.xyz/gtgpttqkzg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.52xcode.cn/gtjxxaeynj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hnxiangtu.top/gtvnxrushq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xylfe.cn/gtibyezcnh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ivvv.top/gticoshtfl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ehwqpu.com/gtjamdnkvo.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xinyue.icu/gtarsawwgw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.gotoacloud.top/gtzacltfca.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.quarkkingdee.top/gtvjjecphh.html

[D02] 追加元素到末尾
来源：http://hz.nanxuanxn.top/gtcccskwcg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.aizwys.cn/gtjqiexina.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.meibo888.top/gtvzszfnmv.html

JS:   arr.push(4);
来源：http://hz.meibo888.top/gtlsydyzgd.html

TS:   arr.push(4);
来源：http://hz.andypj.xyz/gtwbehvrow.html

Java: list.add(4);
来源：http://hz.guannengcc.top/gtfikogkih.html

Go:   arr = append(arr, 4)
来源：http://hz.chenjidiqi.icu/gteihluzku.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hongshengwenyu.top/gtcvhjdpgi.html

C#:   list.Add(4);
来源：http://hz.birdmap.top/gtlfmshqpg.html

[D03] 在指定位置插入元素
来源：http://hz.xuetiantiany.cn/gtcjcduvlj.html

Py:   arr.insert(0, 0)
来源：http://hz.jqgfzy.top/gtoztgyucm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yj20258888.top/gtapnaziql.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xinyue.icu/gtrmnuzmmz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.fengsongda.top/gtxqnodekr.html

Java: list.add(0, 0);
来源：http://hz.jlsjyb.cn/gtsesfzyhp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cheryme.top/gtqcavqqfh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tanke756.top/gtfzsdazbg.html

C#:   list.Insert(0, 0);
来源：http://hz.hnxiangtu.top/gtlqdbxemm.html

[D04] 删除元素
来源：http://hz.smart0.xyz/gtxxppkhqm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hywenlv.cn/gtyaaghxhb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhijiandao.cn/gtledztkua.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ybcxt.top/gtnwhoqxwo.html

TS:   arr.splice(0, 1);
来源：http://hz.haohaochexian.top/gtdstoppct.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xylfe.cn/gtqixxiwnt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shzxlz.cn/gtzuakzzmv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gotoacloud.top/gtccriolag.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.0kj1m.cn/gttaoujzbi.html

[D05] 访问与修改元素
来源：http://hz.zhengqikj.top/gtqkeirgdf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.smart0.xyz/gtkkquhtbh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yonumen.top/gttbvifgwi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ywan-chungtsiang.top/gtrbyxpuon.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nanxinkj.top/gtwafeokwg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ydjk.org.cn/gtcoutqgmt.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yueranfly.top/gtzzdbtrwo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuxming.cn/gtqprrwcxs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cucudq.cn/gtyutovjhr.html

[D06] 数组长度
来源：http://hz.sysykeji.top/gttiggvhft.html

Py:   len(arr)
来源：http://hz.dianchejie.cn/gteedkaius.html

PHP:  count($arr);
来源：http://hz.jinghuilouyu.cn/gtryvbhpsv.html

JS:   arr.length
来源：http://hz.sxryk.cn/gthmgzmbwc.html

TS:   arr.length
来源：http://hz.cqqwz.cn/gtbthwjoij.html

Java: list.size();
来源：http://hz.kuanghao11.cn/gtdftwkegt.html

Go:   len(arr)
来源：http://hz.xuetiantiany.cn/gtltbbnsmv.html

Ruby: arr.length; arr.size
来源：http://hz.chenlongwang.top/gthwsotlnc.html

C#:   list.Count;
来源：http://hz.jinqigufen.top/gtzyslviuo.html

[D07] 切片 / 取子数组
来源：http://hz.feifeiyinyue.top/gtxrnwqoko.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shzxlz.cn/gtpifnimnq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cucudq.cn/gthijnkmin.html

JS:   arr.slice(1, 4);
来源：http://hz.0kj1m.cn/gtvskjdyhw.html

TS:   arr.slice(1, 4);
来源：http://hz.kuanghao11.cn/gtrziutknk.html

Java: list.subList(1, 4);
来源：http://hz.iojbl.cn/gtnqzbsoou.html

Go:   arr[1:4]
来源：http://hz.mhx1999.top/gtrdoongek.html

Ruby: arr[1, 3]
来源：http://hz.cdnleiting.top/gtmxzwvgbt.html

C#:   list.GetRange(1, 3);
来源：http://hz.jlsjyb.cn/gtfytytvsk.html

[D08] 合并两个数组
来源：http://hz.cheryme.top/gtjtackozb.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhoulong.xyz/gtysghhvun.html

PHP:  array_merge($a, $b);
来源：http://hz.zhixingplan.top/gtmekrfrxu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ppjwa.cn/gtxrxirmlx.html

TS:   [...a, ...b];
来源：http://hz.zhijiandao.cn/gtxinjhdmz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhaomingkeji.xyz/gtwbyrssmu.html

Go:   append(a, b...)
来源：http://hz.yuanzhike.top/gtqkvhqpva.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cashguo.top/gthqwpbstg.html

C#:   a.Concat(b).ToList()
来源：http://hz.ydjk.org.cn/gtvrujcyib.html

[D09] 排序（升序）
来源：http://hz.yanxiufei.cn/gthuvdbucb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258888.top/gtdbkauyrv.html

PHP:  sort($arr);
来源：http://hz.yanxiufei.cn/gtmhcvgucx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yonumen.top/gtlsrehrvv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xinyue.icu/gtixzlqzhe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hnqzz.top/gtjsehfwqu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yanxiufei.cn/gtvfluhvsf.html

Ruby: arr.sort
来源：http://hz.ydjk.org.cn/gtwsbxzpbt.html

C#:   list.Sort();
来源：http://hz.havefunace.top/gtwkitmcmf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sysykeji.top/gtpyyyusbj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhiwuduotai.top/gtbgdzdema.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gtvgycjweo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.vqdsnc.cn/gtppsomqgb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhaomingkeji.xyz/gtxuqosfoj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.daxiang520.top/gtrgqxkwtu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.nwbrower.top/gtrkhpunof.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.snrcjt.cn/gttwenfuhi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.guannengcc.top/gtihsesyyw.html

[D11] 反转数组
来源：http://hz.sweek.top/gtwsxwkphy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ehwqpu.com/gtsxuvqijp.html

PHP:  array_reverse($arr);
来源：http://hz.xingfuxueyuan.xyz/gtxryauikv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.birdmap.top/gtfkefzebq.html

TS:   [...arr].reverse();
来源：http://hz.9152youxi.cn/gtelptxbmr.html

Java: Collections.reverse(list);
来源：http://hz.tian-w.cn/gtpxtovyjd.html

Go:   slices.Reverse(arr)
来源：http://hz.jianghu66.top/gtvumvgiqh.html

Ruby: arr.reverse
来源：http://hz.shzxlz.cn/gtqombggfs.html

C#:   list.Reverse();
来源：http://hz.zhixingplan.top/gtyflwsytc.html

[D12] 查找元素下标
来源：http://hz.gogol.net.cn/gtdsxiqisk.html

Py:   arr.index(x);  x in arr
来源：http://hz.jinghuilouyu.cn/gtcsvbmlai.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.daria6918.cn/gtcxjsvntd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gogol.net.cn/gtlxgaezkf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yanxiufei.cn/gtcozzoezf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.daxiang520.top/gtkjjpmyaj.html

Go:   slices.Index(arr, x)
来源：http://hz.snrcjt.cn/gtlhojzhaw.html

Ruby: arr.index(x)
来源：http://hz.guowangkeji.top/gticbnkyvq.html

C#:   list.IndexOf(x);
来源：http://hz.yueranfly.top/gtaqgtynsh.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jqgfzy.top/gtlrxwquqj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jqgufenzy.top/gtuccmyhfb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenjidiqi.icu/gtwfuenofn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hysaishi.cn/gtwhoxdcya.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daxiang520.top/gtynszeooq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.aibaodan.cn/gtwhhnfbsz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xziqi.cn/gtrwpwiepw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.316326.xyz/gtuhgbqhiw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ywan-chungtsiang.top/gtkbadvbkc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.guannengcc.top/gtlgcazipp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ehwqpu.com/gtlyiolmqi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jiagoushi.top/gtrrqhtjux.html

JS:   arr.map(x => x * 2)
来源：http://hz.c1oappe.top/gtuiydijch.html

TS:   arr.map(x => x * 2)
来源：http://hz.tianlin.xyz/gtmwcwgdkr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jianghu66.top/gtxueqmccl.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gtqiojpjex.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cucudq.cn/gtijzzdtuq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gzhubu.top/gtdbtdzlrh.html

[D15] 去重
来源：http://hz.gotoacloud.top/gtxyhmjzer.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nwbrower.top/gtdohgomfr.html

PHP:  array_unique($arr);
来源：http://hz.vqdsnc.cn/gttsdscavn.html

JS:   [...new Set(arr)]
来源：http://hz.ywan-chungtsiang.top/gtbzctqdzb.html

TS:   [...new Set(arr)]
来源：http://hz.ivvv.top/gtajlyrjqu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.fengsongda.top/gtnplajagp.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinyuanbaomall.cn/gtzhwndikp.html

Ruby: arr.uniq
来源：http://hz.dashuyun.cn/gthblpacyn.html

C#:   list.Distinct().ToList()
来源：http://hz.iojbl.cn/gtxjmurswi.html

[D16] 求和与平均值
来源：http://hz.gaohongyu789.top/gtlvufnpqi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.0kj1m.cn/gtvxkbcoxj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pycfn.com/gtiitqvtcu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hfpthk.cn/gtzimcvrds.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nanxuanxn.top/gtggqmczge.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zdqjudy.top/gtnhwzxpeg.html

Go:   // 手写循环累加
来源：http://hz.yonumen.top/gtuflluwpx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sufxvd.cn/gtwijhjmgd.html

C#:   list.Sum();  list.Average()
来源：http://hz.sufxvd.cn/gtfgqdeyvl.html

[D17] 最大值与最小值
来源：http://hz.iojbl.cn/gtzvmqkqqn.html

Py:   max(arr);  min(arr)
来源：http://hz.daria6918.cn/gtxswdxnth.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhaomingkeji.xyz/gtklqyljni.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yj20258888.top/gtpjlrincj.html

TS:   Math.max(...arr);
来源：http://hz.ybcxt.top/gtlkrrqnlr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gogol.net.cn/gtidskeqpr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ywan-chungtsiang.top/gtqipjvhzc.html

Ruby: arr.max;  arr.min
来源：http://hz.gaohongyu789.top/gtootimhcu.html

C#:   list.Max();  list.Min()
来源：http://hz.chenjidiqi.icu/gtmqibpegy.html

[D18] 扁平化嵌套数组
来源：http://hz.dianchejie.cn/gthrsclhcz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.quarkkingdee.top/gtemajuhbs.html

PHP:  array_merge(...$nested);
来源：http://hz.xuanzx.com/gtlivckwtp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.nwbrower.top/gtidgncmyd.html

TS:   nested.flat();
来源：http://hz.gotoacloud.top/gtryylybuo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cashguo.top/gtxhqfqkvq.html

Go:   // 手写双层循环
来源：http://hz.jinyuanbaomall.cn/gtiziefptq.html

Ruby: nested.flatten
来源：http://hz.dianchejie.cn/gtgoafvrbv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hfpthk.cn/gtywnsyoyr.html

[D19] 按字段分组
来源：http://hz.ywan-chungtsiang.top/gtbztrrqxc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.redwolf501.top/gtgvwfcyha.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yangfankeji.com/gtqqbszvmg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhijiandao.cn/gttrjphkev.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.fengsongda.top/gtxmuqluoo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.mhx1999.top/gthhveujwy.html

Go:   // 手写 map[string][]T
来源：http://hz.hfpthk.cn/gtabdhjxnb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.fengsongda.top/gtsnqhjswh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ehwqpu.com/gtwcstgvrj.html

[D20] 统计每个元素出现次数
来源：http://hz.jinqigufen.top/gtachbnnps.html

Py:   Counter(arr)
来源：http://hz.jyoumei.cn/gtracbwrrc.html

PHP:  array_count_values($arr);
来源：http://hz.xinyue.icu/gtrmhnyxde.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.mhx1999.top/gtdzmriufy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xziqi.cn/gthraroqkk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhiwuduotai.top/gtwgdhiqvx.html

Go:   // 手写 map[T]int
来源：http://hz.jyoumei.cn/gtjipjbitd.html

Ruby: arr.tally
来源：http://hz.ydzc1.top/gtcvqyzzwy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yanxiufei.cn/gtxyiyeqzs.html

[D21] 判断是否包含某元素
来源：http://hz.zhixingplan.top/gtzxaexlze.html

Py:   x in arr
来源：http://hz.quarkkingdee.top/gtjdmmxzwc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhiwuduotai.top/gtypbwscdn.html

JS:   arr.includes(x)
来源：http://hz.xuetiantiany.cn/gtzpqjdreh.html

TS:   arr.includes(x)
来源：http://hz.iojbl.cn/gttugpwsvm.html

Java: list.contains(x)
来源：http://hz.shzxlz.cn/gtqrowscmr.html

Go:   slices.Contains(arr, x)
来源：http://hz.fzhhl.top/gtphhertba.html

Ruby: arr.include?(x)
来源：http://hz.c1oappe.top/gtsjscfpwv.html

C#:   list.Contains(x)
来源：http://hz.quarkkingdee.top/gtnqwrihyj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cqqwz.cn/gtxwufends.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ppjwa.cn/gtvgjwsuic.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.mhx1999.top/gtzrjpynuv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.aibaodan.cn/gtsookfhzd.html

TS:   [...arr];
来源：http://hz.bjfxy.top/gtrlyueleg.html

Java: new ArrayList<>(list);
来源：http://hz.jqgfzy.top/gtzhdxiqge.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nwbrower.top/gtyfoirjmq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.9152youxi.cn/gtyizuiwqu.html

C#:   new List<int>(list);
来源：http://hz.aizwys.cn/gtraomqzkr.html

[D23] reduce 累积计算
来源：http://hz.jinqigfzy.top/gtrctvkmbk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.meibo888.top/gtqpwfblpt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.gotoacloud.top/gtgqhuewim.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cucudq.cn/gtfdhhpgaj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tian-w.cn/gtrczfcdto.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.pengpengdd.cyou/gtunaliytg.html

Go:   // 手写循环
来源：http://hz.feifeiyinyue.top/gtjqehyvgq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenjidiqi.icu/gtztxyqbqi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.52xcode.cn/gtryrzxywp.html

[D24] 字典 / Map 基本操作
来源：http://hz.gzhubu.top/gtrspmltdo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.9152youxi.cn/gtyypjrnmc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cheryme.top/gtrxjtexmp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xinyue.icu/gtoggtabbg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.mhx1999.top/gtyisbbgdb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ppjwa.cn/gtzqvmusjg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.tianlin.xyz/gtsrkoqyno.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhongyouzk.top/gtdtfctnhz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.havefunace.top/gtqdbjrnkk.html

[D25] Set 集合去重与交并差
来源：http://hz.yonumen.top/gtfowmhebw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.aizwys.cn/gtjadhjcff.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.wangshuangyany.cn/gtfmelybsa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ehwqpu.com/gtftqnprzk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ehwqpu.com/gttpvepgdx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhengqikj.top/gtrdwrdddq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zdqjudy.top/gtychmxyzu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.dashuyun.cn/gtznbtpuzb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hysaishi.cn/gticcdxwmd.html

[D26] 数组转字符串
来源：http://hz.ybcxt.top/gttqqkopuu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hywenlv.cn/gtswcxizso.html

PHP:  implode(", ", $arr);
来源：http://hz.cqqwz.cn/gtfcncomiu.html

JS:   arr.join(", ")
来源：http://hz.jinqigfzy.top/gtgubcndjg.html

TS:   arr.join(", ")
来源：http://hz.yongpay.top/gtvyxjspoi.html

Java: String.join(", ", list)
来源：http://hz.yj20258888.top/gtvsleiumz.html

Go:   strings.Join(strs, ", ")
来源：http://hz.tianlin.xyz/gtrazrusaz.html

Ruby: arr.join(", ")
来源：http://hz.jinqigfzy.top/gtepgrrhyo.html

C#:   string.Join(", ", list)
来源：http://hz.chenjidiqi.icu/gtuochrfav.html

================================================================================
来源：http://hz.yj202588.top/gtvntsziob.html

E. 字符串处理
来源：http://hz.aibaodan.cn/gtatmasbsp.html

================================================================================
来源：http://hz.chenlongwang.top/gtkollrzub.html

[E01] 拼接字符串
来源：http://hz.zhoulong.xyz/gtmqbczwem.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.smart0.xyz/gtixvuitol.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinqigufen.top/gtwtvnkgto.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuanzhike.top/gtloxxsxlz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gtofbwjfwz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jianghu66.top/gtbhejkoxo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yvedp.cn/gtffstwcjc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gaohongyu789.top/gtigytazfs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zycfv.cn/gtwdevruat.html

[E02] 重复字符串
来源：http://hz.fengsongda.top/gtiwfosbed.html

Py:   "ab" * 3
来源：http://hz.birdmap.top/gthldklnmd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hfpthk.cn/gtookqoqug.html

JS:   "ab".repeat(3)
来源：http://hz.ppjwa.cn/gtrikbtwnm.html

TS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gtxixzelez.html

Java: "ab".repeat(3)
来源：http://hz.hfpthk.cn/gtqluafavd.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.gogol.net.cn/gtqecsfndx.html

Ruby: "ab" * 3
来源：http://hz.zhaomingkeji.xyz/gtcbacpccn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xylfe.cn/gtdnvqzmas.html

[E03] 截取子串
来源：http://hz.aizwys.cn/gtfwhkruzd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.iojbl.cn/gttmllahvh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cdnleiting.top/gtijwoxvbr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinqigfzy.top/gtqbxgqxat.html

TS:   s.slice(1, 4)
来源：http://hz.svipenyu.cn/gtqiyetcmh.html

Java: s.substring(1, 4)
来源：http://hz.nwbrower.top/gtmpwsxuhu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhiwuduotai.top/gtixjwmnlc.html


<!-- 参考信息 -->