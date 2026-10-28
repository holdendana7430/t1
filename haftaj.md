代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhijiandao.cn/gtrzqfvgqx.html

Go:   func add(a, b int) int
来源：http://hz.yanxiufei.cn/gtwwwyfafn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xingfuxueyuan.xyz/gtxraiwqyp.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jiagoushi.top/gtdudcfjht.html

[C14] 泛型函数
来源：http://hz.zhengqikj.top/gtanylejcr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.svipenyu.cn/gtojjmqxkw.html

PHP:  // 无泛型
来源：http://hz.daria6918.cn/gtynznwaes.html

JS:   // 无泛型
来源：http://hz.meibo888.top/gtsfktpczq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shangyingyoupin.top/gtarlljryt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.svipenyu.cn/gtrwnkgviq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nanxinkj.top/gtfhxgwyjg.html

Ruby: # 无泛型
来源：http://hz.yanxiufei.cn/gttdqscjbp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.wangshuangyany.cn/gtajivwtrm.html

[C15] 解构 / 展开参数
来源：http://hz.316326.xyz/gtjgsudtxm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.chenjidiqi.icu/gtzeonbkzr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.316326.xyz/gtqpxqbrca.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yuanzhike.top/gtsokretlb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jqgufenzy.top/gtziepcobn.html

Java: // 无解构
来源：http://hz.shanyushiyangkeji.top/gtqajbgjtw.html

Go:   // 无解构
来源：http://hz.svipenyu.cn/gtnwlthtmr.html

Ruby: a, b = pair
来源：http://hz.ybcxt.top/gtdmshafyn.html

C#:   var (a, b) = pair;
来源：http://hz.zhongyouzk.top/gteyflnjac.html

[C16] 函数 / 方法重载
来源：http://hz.cqqwz.cn/gtxyurxvfs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.fengsongda.top/gtkyxouoxk.html

PHP:  // 无重载
来源：http://hz.snrcjt.cn/gtblcmdegh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.havefunace.top/gthwtfyotw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.smart0.xyz/gttxxsgwlw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinghuilouyu.cn/gtnmeuziop.html

Go:   // 无重载：用不同函数名
来源：http://hz.aizwys.cn/gtviyrxbtk.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gotoacloud.top/gtqcuzghdy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ywan-chungtsiang.top/gtpljayncg.html

================================================================================
来源：http://hz.9152youxi.cn/gtrwlkqeow.html

D. 数组 / 列表 / 集合
来源：http://hz.xuanzx.com/gtfflkkokw.html

================================================================================
来源：http://hz.cdnleiting.top/gtrtdyamef.html

[D01] 创建数组 / 列表
来源：http://hz.daria6918.cn/gtnuflbrwc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xuanzx.com/gthyzdhwua.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ywan-chungtsiang.top/gtmjsfvzxp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jlsjyb.cn/gtoqgwclaj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cdnleiting.top/gthwhysztc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xinyue.icu/gtwngamtun.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hywenlv.cn/gtlezokidn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.bjfxy.top/gtlutppnhi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xziqi.cn/gtfyytjhah.html

[D02] 追加元素到末尾
来源：http://hz.316326.xyz/gtcskvrbpe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cashguo.top/gtncrwyvfi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.dianchejie.cn/gtwipshgud.html

JS:   arr.push(4);
来源：http://hz.dashuyun.cn/gthnzzlsmj.html

TS:   arr.push(4);
来源：http://hz.birdmap.top/gtcrhlopss.html

Java: list.add(4);
来源：http://hz.yj20258.top/gtcjhmmwol.html

Go:   arr = append(arr, 4)
来源：http://hz.jqgfzy.top/gtrhshagkc.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ywan-chungtsiang.top/gtjepkkisn.html

C#:   list.Add(4);
来源：http://hz.yueranfly.top/gtrtmocxgt.html

[D03] 在指定位置插入元素
来源：http://hz.jinghuilouyu.cn/gtrwvqcsqx.html

Py:   arr.insert(0, 0)
来源：http://hz.dianchejie.cn/gtmldhqqrc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ivvv.top/gtrdpapejd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.0kj1m.cn/gtcotmimyx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sweek.top/gtmesddeje.html

Java: list.add(0, 0);
来源：http://hz.52xcode.cn/gtdpgeslmk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.316326.xyz/gtzwfhniur.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.nanxuanxn.top/gtmjhcagzh.html

