代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://hz.dianchejie.cn/gtdxivpqut.html

Go:   func add(a, b int) int
来源：http://hz.feifeiyinyue.top/gtefgeirxw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yj20258888.top/gtksqaaqic.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.nanxinkj.top/gtgewosplx.html

[C14] 泛型函数
来源：http://hz.pycfn.com/gtdgnochoi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.smart0.xyz/gtdquzkedz.html

PHP:  // 无泛型
来源：http://hz.daria6918.cn/gtvdvbpjos.html

JS:   // 无泛型
来源：http://hz.jqgufenzy.top/gtlcukvasu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.0kj1m.cn/gtsqecrlsx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xinyue.icu/gtdewbytvb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xziqi.cn/gtsvbrwczu.html

Ruby: # 无泛型
来源：http://hz.cdnleiting.top/gtblsgunet.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.svipenyu.cn/gtvuamkfgn.html

[C15] 解构 / 展开参数
来源：http://hz.zhongyouzk.top/gtwwqkgxru.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gotoacloud.top/gtsgdllvwj.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shuidangran.top/gtpqtbzfrv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.vqdsnc.cn/gtgqcezutn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hnxiangtu.top/gtebhoheza.html

Java: // 无解构
来源：http://hz.mhx1999.top/gtwwurvqpq.html

Go:   // 无解构
来源：http://hz.meibo888.top/gtqcaqjvqx.html

Ruby: a, b = pair
来源：http://hz.hysaishi.cn/gtvhidkmxk.html

C#:   var (a, b) = pair;
来源：http://hz.bjfxy.top/gtcxfiyual.html

[C16] 函数 / 方法重载
来源：http://hz.aibaodan.cn/gtihkccgrq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinyuanbaomall.cn/gtfxzlaqvb.html

PHP:  // 无重载
来源：http://hz.pycfn.com/gtzpiciouz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yj20258888.top/gtcykumkha.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xziqi.cn/gtnilsclbh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.haohaochexian.top/gtariolseu.html

Go:   // 无重载：用不同函数名
来源：http://hz.yanxiufei.cn/gtlopmtwbb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shangyingyoupin.top/gtodtvncyy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ydjk.org.cn/gttcvxpbem.html

================================================================================
来源：http://hz.zycfv.cn/gtjemvgykj.html

D. 数组 / 列表 / 集合
来源：http://hz.havefunace.top/gtxybwsbgl.html

================================================================================
来源：http://hz.zhongyouzk.top/gtxflavmhu.html

[D01] 创建数组 / 列表
来源：http://hz.yonumen.top/gtoetzpvkk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xylfe.cn/gtgfvrhtdn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhongyouzk.top/gtamqgxlif.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.aibaodan.cn/gtljvibgcm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ybcxt.top/gttjtgmmhr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhoulong.xyz/gthjkitdyn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hammf.cn/gtctdmrdcm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.daxiang520.top/gtbzhnzqcn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.nwbrower.top/gtnsagntnn.html

[D02] 追加元素到末尾
来源：http://hz.cdnleiting.top/gttapensbr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.nanxinkj.top/gtxzfahnrz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jyoumei.cn/gtldvafqal.html

JS:   arr.push(4);
来源：http://hz.yonumen.top/gtmtdrfivz.html

TS:   arr.push(4);
来源：http://hz.gogol.net.cn/gtstfozobq.html

Java: list.add(4);
来源：http://hz.ywan-chungtsiang.top/gtczzekain.html

Go:   arr = append(arr, 4)
来源：http://hz.xylfe.cn/gtxqkclqux.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yvedp.cn/gtfsozxfix.html

C#:   list.Add(4);
来源：http://hz.yuanzhike.top/gtbmsuyxbx.html

[D03] 在指定位置插入元素
来源：http://hz.nanxuanxn.top/gtywxcuglz.html

Py:   arr.insert(0, 0)
来源：http://hz.yueranfly.top/gtgiduzrqz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shanyushiyangtech.top/gtszhkawje.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yanxiufei.cn/gtlwgfugfr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sweek.top/gtixdmtqzr.html

Java: list.add(0, 0);
来源：http://hz.chenzaomai.com/gtcahtzmai.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.smart0.xyz/gtexitfxgm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj20258888.top/gtdsvroxje.html

C#:   list.Insert(0, 0);
来源：http://hz.guowangkeji.top/gtoigxvmgv.html

