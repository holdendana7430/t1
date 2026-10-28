代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://hz.yj20258888.top/gtffykfqse.html

Ruby: -> { puts "run" }.call
来源：http://hz.yvedp.cn/gtspdqoxki.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xinyue.icu/gtnifokcyl.html

[C13] 类型声明 / 类型注解
来源：http://hz.hfpthk.cn/gthbwvldmj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.dashuyun.cn/gtqvavggzs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shuidangran.top/gtxwbsckvt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xingfuxueyuan.xyz/gtmzygtpoz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hammf.cn/gtooycjnne.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtbkfxmncz.html

Go:   func add(a, b int) int
来源：http://hz.zdqjudy.top/gtlxyyqmhf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.chenzaomai.com/gtbvdhgdku.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jqgfzy.top/gtmspdacls.html

[C14] 泛型函数
来源：http://hz.jianghu66.top/gtaijjtebw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xuanzx.com/gtiagcpwip.html

PHP:  // 无泛型
来源：http://hz.zhongyouzk.top/gtyzxmhswj.html

JS:   // 无泛型
来源：http://hz.hfpthk.cn/gtiomntoii.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yj20258888.top/gtbtkbelda.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ppjwa.cn/gtuwesfget.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.andypj.xyz/gttsqvoget.html

Ruby: # 无泛型
来源：http://hz.ywan-chungtsiang.top/gtqomstapm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.andypj.xyz/gthozeuzrf.html

[C15] 解构 / 展开参数
来源：http://hz.gotoacloud.top/gtdjyoxdbt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cucudq.cn/gtvzjynghx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hywenlv.cn/gtqgnluelz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cucudq.cn/gtlzgsihlu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.bjfxy.top/gtqvxustbw.html

Java: // 无解构
来源：http://hz.vqdsnc.cn/gthjbvphzv.html

Go:   // 无解构
来源：http://hz.jinghuilouyu.cn/gtwwqhglix.html

Ruby: a, b = pair
来源：http://hz.yj202588.top/gtkzdcjijp.html

C#:   var (a, b) = pair;
来源：http://hz.yj20258.top/gtzmdqucws.html

[C16] 函数 / 方法重载
来源：http://hz.zhijiandao.cn/gtzgysmtly.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hfpthk.cn/gtkiglgvyh.html

PHP:  // 无重载
来源：http://hz.yonumen.top/gtcxshslla.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hammf.cn/gtynbqvxlc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ybcxt.top/gtjfecmsrg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.iojbl.cn/gtoaqihghw.html

Go:   // 无重载：用不同函数名
来源：http://hz.snrcjt.cn/gtptqizili.html

Ruby: # 无重载：靠动态参数
来源：http://hz.wangshuangyany.cn/gtklhasbhq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xuanzx.com/gtucltlcii.html

================================================================================
来源：http://hz.ppjwa.cn/gtfdiafmtm.html

D. 数组 / 列表 / 集合
来源：http://hz.chenlongwang.top/gtjxjvbhsg.html

================================================================================
来源：http://hz.yvedp.cn/gtcdvfmxhc.html

[D01] 创建数组 / 列表
来源：http://hz.ywan-chungtsiang.top/gterljfbbc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yuanzhike.top/gtkvlrjbgy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sufxvd.cn/gtsxbvjpvm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhengqikj.top/gtadzlrwhv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hongshengwenyu.top/gtrmkyavzq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.quarkkingdee.top/gtmemftevz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hnqzz.top/gtyqbgdyfp.html

Ruby: arr = [1, 2, 3]
来源：http://hz.kuanghao11.cn/gtsotqttlx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jinghuilouyu.cn/gttabctfsd.html

[D02] 追加元素到末尾
来源：http://hz.jinghuilouyu.cn/gtkhktwzma.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.nanxuanxn.top/gtelquuytd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.svipenyu.cn/gtmaujjwxu.html

JS:   arr.push(4);
来源：http://hz.chenlongwang.top/gthtbizhti.html

TS:   arr.push(4);
来源：http://hz.nanxuanxn.top/gtsuntolen.html

Java: list.add(4);
来源：http://hz.0kj1m.cn/gtpavhlczr.html

Go:   arr = append(arr, 4)
来源：http://hz.cheryme.top/gthcpaqzlz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.snrcjt.cn/gtkwnsbpom.html