C#:   list.Insert(0, 0);
来源：http://hz.316326.xyz/gtctaouezt.html

[D04] 删除元素
来源：http://hz.chenlongwang.top/gtthsiauys.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.redwolf501.top/gtprjshign.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.nanxinkj.top/gthqlkeeul.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.9152youxi.cn/gtshwgvuim.html

TS:   arr.splice(0, 1);
来源：http://hz.cheryme.top/gtfgruxilf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ivvv.top/gtkvxxxdst.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.aizwys.cn/gtzwghnuyl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hongshengwenyu.top/gttydiwzgp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jyoumei.cn/gtdeoycbum.html

[D05] 访问与修改元素
来源：http://hz.cheryme.top/gtpcektqzl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ywan-chungtsiang.top/gtdqqzyhur.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhixingplan.top/gtjjopeabl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.9152youxi.cn/gtdsqkcaee.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nanxinkj.top/gtuzvgyhnz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ywan-chungtsiang.top/gtlrncgkyl.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sxryk.cn/gtsjbzvwmc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fzhhl.top/gtwzjevdgd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhaomingkeji.xyz/gtzrfuzorf.html

[D06] 数组长度
来源：http://hz.jlsjyb.cn/gttquurqvs.html

Py:   len(arr)
来源：http://hz.zhijiandao.cn/gttgcwvxdg.html

PHP:  count($arr);
来源：http://hz.dianchejie.cn/gtpmznvkbw.html

JS:   arr.length
来源：http://hz.zdqjudy.top/gtqzjituhd.html

TS:   arr.length
来源：http://hz.cdnleiting.top/gtjsgsyxaj.html

Java: list.size();
来源：http://hz.pengpengdd.cyou/gtwzorqtci.html

Go:   len(arr)
来源：http://hz.chenzaomai.com/gtftrvfmdt.html

Ruby: arr.length; arr.size
来源：http://hz.ywan-chungtsiang.top/gtcwrvkwlw.html

C#:   list.Count;
来源：http://hz.xinyue.icu/gtftibjhfo.html

[D07] 切片 / 取子数组
来源：http://hz.jinghuilouyu.cn/gtcyqwdctq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.wangshuangyany.cn/gtsuwztwcn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shanyushiyangkeji.top/gthyiqqkbe.html

JS:   arr.slice(1, 4);
来源：http://hz.zhaomingkeji.xyz/gtadsteyxx.html

TS:   arr.slice(1, 4);
来源：http://hz.xylfe.cn/gthbfkxcvv.html

Java: list.subList(1, 4);
来源：http://hz.jyoumei.cn/gtdjrkyecn.html

Go:   arr[1:4]
来源：http://hz.yvedp.cn/gtbizveelk.html

Ruby: arr[1, 3]
来源：http://hz.aibaodan.cn/gtatzmgrrb.html

C#:   list.GetRange(1, 3);
来源：http://hz.hfpthk.cn/gtqiomheth.html

[D08] 合并两个数组
来源：http://hz.chenzaomai.com/gttoqexypr.html

Py:   a + b;  a.extend(b)
来源：http://hz.nwbrower.top/gtajnicfqm.html

PHP:  array_merge($a, $b);
来源：http://hz.iojbl.cn/gtjkdtqhrf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.tanke756.top/gtjlwiofiv.html

TS:   [...a, ...b];
来源：http://hz.hywenlv.cn/gtcnyhtvzw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hammf.cn/gtmueglghc.html

Go:   append(a, b...)
来源：http://hz.zdqjudy.top/gtikbcupqy.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ywan-chungtsiang.top/gtewtmavta.html

C#:   a.Concat(b).ToList()
来源：http://hz.yonumen.top/gtegtpzkpl.html

[D09] 排序（升序）
来源：http://hz.xuetiantiany.cn/gtjhurzrlt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xziqi.cn/gtxrjiabtf.html

PHP:  sort($arr);
来源：http://hz.zhijiandao.cn/gtybhokhum.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.vqdsnc.cn/gtafxnoouw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhengqikj.top/gtbvytusag.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xinyue.icu/gtpmpalqcy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.9152youxi.cn/gtetwfiwat.html

Ruby: arr.sort
来源：http://hz.ybcxt.top/gtnfcaoibv.html