[D04] 删除元素
来源：http://hz.sysykeji.top/gtuhfnngwl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenzaomai.com/gtlplyenyz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.c1oappe.top/gtiygricai.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.aibaodan.cn/gtnlatitfj.html

TS:   arr.splice(0, 1);
来源：http://hz.yangfankeji.com/gtfyymcdng.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yongpay.top/gtuoyaaepi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.andypj.xyz/gtzjxgnyzb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinqigfzy.top/gtbymfpuwm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.nanxuanxn.top/gtkwuaypiq.html

[D05] 访问与修改元素
来源：http://hz.hywenlv.cn/gtgsvhzebq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gtevjwhykv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj20258.top/gtddspyycu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shangyingyoupin.top/gtbvegzcxk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.birdmap.top/gtyprvrzvq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.kuanghao11.cn/gthlbqwyky.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gogol.net.cn/gtdjsnxtxe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jianghu66.top/gtwnzsvdwu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.daxiang520.top/gtyhqdwdjf.html

[D06] 数组长度
来源：http://hz.jinqigufen.top/gtyiwljyqp.html

Py:   len(arr)
来源：http://hz.yanxiufei.cn/gtpfwgxjqd.html

PHP:  count($arr);
来源：http://hz.kuanghao11.cn/gtvrajzrxk.html

JS:   arr.length
来源：http://hz.daria6918.cn/gtyybbjhxp.html

TS:   arr.length
来源：http://hz.zhaomingkeji.xyz/gtqetyrcxq.html

Java: list.size();
来源：http://hz.zhengqikj.top/gtysbjacaa.html

Go:   len(arr)
来源：http://hz.shzxlz.cn/gtjqzzkcao.html

Ruby: arr.length; arr.size
来源：http://hz.zycfv.cn/gtkdbnazrr.html

C#:   list.Count;
来源：http://hz.bjfxy.top/gtdkndpica.html

[D07] 切片 / 取子数组
来源：http://hz.yonumen.top/gtbrpkiisn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.haohaochexian.top/gtcgnzrpbc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.316326.xyz/gtnieetlim.html

JS:   arr.slice(1, 4);
来源：http://hz.yuanzhike.top/gtetghbdac.html

TS:   arr.slice(1, 4);
来源：http://hz.sweek.top/gtjdqauzgh.html

Java: list.subList(1, 4);
来源：http://hz.cucudq.cn/gtsxwhuhxa.html

Go:   arr[1:4]
来源：http://hz.jinqigufen.top/gtnwwkhinp.html

Ruby: arr[1, 3]
来源：http://hz.316326.xyz/gtgwirterb.html

C#:   list.GetRange(1, 3);
来源：http://hz.zdqjudy.top/gtcazvpmeb.html

[D08] 合并两个数组
来源：http://hz.gotoacloud.top/gtppknenrh.html

Py:   a + b;  a.extend(b)
来源：http://hz.vqdsnc.cn/gtacsodwto.html

PHP:  array_merge($a, $b);
来源：http://hz.dianchejie.cn/gtmkikqgem.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yanxiufei.cn/gtxwxlcnmm.html

TS:   [...a, ...b];
来源：http://hz.cucudq.cn/gtkctqpzzs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yuanzhike.top/gtefbbmbtr.html

Go:   append(a, b...)
来源：http://hz.shuidangran.top/gtympworjx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zycfv.cn/gtktnuhscn.html

C#:   a.Concat(b).ToList()
来源：http://hz.yongpay.top/gtmzseaxef.html

[D09] 排序（升序）
来源：http://hz.shanyushiyangtech.top/gtsupnpkdr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.vqdsnc.cn/gtbvcwsqui.html

PHP:  sort($arr);
来源：http://hz.sweek.top/gtdgtuwlur.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhongyouzk.top/gthwdsvbtl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xuanzx.com/gtppoklzgi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ybcxt.top/gthveijcvo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.guowangkeji.top/gtskiwnjgx.html

Ruby: arr.sort
来源：http://hz.316326.xyz/gtljtndiey.html

C#:   list.Sort();
来源：http://hz.dashuyun.cn/gtdyxzguei.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.316326.xyz/gtmnvnobrn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.9152youxi.cn/gtxhkpumgh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.dianchejie.cn/gtuffwunwl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.svipenyu.cn/gtiarisefo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sufxvd.cn/gtscomparr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinqigufen.top/gtmlkvllzz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yj20258.top/gtckkbodei.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ybcxt.top/gtbljlceqy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.aizwys.cn/gtwopgpwew.html