C#:   list.Add(4);
来源：http://hz.xinyue.icu/gtteimghyd.html

[D03] 在指定位置插入元素
来源：http://hz.yanxiufei.cn/gtiwtbmukx.html

Py:   arr.insert(0, 0)
来源：http://hz.zhiwuduotai.top/gtwvrxxbrg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xziqi.cn/gtifpqvblr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hammf.cn/gtwydfenre.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.wangshuangyany.cn/gtbhisgsio.html

Java: list.add(0, 0);
来源：http://hz.iojbl.cn/gtshfascpz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hammf.cn/gttstfgsex.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.svipenyu.cn/gtzqxqkiic.html

C#:   list.Insert(0, 0);
来源：http://hz.cashguo.top/gtioxmxzwi.html

[D04] 删除元素
来源：http://hz.jinghuilouyu.cn/gtbsgyqnhm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cucudq.cn/gtqtgheums.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yuxming.cn/gtehroxtag.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jyoumei.cn/gtwnnuharg.html

TS:   arr.splice(0, 1);
来源：http://hz.guowangkeji.top/gtqgpefpdf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zdqjudy.top/gtklouxtrv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ppjwa.cn/gtrbjbhfty.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.haohaochexian.top/gtrhswuxfc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhongyouzk.top/gtmciobbzx.html

[D05] 访问与修改元素
来源：http://hz.yj20258.top/gttoigwvbl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xziqi.cn/gtyrputydk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cheryme.top/gtlkfrfdnk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ppjwa.cn/gtcjzwdmus.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.wangdashe.top/gtvcneiemj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ehwqpu.com/gteknjgzmd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.kuanghao11.cn/gtzjmowocs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.meibo888.top/gttospxrou.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shanyushiyangkeji.top/gtjggawfse.html

[D06] 数组长度
来源：http://hz.shzxlz.cn/gtjudtusfr.html

Py:   len(arr)
来源：http://hz.jqgfzy.top/gtywmtqusc.html

PHP:  count($arr);
来源：http://hz.yuanzhike.top/gtadmfgcff.html

JS:   arr.length
来源：http://hz.guowangkeji.top/gtlbkxpxbu.html

TS:   arr.length
来源：http://hz.nwbrower.top/gtvhmjxdrj.html

Java: list.size();
来源：http://hz.ehwqpu.com/gtpvpnuerz.html

Go:   len(arr)
来源：http://hz.shanyushiyangkeji.top/gtbslaggwu.html

Ruby: arr.length; arr.size
来源：http://hz.dashuyun.cn/gtukquqbam.html

C#:   list.Count;
来源：http://hz.316326.xyz/gtdhfixzyf.html

[D07] 切片 / 取子数组
来源：http://hz.zhixingplan.top/gtcpjqoori.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shanyushiyangkeji.top/gtpylvdhfb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xuetiantiany.cn/gtapkexzez.html

JS:   arr.slice(1, 4);
来源：http://hz.pycfn.com/gtftgdhweq.html

TS:   arr.slice(1, 4);
来源：http://hz.xuetiantiany.cn/gtgrupluez.html

Java: list.subList(1, 4);
来源：http://hz.yangfankeji.com/gtedhnqfqh.html

Go:   arr[1:4]
来源：http://hz.andypj.xyz/gtmcgulctx.html

Ruby: arr[1, 3]
来源：http://hz.nwbrower.top/gtfgzywohn.html

C#:   list.GetRange(1, 3);
来源：http://hz.jinqigufen.top/gtjihkqajc.html

[D08] 合并两个数组
来源：http://hz.xuanzx.com/gtlyzgozvi.html

Py:   a + b;  a.extend(b)
来源：http://hz.jlsjyb.cn/gtxkepscpj.html

PHP:  array_merge($a, $b);
来源：http://hz.havefunace.top/gtdgjgrzlk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gotoacloud.top/gtocxdxpzg.html

TS:   [...a, ...b];
来源：http://hz.ydjk.org.cn/gtdcohbmwp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cqqwz.cn/gtkngriewx.html

Go:   append(a, b...)
来源：http://hz.bjfxy.top/gtpgrdpjth.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xuanzx.com/gtqbtetsrk.html

C#:   a.Concat(b).ToList()
来源：http://hz.pengpengdd.cyou/gthtdgsspg.html

[D09] 排序（升序）
来源：http://hz.xziqi.cn/gtdvcbriem.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cheryme.top/gtltmhvbex.html