C#:   list.Sort();
来源：http://hz.316326.xyz/gtsjqifrin.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.dianchejie.cn/gtvfjponbv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhoulong.xyz/gtbzuufpah.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.pycfn.com/gtywdxoquo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gotoacloud.top/gtlekevtzk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnxiangtu.top/gtnsuermnv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.smart0.xyz/gtsjggzknq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zdqjudy.top/gtotrmylmm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hnqzz.top/gtqjvtonlx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xuanzx.com/gtshwezcle.html

[D11] 反转数组
来源：http://hz.haohaochexian.top/gtyrveqpos.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhijiandao.cn/gtyiayspwc.html

PHP:  array_reverse($arr);
来源：http://hz.dashuyun.cn/gtzgtecqut.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.nanxuanxn.top/gtbdjmzhnh.html

TS:   [...arr].reverse();
来源：http://hz.zhaomingkeji.xyz/gttqfobzjj.html

Java: Collections.reverse(list);
来源：http://hz.aibaodan.cn/gtccjryomn.html

Go:   slices.Reverse(arr)
来源：http://hz.zhaomingkeji.xyz/gtindcohtb.html

Ruby: arr.reverse
来源：http://hz.gaohongyu789.top/gtmbonyquo.html

C#:   list.Reverse();
来源：http://hz.yanxiufei.cn/gtzflljzyj.html

[D12] 查找元素下标
来源：http://hz.hammf.cn/gtcmifwego.html

Py:   arr.index(x);  x in arr
来源：http://hz.aizwys.cn/gtutjxawxr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jianghu66.top/gtzyzymkak.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gtvzfzolfi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gaohongyu789.top/gtsefblefc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.wangshuangyany.cn/gtfvqpfyzo.html

Go:   slices.Index(arr, x)
来源：http://hz.yj20258888.top/gtycvfgaoh.html

Ruby: arr.index(x)
来源：http://hz.hammf.cn/gtucsliafa.html

C#:   list.IndexOf(x);
来源：http://hz.yj202588.top/gtyppalghd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhoulong.xyz/gtdfqxezou.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yueranfly.top/gtbapvntdc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.pycfn.com/gtnvogvtzn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ppjwa.cn/gtwgqlpito.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ehwqpu.com/gtryqznzsd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.havefunace.top/gttriupapa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cucudq.cn/gthadvlpjp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.meibo888.top/gtnfifbojw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sxryk.cn/gthtklcyyw.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sufxvd.cn/gtfeggawmq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jqgufenzy.top/gtselmxsev.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.guowangkeji.top/gtoekkxetf.html

JS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangtech.top/gtjrjlgtot.html

TS:   arr.map(x => x * 2)
来源：http://hz.cashguo.top/gtvfgjnawd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yj202588.top/gtwofshqij.html

Go:   // 手写循环
来源：http://hz.daxiang520.top/gtdpvuttha.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ivvv.top/gtqdhsmlvk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hammf.cn/gtbpafmcyl.html

[D15] 去重
来源：http://hz.daria6918.cn/gtgeuhyvho.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xuetiantiany.cn/gtpxqjstvs.html

PHP:  array_unique($arr);
来源：http://hz.sysykeji.top/gtmmdetfue.html

JS:   [...new Set(arr)]
来源：http://hz.yj20258.top/gtfzytudtj.html

TS:   [...new Set(arr)]
来源：http://hz.cheryme.top/gtuommhtit.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.snrcjt.cn/gtbcsgiuic.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hysaishi.cn/gtumpunmhg.html

Ruby: arr.uniq
来源：http://hz.yvedp.cn/gthtxiauvx.html

C#:   list.Distinct().ToList()
来源：http://hz.ivvv.top/gtmiexoznc.html

[D16] 求和与平均值
来源：http://hz.gzhubu.top/gtribcgmco.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hywenlv.cn/gtgtkykfyn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nwbrower.top/gteciixcwk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.c1oappe.top/gtgqsogoai.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258888.top/gtcrmemgwf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xylfe.cn/gtmwarbcpu.html

Go:   // 手写循环累加
来源：http://hz.ivvv.top/gtkhhaunco.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinqigufen.top/gtitokwpje.html

C#:   list.Sum();  list.Average()
来源：http://hz.haohaochexian.top/gtnafuslsl.html

[D17] 最大值与最小值
来源：http://hz.chenzaomai.com/gttedtwbkm.html

Py:   max(arr);  min(arr)
来源：http://hz.shangyingyoupin.top/gtsdmmtgxz.html