[D11] 反转数组
来源：http://hz.yanxiufei.cn/gtwiashrbw.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhijiandao.cn/gtfvrquzwe.html

PHP:  array_reverse($arr);
来源：http://hz.gogol.net.cn/gtnxepxlny.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.aizwys.cn/gtynruzxcz.html

TS:   [...arr].reverse();
来源：http://hz.hnqzz.top/gtywarlvax.html

Java: Collections.reverse(list);
来源：http://hz.aizwys.cn/gthpfyydjr.html

Go:   slices.Reverse(arr)
来源：http://hz.jyoumei.cn/gtxsbibovz.html

Ruby: arr.reverse
来源：http://hz.wangdashe.top/gtttaxjupl.html

C#:   list.Reverse();
来源：http://hz.svipenyu.cn/gtjllhcpcj.html

[D12] 查找元素下标
来源：http://hz.ppjwa.cn/gtfgqrcphk.html

Py:   arr.index(x);  x in arr
来源：http://hz.cheryme.top/gtuuckndmh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.c1oappe.top/gtjcgypxym.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shangyingyoupin.top/gtyzolprxg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guowangkeji.top/gtivrdjnrt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.chenzaomai.com/gtizaquwkw.html

Go:   slices.Index(arr, x)
来源：http://hz.shzxlz.cn/gtxpviaaij.html

Ruby: arr.index(x)
来源：http://hz.guannengcc.top/gtfixwysmj.html

C#:   list.IndexOf(x);
来源：http://hz.ppjwa.cn/gtpdnnurie.html

[D13] 过滤（保留满足条件的）
来源：http://hz.chenlongwang.top/gtkjbhifzk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cheryme.top/gttasgtpnd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.quarkkingdee.top/gtpbucvcqn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.cqqwz.cn/gtqgddwcac.html

TS:   arr.filter(x => x > 3)
来源：http://hz.meibo888.top/gtlrhkcrwo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ppjwa.cn/gtjgonxwmw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hongshengwenyu.top/gtuuswgdvh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shzxlz.cn/gtpijbyjyn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jiagoushi.top/gtvesyklpo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhongyouzk.top/gtsxcullhg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cdnleiting.top/gttcgmtpdb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ywan-chungtsiang.top/gtqkozbnqx.html

JS:   arr.map(x => x * 2)
来源：http://hz.gaohongyu789.top/gtrpslkrtj.html

TS:   arr.map(x => x * 2)
来源：http://hz.xinyue.icu/gtgoygkjxt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hnxiangtu.top/gtuculpohr.html

Go:   // 手写循环
来源：http://hz.svipenyu.cn/gtqqgaskgc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hnqzz.top/gtrhnqdsdw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cdnleiting.top/gtktywdadx.html

[D15] 去重
来源：http://hz.wangdashe.top/gttllyznhk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.tianlin.xyz/gtzzturimh.html

PHP:  array_unique($arr);
来源：http://hz.c1oappe.top/gtyjxzhjve.html

JS:   [...new Set(arr)]
来源：http://hz.316326.xyz/gtqhfszyip.html

TS:   [...new Set(arr)]
来源：http://hz.shzxlz.cn/gtnjpqaolo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinyuanbaomall.cn/gttqgniusl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cheryme.top/gtklrxzskr.html

Ruby: arr.uniq
来源：http://hz.jinghuilouyu.cn/gtqidspihx.html

C#:   list.Distinct().ToList()
来源：http://hz.shangyingyoupin.top/gtnkfdblxa.html

[D16] 求和与平均值
来源：http://hz.dashuyun.cn/gtunksdnbx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhixingplan.top/gtalklqbyr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.aibaodan.cn/gtiwaurrck.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.haohaochexian.top/gtnxiyyuce.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cheryme.top/gtgjskbbzc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hnqzz.top/gtljivuaiw.html

Go:   // 手写循环累加
来源：http://hz.chenjidiqi.icu/gtqxvqlfmd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hnxiangtu.top/gtefvtaseg.html

C#:   list.Sum();  list.Average()
来源：http://hz.fzhhl.top/gtohzlmfqa.html

[D17] 最大值与最小值
来源：http://hz.redwolf501.top/gtbhzhvwyv.html

Py:   max(arr);  min(arr)
来源：http://hz.shangyingyoupin.top/gtzmhlmvhy.html