PHP:  sort($arr);
来源：http://hz.yuanzhike.top/gtcbklqmmx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xuetiantiany.cn/gtrbnybvma.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shangyingyoupin.top/gtoigdpqct.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.vqdsnc.cn/gtyvwbfbhr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jinqigfzy.top/gtoiqsdhhw.html

Ruby: arr.sort
来源：http://hz.c1oappe.top/gtcsfcblmx.html

C#:   list.Sort();
来源：http://hz.yonumen.top/gthplmflzm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.iojbl.cn/gtzjmgipyg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yj20258.top/gtwnftvwra.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shzxlz.cn/gthghahmtm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hammf.cn/gtdqlbbkuz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xingfuxueyuan.xyz/gtjxarhwin.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hysaishi.cn/gtyblogxcl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhixingplan.top/gtvafzbvmv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cashguo.top/gteroayxrv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.haohaochexian.top/gtyaucczcp.html

[D11] 反转数组
来源：http://hz.nwbrower.top/gtonwdtoqf.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.fengsongda.top/gtfdphpqrt.html

PHP:  array_reverse($arr);
来源：http://hz.havefunace.top/gthexongnm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.9152youxi.cn/gtoetstzlk.html

TS:   [...arr].reverse();
来源：http://hz.daria6918.cn/gtfjbcmxwf.html

Java: Collections.reverse(list);
来源：http://hz.gogol.net.cn/gtmvmjjvap.html

Go:   slices.Reverse(arr)
来源：http://hz.tian-w.cn/gtynioqvoq.html

Ruby: arr.reverse
来源：http://hz.dianchejie.cn/gtimodduia.html

C#:   list.Reverse();
来源：http://hz.pengpengdd.cyou/gtapmocdij.html

[D12] 查找元素下标
来源：http://hz.mhx1999.top/gtgloccmhm.html

Py:   arr.index(x);  x in arr
来源：http://hz.jqgfzy.top/gtzvbpmcdm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenjidiqi.icu/gtynxecjrm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.andypj.xyz/gtwumkcbzq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gzhubu.top/gtaqzyrivg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhaomingkeji.xyz/gthwkaizvy.html

Go:   slices.Index(arr, x)
来源：http://hz.svipenyu.cn/gtainflnry.html

Ruby: arr.index(x)
来源：http://hz.redwolf501.top/gtsjpygxui.html

C#:   list.IndexOf(x);
来源：http://hz.zdqjudy.top/gtqwjhztll.html

[D13] 过滤（保留满足条件的）
来源：http://hz.pycfn.com/gtnbqcvcyp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yuanzhike.top/gtxjmgrpbt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhoulong.xyz/gtajfxaasi.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhongyouzk.top/gtkaijjkue.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xuanzx.com/gtnphmtjhm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ydjk.org.cn/gtmyfgbfiw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yuxming.cn/gtdtzpsgvc.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ydzc1.top/gtmceojmhb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cucudq.cn/gteaxybift.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jlsjyb.cn/gtaelugrck.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ydzc1.top/gtxvfojsgl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yuanzhike.top/gtkbbxdrlb.html

JS:   arr.map(x => x * 2)
来源：http://hz.haohaochexian.top/gtizbihcfe.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhoulong.xyz/gtcwmtnwxl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yj20258.top/gtmexpzzui.html

Go:   // 手写循环
来源：http://hz.cashguo.top/gttarpelxc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yuxming.cn/gtileoneys.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.svipenyu.cn/gtfgyjuhzg.html

[D15] 去重
来源：http://hz.jqgfzy.top/gtzygsdawh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jianghu66.top/gtmvproido.html

PHP:  array_unique($arr);
来源：http://hz.chenlongwang.top/gtolfdtxjq.html

JS:   [...new Set(arr)]
来源：http://hz.tianlin.xyz/gtlleupaaf.html

TS:   [...new Set(arr)]
来源：http://hz.xziqi.cn/gteqbbyvnw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xingfuxueyuan.xyz/gtlbkmafxx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jianghu66.top/gtbhxvwbye.html

Ruby: arr.uniq
来源：http://hz.jinqigfzy.top/gtotvvxgtg.html

C#:   list.Distinct().ToList()
来源：http://hz.birdmap.top/gtocadguth.html