PHP:  max($arr);  min($arr);
来源：http://hz.dianchejie.cn/gtcfsgpfhy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gaohongyu789.top/gtpconndcw.html

TS:   Math.max(...arr);
来源：http://hz.tanke756.top/gtcgjxrybp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.redwolf501.top/gthlydbfde.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xziqi.cn/gtemvetede.html

Ruby: arr.max;  arr.min
来源：http://hz.ivvv.top/gtyrxhlunc.html

C#:   list.Max();  list.Min()
来源：http://hz.meibo888.top/gttsutofhj.html

[D18] 扁平化嵌套数组
来源：http://hz.chenlongwang.top/gtrahuelzt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.fengsongda.top/gtachlkoid.html

PHP:  array_merge(...$nested);
来源：http://hz.shanyushiyangtech.top/gtdzenumil.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yuanzhike.top/gtcglhuabm.html

TS:   nested.flat();
来源：http://hz.ywan-chungtsiang.top/gtxsyrczyz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jqgufenzy.top/gtbaleexau.html

Go:   // 手写双层循环
来源：http://hz.hnxiangtu.top/gtuvchusro.html

Ruby: nested.flatten
来源：http://hz.cashguo.top/gteeyebrzq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cdnleiting.top/gtebelwxxm.html

[D19] 按字段分组
来源：http://hz.jinghuilouyu.cn/gtszlqkddx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj202588.top/gtayxacavn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yongpay.top/gtlbxsgpvw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tian-w.cn/gtskwnzneu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.guowangkeji.top/gtpjiheamf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.daria6918.cn/gtgeilkiil.html

Go:   // 手写 map[string][]T
来源：http://hz.xziqi.cn/gteqeunmmw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ydjk.org.cn/gteeveodan.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yueranfly.top/gtkwnjfide.html

[D20] 统计每个元素出现次数
来源：http://hz.snrcjt.cn/gtizqkawit.html

Py:   Counter(arr)
来源：http://hz.haohaochexian.top/gtznpibmsq.html

PHP:  array_count_values($arr);
来源：http://hz.aizwys.cn/gtnwuqgfdd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yonumen.top/gtggeeziig.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ehwqpu.com/gtznczhyhz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.feifeiyinyue.top/gthgiyhjkx.html

Go:   // 手写 map[T]int
来源：http://hz.zycfv.cn/gtybygkiju.html

Ruby: arr.tally
来源：http://hz.zhoulong.xyz/gtqtafockp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.wangdashe.top/gteaeizsij.html

[D21] 判断是否包含某元素
来源：http://hz.fengsongda.top/gtoowlbkng.html

Py:   x in arr
来源：http://hz.dianchejie.cn/gtysycgrjn.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yvedp.cn/gtljdberjt.html

JS:   arr.includes(x)
来源：http://hz.shanyushiyangtech.top/gtqeauopwr.html

TS:   arr.includes(x)
来源：http://hz.hnqzz.top/gtqilnnayq.html

Java: list.contains(x)
来源：http://hz.ydzc1.top/gtkekdzbeu.html

Go:   slices.Contains(arr, x)
来源：http://hz.redwolf501.top/gtjcenpnxr.html

Ruby: arr.include?(x)
来源：http://hz.jinghuilouyu.cn/gtgobvfhtn.html

C#:   list.Contains(x)
来源：http://hz.snrcjt.cn/gthpdoydyv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.pycfn.com/gtdmudsfkf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.daxiang520.top/gtfnzajdio.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.aizwys.cn/gttviivvda.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xinyue.icu/gtkdrnwrdp.html

TS:   [...arr];
来源：http://hz.ehwqpu.com/gtfcgejtgt.html

Java: new ArrayList<>(list);
来源：http://hz.c1oappe.top/gtxgwussxb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.andypj.xyz/gtefxfmzop.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xinyue.icu/gtqxjpyxgx.html

C#:   new List<int>(list);
来源：http://hz.316326.xyz/gtayyjvplk.html

[D23] reduce 累积计算
来源：http://hz.ppjwa.cn/gtpjczpbcp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ydjk.org.cn/gtjrnmbwcb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.meibo888.top/gteoqgcjlc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.dashuyun.cn/gtggsvayng.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhongyouzk.top/gtdjweorsh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.chenzaomai.com/gtpfzgaeot.html