PHP:  max($arr);  min($arr);
来源：http://hz.bjfxy.top/gtjvficodm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.pengpengdd.cyou/gtjyxsaajv.html

TS:   Math.max(...arr);
来源：http://hz.zhoulong.xyz/gtptsukgdt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.vqdsnc.cn/gtudcgszxw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zdqjudy.top/gtjbykkyum.html

Ruby: arr.max;  arr.min
来源：http://hz.zhengqikj.top/gttaggnxvd.html

C#:   list.Max();  list.Min()
来源：http://hz.mhx1999.top/gtlpvohezx.html

[D18] 扁平化嵌套数组
来源：http://hz.ehwqpu.com/gtnretdppe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.fengsongda.top/gtdozauojn.html

PHP:  array_merge(...$nested);
来源：http://hz.kuanghao11.cn/gtrtmdovsz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.dianchejie.cn/gtkxtnhjsc.html

TS:   nested.flat();
来源：http://hz.sweek.top/gthggpvbdo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xinyue.icu/gtcqmjiags.html

Go:   // 手写双层循环
来源：http://hz.pycfn.com/gtasuoivbe.html

Ruby: nested.flatten
来源：http://hz.ehwqpu.com/gthekuxbjb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zdqjudy.top/gtnjcfksjk.html

[D19] 按字段分组
来源：http://hz.ywan-chungtsiang.top/gtfmffrylt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenjidiqi.icu/gtfkemcrgi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jqgfzy.top/gtzeecekos.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinyuanbaomall.cn/gtjwlvieug.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yonumen.top/gtfnewpcud.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yanxiufei.cn/gtmhwpimdz.html

Go:   // 手写 map[string][]T
来源：http://hz.yuanzhike.top/gtntjapjei.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shangyingyoupin.top/gtiepdhwof.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hysaishi.cn/gtswfwdner.html

[D20] 统计每个元素出现次数
来源：http://hz.wangshuangyany.cn/gtjepgnwnd.html

Py:   Counter(arr)
来源：http://hz.zhijiandao.cn/gtxvpuelat.html

PHP:  array_count_values($arr);
来源：http://hz.c1oappe.top/gtpdsfimcw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zycfv.cn/gtijqxbgrq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ivvv.top/gtoxtuflle.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hammf.cn/gtculkarof.html

Go:   // 手写 map[T]int
来源：http://hz.sweek.top/gtptwvpnll.html

Ruby: arr.tally
来源：http://hz.cdnleiting.top/gtnolxlbev.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yueranfly.top/gtzcvzeecc.html

[D21] 判断是否包含某元素
来源：http://hz.shzxlz.cn/gtbaawhbsq.html

Py:   x in arr
来源：http://hz.zhongyouzk.top/gtijmsytkk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhixingplan.top/gtjebzvgaj.html

JS:   arr.includes(x)
来源：http://hz.hongshengwenyu.top/gtawfuhtkx.html

TS:   arr.includes(x)
来源：http://hz.tian-w.cn/gtnfrhxvca.html

Java: list.contains(x)
来源：http://hz.jinghuilouyu.cn/gtlufxicop.html

Go:   slices.Contains(arr, x)
来源：http://hz.316326.xyz/gtsebnjkqi.html

Ruby: arr.include?(x)
来源：http://hz.nanxuanxn.top/gtudzuswjm.html

C#:   list.Contains(x)
来源：http://hz.hfpthk.cn/gtiqcoetlf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.snrcjt.cn/gtzmvmaozj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhaomingkeji.xyz/gtqihjhcwg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cqqwz.cn/gtyjrcvqok.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zdqjudy.top/gtpakwmzty.html

TS:   [...arr];
来源：http://hz.hnxiangtu.top/gtwibnlfxh.html

Java: new ArrayList<>(list);
来源：http://hz.iojbl.cn/gtfjdhgokm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.meibo888.top/gtbxqnnyrv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yanxiufei.cn/gtpinrxhty.html

C#:   new List<int>(list);
来源：http://hz.yuanzhike.top/gtjmhhytcj.html

[D23] reduce 累积计算
来源：http://hz.hammf.cn/gtwkifjprq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.52xcode.cn/gtmvltncst.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.fzhhl.top/gtlarxqffj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhaomingkeji.xyz/gttjshjfnt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.daria6918.cn/gtzlqrtvmd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.dashuyun.cn/gtgajgbfex.html