[D16] 求和与平均值
来源：http://hz.tianlin.xyz/gthjjbwhmo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yvedp.cn/gtizsufwip.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj202588.top/gtrmzcctdk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnxiangtu.top/gtlkciqpmn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtarhxivct.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.wangdashe.top/gtfxtqbxjy.html

Go:   // 手写循环累加
来源：http://hz.xinyue.icu/gtwphtjcur.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.daria6918.cn/gtpzhrxeud.html

C#:   list.Sum();  list.Average()
来源：http://hz.svipenyu.cn/gttgkpuwxn.html

[D17] 最大值与最小值
来源：http://hz.yj202588.top/gtcnzcycae.html

Py:   max(arr);  min(arr)
来源：http://hz.aizwys.cn/gtiwfykmxf.html

PHP:  max($arr);  min($arr);
来源：http://hz.hnqzz.top/gtmxfziaxg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shangyingyoupin.top/gtfwpzxyak.html

TS:   Math.max(...arr);
来源：http://hz.daria6918.cn/gttqrejyug.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.daria6918.cn/gtcmjrpqjc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhengqikj.top/gteymctmmk.html

Ruby: arr.max;  arr.min
来源：http://hz.hfpthk.cn/gtyxxtqfal.html

C#:   list.Max();  list.Min()
来源：http://hz.gotoacloud.top/gtfecudxge.html

[D18] 扁平化嵌套数组
来源：http://hz.316326.xyz/gtbhjovixj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.fengsongda.top/gtpekrrwuj.html

PHP:  array_merge(...$nested);
来源：http://hz.jianghu66.top/gtuzopsgtl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cashguo.top/gtzpimyspx.html

TS:   nested.flat();
来源：http://hz.xylfe.cn/gtghgvybwr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.0kj1m.cn/gtmrexfqni.html

Go:   // 手写双层循环
来源：http://hz.andypj.xyz/gtlythghoj.html

Ruby: nested.flatten
来源：http://hz.havefunace.top/gtvlaeydzc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinyuanbaomall.cn/gtcrjmokxu.html

[D19] 按字段分组
来源：http://hz.yuxming.cn/gtidtnawii.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhijiandao.cn/gtmwoziiql.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cqqwz.cn/gtsmgkzcnv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.smart0.xyz/gtmggolgww.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ybcxt.top/gtviwrqare.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.aizwys.cn/gtakwvdwja.html

Go:   // 手写 map[string][]T
来源：http://hz.hfpthk.cn/gtqyozrske.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gogol.net.cn/gtweuxufpp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jyoumei.cn/gtnepblaqy.html

[D20] 统计每个元素出现次数
来源：http://hz.nanxinkj.top/gtzdpylhov.html

Py:   Counter(arr)
来源：http://hz.cashguo.top/gtujbggnmb.html

PHP:  array_count_values($arr);
来源：http://hz.yangfankeji.com/gtihlhvecn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shzxlz.cn/gtmtysvmta.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangshuangyany.cn/gtarjpndzi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.0kj1m.cn/gtslyugnjf.html

Go:   // 手写 map[T]int
来源：http://hz.yongpay.top/gtfiucrhin.html

Ruby: arr.tally
来源：http://hz.zhoulong.xyz/gtonsxpzgc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yanxiufei.cn/gtdsukrjrd.html

[D21] 判断是否包含某元素
来源：http://hz.aizwys.cn/gtsbaaysal.html

Py:   x in arr
来源：http://hz.yuxming.cn/gtmvqqehzp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.dianchejie.cn/gtkjyuriuk.html

JS:   arr.includes(x)
来源：http://hz.zhengqikj.top/gtrvboruai.html

TS:   arr.includes(x)
来源：http://hz.snrcjt.cn/gtqrzgbgwp.html

Java: list.contains(x)
来源：http://hz.cqqwz.cn/gtpztfvjrx.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhixingplan.top/gtnqwafnrg.html

Ruby: arr.include?(x)
来源：http://hz.jqgufenzy.top/gtynkkgegq.html

C#:   list.Contains(x)
来源：http://hz.nwbrower.top/gtyluqdddn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cucudq.cn/gtjsggafws.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sufxvd.cn/gtmtloqcmd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hfpthk.cn/gtymjnmvbl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jqgfzy.top/gtsmaazdlu.html

TS:   [...arr];
来源：http://hz.chenlongwang.top/gtrdynnwxg.html