Go:   // 手写循环
来源：http://hz.haohaochexian.top/gtbgnjbaml.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.dianchejie.cn/gtuprredwi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.c1oappe.top/gtilatubbm.html

[D24] 字典 / Map 基本操作
来源：http://hz.tanke756.top/gtpfkgprdt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ehwqpu.com/gttjxfirgg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jianghu66.top/gttboiruli.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shangyingyoupin.top/gtbfwqqcfs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.tanke756.top/gtbzkvaozr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenjidiqi.icu/gtuuealkcj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.mhx1999.top/gtzvogpxzp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xuanzx.com/gtdoqnhjrr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xinyue.icu/gtopgaqcgc.html

[D25] Set 集合去重与交并差
来源：http://hz.ehwqpu.com/gtzxzxkeps.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yongpay.top/gtyhqlekyz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jiagoushi.top/gtwsjjlcne.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.aibaodan.cn/gtmzvrsizh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.birdmap.top/gtptbcjbia.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.havefunace.top/gtnoeudggd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.redwolf501.top/gtqverwyod.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.daria6918.cn/gtijoeyghf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.mhx1999.top/gtkhuqvtwo.html

[D26] 数组转字符串
来源：http://hz.yanxiufei.cn/gtxtwxzhkm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yuanzhike.top/gtncfvetrl.html

PHP:  implode(", ", $arr);
来源：http://hz.mhx1999.top/gtkgpeatxt.html

JS:   arr.join(", ")
来源：http://hz.haohaochexian.top/gtplfvqqxz.html

TS:   arr.join(", ")
来源：http://hz.hfpthk.cn/gtzoouqyjc.html

Java: String.join(", ", list)
来源：http://hz.kuanghao11.cn/gtvdhpdqga.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xinyue.icu/gtdwzdtseb.html

Ruby: arr.join(", ")
来源：http://hz.vqdsnc.cn/gtahiwsfhl.html

C#:   string.Join(", ", list)
来源：http://hz.aibaodan.cn/gthvurypsx.html

================================================================================
来源：http://hz.0kj1m.cn/gtmyzcwfxe.html

E. 字符串处理
来源：http://hz.kuanghao11.cn/gtggdnccck.html

================================================================================
来源：http://hz.cheryme.top/gtfkaflsjw.html

[E01] 拼接字符串
来源：http://hz.iojbl.cn/gtzfcuwlji.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zycfv.cn/gtrwdyogyf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.c1oappe.top/gtdskwtttx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuanzx.com/gtapgeeevt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nwbrower.top/gthzfxhnyc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhixingplan.top/gtgtkrvtpv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.sysykeji.top/gtkqdrumjo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tianlin.xyz/gteocusxfm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.birdmap.top/gtrodpfagc.html

[E02] 重复字符串
来源：http://hz.ppjwa.cn/gtyxcjtokm.html

Py:   "ab" * 3
来源：http://hz.hnxiangtu.top/gtqzrjyggp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.52xcode.cn/gthlbeklcj.html

JS:   "ab".repeat(3)
来源：http://hz.sxryk.cn/gtuwzjqxzc.html

TS:   "ab".repeat(3)
来源：http://hz.ywan-chungtsiang.top/gtefurbohc.html

Java: "ab".repeat(3)
来源：http://hz.jinyuanbaomall.cn/gtczmtglrb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yueranfly.top/gttgiyeqmv.html

Ruby: "ab" * 3
来源：http://hz.jlsjyb.cn/gtbulxokxg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.sysykeji.top/gtkdcfoggi.html

[E03] 截取子串
来源：http://hz.cucudq.cn/gtdgmdcmdg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yuanzhike.top/gtjxgfvlld.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.9152youxi.cn/gtynxbwarc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.316326.xyz/gtiqckivlg.html

TS:   s.slice(1, 4)
来源：http://hz.zycfv.cn/gtiepklgju.html

Java: s.substring(1, 4)
来源：http://hz.chenzaomai.com/gtnqoyuqpy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.iojbl.cn/gtxvnhzqsf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.bjfxy.top/gtjvutaxic.html

C#:   s.Substring(1, 3)
来源：http://hz.aizwys.cn/gteczmfiyh.html

[E04] 查找子串位置
来源：http://hz.yj20258888.top/gtbeutnhtt.html

Py:   s.find("x");  s.index("x")
来源：http://hz.chenzaomai.com/gtkehfofuv.html


<!-- 参考信息 -->