Go:   // 手写循环
来源：http://hz.shanyushiyangkeji.top/gtrfnfrwwo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sufxvd.cn/gtvlvigxrl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yueranfly.top/gtjemhczsv.html

[D24] 字典 / Map 基本操作
来源：http://hz.nanxinkj.top/gtmrpqcqcd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.aizwys.cn/gtlwfsycas.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.snrcjt.cn/gtpvrvjopd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xingfuxueyuan.xyz/gtnxjiijhu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yanxiufei.cn/gtmuygqpgw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yongpay.top/gtsuqbeesa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jiagoushi.top/gtfbzvcatz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xuetiantiany.cn/gtakxznsgi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ppjwa.cn/gtzzhjsgxd.html

[D25] Set 集合去重与交并差
来源：http://hz.cdnleiting.top/gtxmvriuzp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yueranfly.top/gtcbroxdpj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhoulong.xyz/gtonekltqg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.guannengcc.top/gtzhqmlnpl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xziqi.cn/gtjhhkiuhq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.quarkkingdee.top/gtbwipsluo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.316326.xyz/gtzyoynkol.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhaomingkeji.xyz/gtjhmimdfa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cqqwz.cn/gtkvoxrami.html

[D26] 数组转字符串
来源：http://hz.vqdsnc.cn/gtmaivsmii.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ppjwa.cn/gtkzidrtxv.html

PHP:  implode(", ", $arr);
来源：http://hz.jinqigfzy.top/gtmfhdsfsf.html

JS:   arr.join(", ")
来源：http://hz.sysykeji.top/gtcinuxmwy.html

TS:   arr.join(", ")
来源：http://hz.tianlin.xyz/gtxlchldga.html

Java: String.join(", ", list)
来源：http://hz.redwolf501.top/gtqfhblrrp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hywenlv.cn/gtpwqgbyxh.html

Ruby: arr.join(", ")
来源：http://hz.ehwqpu.com/gtigwiidcx.html

C#:   string.Join(", ", list)
来源：http://hz.gogol.net.cn/gtkxrhclbe.html

================================================================================
来源：http://hz.yuxming.cn/gtxrvgcfbm.html

E. 字符串处理
来源：http://hz.yj20258.top/gtgcwfhibr.html

================================================================================
来源：http://hz.svipenyu.cn/gtewpclvtr.html

[E01] 拼接字符串
来源：http://hz.c1oappe.top/gtfiwlletk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ybcxt.top/gthmtbepjd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sxryk.cn/gtyrsgysix.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhaomingkeji.xyz/gtdpnmetyb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nwbrower.top/gtijxaeiox.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.316326.xyz/gtshgltdvt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.kuanghao11.cn/gtwcdcyqmt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.svipenyu.cn/gtdhkuhjct.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gogol.net.cn/gtwamzhwty.html

[E02] 重复字符串
来源：http://hz.xuetiantiany.cn/gtebuxszxu.html

Py:   "ab" * 3
来源：http://hz.quarkkingdee.top/gtpvabzvlt.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hongshengwenyu.top/gtoocgoyog.html

JS:   "ab".repeat(3)
来源：http://hz.gzhubu.top/gtptbvbdof.html

TS:   "ab".repeat(3)
来源：http://hz.gaohongyu789.top/gtvzfjswvf.html

Java: "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtfmlyxmdv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.fzhhl.top/gtqybdflfy.html

Ruby: "ab" * 3
来源：http://hz.nwbrower.top/gticgwvkvm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhengqikj.top/gtycthmnuq.html

[E03] 截取子串
来源：http://hz.pengpengdd.cyou/gtfmowvtix.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj20258.top/gtijxlfolo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gaohongyu789.top/gtthytchpv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhengqikj.top/gtybxorrcg.html

TS:   s.slice(1, 4)
来源：http://hz.zhixingplan.top/gtpngoxjvk.html

Java: s.substring(1, 4)
来源：http://hz.hnxiangtu.top/gtchsdhhkl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.aizwys.cn/gtzajlxizl.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jqgfzy.top/gtcthffziw.html

C#:   s.Substring(1, 3)
来源：http://hz.zhongyouzk.top/gtpjyelkrk.html

[E04] 查找子串位置
来源：http://hz.zhongyouzk.top/gtnlpvswbl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.daria6918.cn/gtrrnrppti.html


<!-- 参考信息 -->