Java: new ArrayList<>(list);
来源：http://hz.aizwys.cn/gtjftsddvi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.dianchejie.cn/gtiqdbupqh.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhiwuduotai.top/gtcpdsvjzs.html

C#:   new List<int>(list);
来源：http://hz.zhiwuduotai.top/gtbggsyhfh.html

[D23] reduce 累积计算
来源：http://hz.gaohongyu789.top/gtdnqdfwfs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.chenzaomai.com/gthbhfysfq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.shangyingyoupin.top/gtjmzhyyhz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gtezqvrzmq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.snrcjt.cn/gtnvhcrdks.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.quarkkingdee.top/gtaaagwjmw.html

Go:   // 手写循环
来源：http://hz.zhaomingkeji.xyz/gtmorajrlo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.snrcjt.cn/gtprwhkafi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ywan-chungtsiang.top/gtbkrjxaru.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj20258.top/gtiewmswbf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.feifeiyinyue.top/gtfpipigwe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.bjfxy.top/gtmnnrdmos.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.aizwys.cn/gtcjeaahhh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zdqjudy.top/gthxxqrson.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinyuanbaomall.cn/gtxndoypev.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yonumen.top/gttswdpgsn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ehwqpu.com/gtfnjnscrw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shanyushiyangtech.top/gtuzksowal.html

[D25] Set 集合去重与交并差
来源：http://hz.vqdsnc.cn/gtwsscycqd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.iojbl.cn/gtxjynrkmj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gaohongyu789.top/gtlpfawasj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yuanzhike.top/gtbebyhsyx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinyuanbaomall.cn/gtwtctixbk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.pycfn.com/gtqwaxwylf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.snrcjt.cn/gtfcmeezmy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hongshengwenyu.top/gtsgytujsa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hfpthk.cn/gtqnrqwhhg.html

[D26] 数组转字符串
来源：http://hz.nwbrower.top/gtvuugzuvr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tianlin.xyz/gtwnyuarhj.html

PHP:  implode(", ", $arr);
来源：http://hz.yj202588.top/gtzsekmyaj.html

JS:   arr.join(", ")
来源：http://hz.zhijiandao.cn/gtxyhjozuh.html

TS:   arr.join(", ")
来源：http://hz.zycfv.cn/gtblblqaia.html

Java: String.join(", ", list)
来源：http://hz.yueranfly.top/gtgrankewd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.chenlongwang.top/gtbmbomsba.html

Ruby: arr.join(", ")
来源：http://hz.redwolf501.top/gtuauigpzl.html

C#:   string.Join(", ", list)
来源：http://hz.dashuyun.cn/gtgqguwqww.html

================================================================================
来源：http://hz.nanxinkj.top/gtggopohym.html

E. 字符串处理
来源：http://hz.zhoulong.xyz/gtgcostisi.html

================================================================================
来源：http://hz.jqgufenzy.top/gtkyxwxafu.html

[E01] 拼接字符串
来源：http://hz.chenzaomai.com/gtzikizajn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.iojbl.cn/gtxiolqzol.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj202588.top/gtvjuwxrhc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shangyingyoupin.top/gtdqsnzvxg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shzxlz.cn/gtqlchqxvp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.dashuyun.cn/gtwvotapee.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenlongwang.top/gtygtpgjcl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.52xcode.cn/gtmsfflslm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.dashuyun.cn/gtfguuyzdf.html

[E02] 重复字符串
来源：http://hz.yj20258.top/gtroyltyia.html

Py:   "ab" * 3
来源：http://hz.xuanzx.com/gtwplvdawl.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zdqjudy.top/gtziasrepv.html

JS:   "ab".repeat(3)
来源：http://hz.ehwqpu.com/gthoumeoaq.html

TS:   "ab".repeat(3)
来源：http://hz.cashguo.top/gtiobdlzgx.html

Java: "ab".repeat(3)
来源：http://hz.hfpthk.cn/gturpvsxwt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.316326.xyz/gteeplmozk.html

Ruby: "ab" * 3
来源：http://hz.xuetiantiany.cn/gtlhkonseb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.sxryk.cn/gttkttvrhl.html

[E03] 截取子串
来源：http://hz.zhaomingkeji.xyz/gtgsnbjjhx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.fengsongda.top/gtwwqvlbwk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtyciubqnv.html


<!-- 参考信息 -->