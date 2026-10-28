代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.fengsongda.top/gtqvjqxpnd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhoulong.xyz/gtrruzxdtd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cdnleiting.top/gtgddwqndn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhixingplan.top/gtppklzzzf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gogol.net.cn/gtmexmgirq.html

Go:   func add(a, b int) int
来源：http://hz.sufxvd.cn/gtxetsjioz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shuidangran.top/gtoqsfgcoc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gzhubu.top/gtbbxbwjdg.html

[C14] 泛型函数
来源：http://hz.daria6918.cn/gtpkkfncbf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jyoumei.cn/gtngbgonmd.html

PHP:  // 无泛型
来源：http://hz.aizwys.cn/gtxnzkvxwb.html

JS:   // 无泛型
来源：http://hz.nwbrower.top/gtpnfqjhgu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.havefunace.top/gtgznbynng.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xinyue.icu/gthmohvuzo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shzxlz.cn/gtlxjekxol.html

Ruby: # 无泛型
来源：http://hz.316326.xyz/gtvnwvkwpq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.0kj1m.cn/gtrdroxenn.html

[C15] 解构 / 展开参数
来源：http://hz.316326.xyz/gtmsazxqrx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ywan-chungtsiang.top/gtqtusilfz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sxryk.cn/gtuvzyttag.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yj20258.top/gtlgxvtids.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.9152youxi.cn/gtfpojxrtm.html

Java: // 无解构
来源：http://hz.shuidangran.top/gtsbqnrsua.html

Go:   // 无解构
来源：http://hz.jiagoushi.top/gtdkspezxc.html

Ruby: a, b = pair
来源：http://hz.fengsongda.top/gtucohkfwl.html

C#:   var (a, b) = pair;
来源：http://hz.jqgfzy.top/gtgniazheg.html

[C16] 函数 / 方法重载
来源：http://hz.jinyuanbaomall.cn/gtzeoiifxn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.birdmap.top/gtpftuiubl.html

PHP:  // 无重载
来源：http://hz.birdmap.top/gtaosmgmgi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yueranfly.top/gtiplckraj.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ywan-chungtsiang.top/gtynunsclz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.fzhhl.top/gtnzjvzocf.html

Go:   // 无重载：用不同函数名
来源：http://hz.havefunace.top/gtltwbsvbw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cashguo.top/gtbumubtgp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hysaishi.cn/gtowqdckzb.html

================================================================================
来源：http://hz.yuanzhike.top/gtnsybqfub.html

D. 数组 / 列表 / 集合
来源：http://hz.gaohongyu789.top/gtkyzwcmgo.html

================================================================================
来源：http://hz.0kj1m.cn/gttzeueoes.html

[D01] 创建数组 / 列表
来源：http://hz.9152youxi.cn/gtwwpoqmmr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenzaomai.com/gttfxgkcgr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.svipenyu.cn/gtkritqakn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhijiandao.cn/gtvsyyenie.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj20258888.top/gtbmxhliky.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yj20258888.top/gtdxmozawc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.dashuyun.cn/gtnhutunyg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xingfuxueyuan.xyz/gtqhusetrd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xylfe.cn/gtqvtyujsd.html

[D02] 追加元素到末尾
来源：http://hz.yangfankeji.com/gtjsrxwcaw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.fzhhl.top/gtcnyiigfa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.guowangkeji.top/gtnilxaigv.html

JS:   arr.push(4);
来源：http://hz.zhengqikj.top/gtzckvagsy.html

TS:   arr.push(4);
来源：http://hz.andypj.xyz/gtoopuqtxw.html

Java: list.add(4);
来源：http://hz.dashuyun.cn/gtgsjadqmf.html

Go:   arr = append(arr, 4)
来源：http://hz.hnxiangtu.top/gtzfpquhrw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cheryme.top/gtotlyizcr.html

C#:   list.Add(4);
来源：http://hz.xinyue.icu/gtejvlwbcy.html

[D03] 在指定位置插入元素
来源：http://hz.nanxuanxn.top/gteimyexmy.html

Py:   arr.insert(0, 0)
来源：http://hz.jinqigufen.top/gthnvdgawt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.guowangkeji.top/gtuctdufcz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shanyushiyangkeji.top/gtagwbdfei.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shanyushiyangtech.top/gtnccjbbwq.html

Java: list.add(0, 0);
来源：http://hz.c1oappe.top/gtzuvvhozq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shzxlz.cn/gtagloydky.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sweek.top/gtbarkospj.html

C#:   list.Insert(0, 0);
来源：http://hz.jqgfzy.top/gthjvlotod.html

[D04] 删除元素
来源：http://hz.dashuyun.cn/gtzujerggq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.meibo888.top/gtvgichxun.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yanxiufei.cn/gtsrowssdi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jinqigufen.top/gtnaaispxc.html

TS:   arr.splice(0, 1);
来源：http://hz.sweek.top/gtcfdpayfp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.wangdashe.top/gtwgsolmkj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cheryme.top/gtzfvnojax.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jiagoushi.top/gttrkhqxqy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.wangdashe.top/gtyyzdzszv.html

[D05] 访问与修改元素
来源：http://hz.yonumen.top/gtumzovhrd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.c1oappe.top/gtbkgbkzko.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xinyue.icu/gtqggbrvus.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.kuanghao11.cn/gtbqthbkmw.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.chenzaomai.com/gtuyzzktyt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.quarkkingdee.top/gtsxtrrzjp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtkkkgjwpo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtykswqqrh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cucudq.cn/gtdmpdnsih.html

[D06] 数组长度
来源：http://hz.mhx1999.top/gtspaypmwu.html

Py:   len(arr)
来源：http://hz.yuanzhike.top/gtjvkusawh.html

PHP:  count($arr);
来源：http://hz.ivvv.top/gtfmztnsgm.html

JS:   arr.length
来源：http://hz.yueranfly.top/gtttqdqzvx.html

TS:   arr.length
来源：http://hz.nanxinkj.top/gtehwzltjm.html

Java: list.size();
来源：http://hz.yvedp.cn/gtmjfklzyf.html

Go:   len(arr)
来源：http://hz.jyoumei.cn/gtxiwilqit.html

Ruby: arr.length; arr.size
来源：http://hz.wangdashe.top/gtannyqlzc.html

C#:   list.Count;
来源：http://hz.yj20258.top/gtgabiycva.html

[D07] 切片 / 取子数组
来源：http://hz.guannengcc.top/gtykyzqjtq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhiwuduotai.top/gtgsuyitdy.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.havefunace.top/gtyuouthdt.html

JS:   arr.slice(1, 4);
来源：http://hz.cashguo.top/gtyajukbtn.html

TS:   arr.slice(1, 4);
来源：http://hz.nanxinkj.top/gtegnjcqyf.html

Java: list.subList(1, 4);
来源：http://hz.sysykeji.top/gtsyzpqiso.html

Go:   arr[1:4]
来源：http://hz.vqdsnc.cn/gtitsbjauv.html

Ruby: arr[1, 3]
来源：http://hz.zhijiandao.cn/gtrdrrloqp.html

C#:   list.GetRange(1, 3);
来源：http://hz.kuanghao11.cn/gtqvtqftpm.html

[D08] 合并两个数组
来源：http://hz.ydjk.org.cn/gtanjrevlw.html

Py:   a + b;  a.extend(b)
来源：http://hz.yueranfly.top/gttmhxnoqa.html

PHP:  array_merge($a, $b);
来源：http://hz.iojbl.cn/gtnxadutka.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.bjfxy.top/gtpqfejpey.html

TS:   [...a, ...b];
来源：http://hz.c1oappe.top/gttipzmtxm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhoulong.xyz/gtpakzapjw.html

Go:   append(a, b...)
来源：http://hz.hammf.cn/gtmrwcgoyd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.andypj.xyz/gtzkktjyhu.html

C#:   a.Concat(b).ToList()
来源：http://hz.kuanghao11.cn/gtqvnajjai.html

[D09] 排序（升序）
来源：http://hz.yanxiufei.cn/gtkkkridew.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cucudq.cn/gtqwrtmlxw.html

PHP:  sort($arr);
来源：http://hz.tian-w.cn/gtofmjafog.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.nanxuanxn.top/gtchshyyjb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.pycfn.com/gtjdsgejmw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.fzhhl.top/gtdlktowpp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shanyushiyangtech.top/gtycnujahh.html

Ruby: arr.sort
来源：http://hz.pycfn.com/gtqpgslmdo.html

C#:   list.Sort();
来源：http://hz.yongpay.top/gtmdppuqhw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.wangshuangyany.cn/gtdwqszias.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xinyue.icu/gtskjppyky.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aibaodan.cn/gtunwmjsgj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cashguo.top/gtmskrgonq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.redwolf501.top/gtjhrfdzpo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.wangshuangyany.cn/gteiqpocxp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jlsjyb.cn/gtcwxwpadm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yuxming.cn/gtvamhdwzs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj202588.top/gtlrxvvlhm.html

[D11] 反转数组
来源：http://hz.aizwys.cn/gtiorbikze.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xingfuxueyuan.xyz/gttxjtyvpd.html

PHP:  array_reverse($arr);
来源：http://hz.jlsjyb.cn/gtaqwtrpbp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.andypj.xyz/gtuelxfhfw.html

TS:   [...arr].reverse();
来源：http://hz.hongshengwenyu.top/gtqvvrgydq.html

Java: Collections.reverse(list);
来源：http://hz.daxiang520.top/gtgvrissce.html

Go:   slices.Reverse(arr)
来源：http://hz.cqqwz.cn/gthpwfnbnh.html

Ruby: arr.reverse
来源：http://hz.xuanzx.com/gtvjqjyelk.html

C#:   list.Reverse();
来源：http://hz.chenjidiqi.icu/gtbxdhapln.html

[D12] 查找元素下标
来源：http://hz.316326.xyz/gtrnonflpp.html

Py:   arr.index(x);  x in arr
来源：http://hz.wangshuangyany.cn/gtuetgxnnc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ydzc1.top/gtancuwzmf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xinyue.icu/gtdgrifcpt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daxiang520.top/gtfqnrqxlj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gaohongyu789.top/gtbgwtqzak.html

Go:   slices.Index(arr, x)
来源：http://hz.hnqzz.top/gthwxkmchq.html

Ruby: arr.index(x)
来源：http://hz.cashguo.top/gtguqefwun.html

C#:   list.IndexOf(x);
来源：http://hz.nwbrower.top/gtjkvwcnfc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.iojbl.cn/gtsxodaezk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.aibaodan.cn/gtqbqxhcjr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yuxming.cn/gtobsjwhjm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinghuilouyu.cn/gtymagcdzp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sysykeji.top/gtmjrqmzll.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhaomingkeji.xyz/gtjaditlbu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.fzhhl.top/gtkztloisa.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xingfuxueyuan.xyz/gtfiqxwdiz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zdqjudy.top/gtdojfasdr.html

[D14] 映射转换（每个元素变形）
来源：http://hz.52xcode.cn/gtjicmgnvl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhongyouzk.top/gtdevipnfw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinqigfzy.top/gtvhndpkdy.html

JS:   arr.map(x => x * 2)
来源：http://hz.cucudq.cn/gtuglfvhkq.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gtsycehfek.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhengqikj.top/gtwoupvbil.html

Go:   // 手写循环
来源：http://hz.hywenlv.cn/gtuvbuoqzd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinghuilouyu.cn/gtgkpfuulw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.daxiang520.top/gttbikmjnp.html

[D15] 去重
来源：http://hz.pengpengdd.cyou/gtktrpkzih.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ehwqpu.com/gtvjupyktl.html

PHP:  array_unique($arr);
来源：http://hz.yanxiufei.cn/gtmghsxctd.html

JS:   [...new Set(arr)]
来源：http://hz.wangshuangyany.cn/gtuyqagxpc.html

TS:   [...new Set(arr)]
来源：http://hz.hywenlv.cn/gtugpsrhmi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.pengpengdd.cyou/gtotejnwbw.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.chenzaomai.com/gtdmgcfdhb.html

Ruby: arr.uniq
来源：http://hz.9152youxi.cn/gtjdwrhwfw.html

C#:   list.Distinct().ToList()
来源：http://hz.jinyuanbaomall.cn/gtibjcopsg.html

[D16] 求和与平均值
来源：http://hz.yvedp.cn/gtrukgysxe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sufxvd.cn/gtackenqxm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yonumen.top/gtzaoewmsf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtkxcmbtud.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj202588.top/gtccbdtubs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinqigfzy.top/gtvaodygna.html

Go:   // 手写循环累加
来源：http://hz.yonumen.top/gtfavqyfrs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xuetiantiany.cn/gtmagkxfib.html

C#:   list.Sum();  list.Average()
来源：http://hz.gaohongyu789.top/gtlrpsqlpy.html

[D17] 最大值与最小值
来源：http://hz.bjfxy.top/gtdilutfft.html

Py:   max(arr);  min(arr)
来源：http://hz.feifeiyinyue.top/gtwlmimyur.html

PHP:  max($arr);  min($arr);
来源：http://hz.0kj1m.cn/gtgwganwtj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.nanxinkj.top/gtxactbqsu.html

TS:   Math.max(...arr);
来源：http://hz.haohaochexian.top/gthlvpcjwm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sufxvd.cn/gtsoioxecy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jqgfzy.top/gthofxprxz.html

Ruby: arr.max;  arr.min
来源：http://hz.shzxlz.cn/gtaokahkjb.html

C#:   list.Max();  list.Min()
来源：http://hz.hnqzz.top/gtbqubejql.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangkeji.top/gtfaekcrea.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.aizwys.cn/gtmnsjdeny.html

PHP:  array_merge(...$nested);
来源：http://hz.vqdsnc.cn/gtudmeegsh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhoulong.xyz/gtiqwjvgie.html

TS:   nested.flat();
来源：http://hz.andypj.xyz/gtuimfbqlm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xinyue.icu/gtowlaguwn.html

Go:   // 手写双层循环
来源：http://hz.zhijiandao.cn/gtwugjzdey.html

Ruby: nested.flatten
来源：http://hz.cdnleiting.top/gtkybbkeoz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.snrcjt.cn/gtcauljiiu.html

[D19] 按字段分组
来源：http://hz.jlsjyb.cn/gtojiqcwvh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.vqdsnc.cn/gttscxctmx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.gogol.net.cn/gtqctjgxct.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.guannengcc.top/gtnxhdpbbo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sxryk.cn/gtjlghhxtp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jqgfzy.top/gtvlsuhlpq.html

Go:   // 手写 map[string][]T
来源：http://hz.gotoacloud.top/gtgjzlquyc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gogol.net.cn/gtvngxizpk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.tanke756.top/gtiajtidvx.html

[D20] 统计每个元素出现次数
来源：http://hz.yonumen.top/gtibojqrkp.html

Py:   Counter(arr)
来源：http://hz.xingfuxueyuan.xyz/gtweqyywiy.html

PHP:  array_count_values($arr);
来源：http://hz.guowangkeji.top/gtqxcukwaz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ppjwa.cn/gtpeuwiezd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhixingplan.top/gtynloyqxk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dashuyun.cn/gtvpepnrgs.html

Go:   // 手写 map[T]int
来源：http://hz.nanxinkj.top/gtnjvcfzhl.html

Ruby: arr.tally
来源：http://hz.yongpay.top/gtbsayqgbg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj202588.top/gtloqlhrfv.html

[D21] 判断是否包含某元素
来源：http://hz.ydjk.org.cn/gtjwzagxiu.html

Py:   x in arr
来源：http://hz.nanxuanxn.top/gtaqdccmdt.html

PHP:  in_array($x, $arr, true);
来源：http://hz.c1oappe.top/gtqnlznzbu.html

JS:   arr.includes(x)
来源：http://hz.chenlongwang.top/gtiloatnsh.html

TS:   arr.includes(x)
来源：http://hz.quarkkingdee.top/gtnmwxuwfd.html

Java: list.contains(x)
来源：http://hz.cashguo.top/gtgxdwbpke.html

Go:   slices.Contains(arr, x)
来源：http://hz.sysykeji.top/gtawaxogdn.html

Ruby: arr.include?(x)
来源：http://hz.zhiwuduotai.top/gthrtcdlbm.html

C#:   list.Contains(x)
来源：http://hz.shanyushiyangtech.top/gtemboqpwk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shangyingyoupin.top/gtyullmzgl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.fengsongda.top/gtavsxdfyd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jyoumei.cn/gtglauilqb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.316326.xyz/gtbweoqnbu.html

TS:   [...arr];
来源：http://hz.jqgfzy.top/gtdmpsneqz.html

Java: new ArrayList<>(list);
来源：http://hz.gzhubu.top/gtmquwglrd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yangfankeji.com/gtuibetdsy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yangfankeji.com/gtzybphkqb.html

C#:   new List<int>(list);
来源：http://hz.chenlongwang.top/gtsyhqzhhe.html

[D23] reduce 累积计算
来源：http://hz.tian-w.cn/gtwknwlzhq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.svipenyu.cn/gtskfetgpg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.pycfn.com/gtznzsfgyi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tian-w.cn/gtybweofxl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhoulong.xyz/gtywklrwoc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.guannengcc.top/gtlojfepbl.html

Go:   // 手写循环
来源：http://hz.havefunace.top/gtooivapsd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.dianchejie.cn/gtjddipgya.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cashguo.top/gtogisjwfd.html

[D24] 字典 / Map 基本操作
来源：http://hz.shzxlz.cn/gtvpjmmwcf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.svipenyu.cn/gtgjmzibtc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yongpay.top/gtimtkxkqy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hnqzz.top/gtthigisjv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.tian-w.cn/gtfnqozvyq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinqigfzy.top/gtfpfhbjsr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.tanke756.top/gtckcxeljx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hnxiangtu.top/gtevpobmka.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhengqikj.top/gtnbbkoptz.html

[D25] Set 集合去重与交并差
来源：http://hz.jqgfzy.top/gtfvtgklse.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xuetiantiany.cn/gtlbgqbgpk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenzaomai.com/gtjmwbqkes.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yangfankeji.com/gtimolvycz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hammf.cn/gtxyycqfsn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gzhubu.top/gtnsoosxoe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yonumen.top/gtzinfdnqt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nanxinkj.top/gtjyvyfdzb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.chenjidiqi.icu/gteqxweiap.html

[D26] 数组转字符串
来源：http://hz.ydzc1.top/gtgoguzwjj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jyoumei.cn/gtbirmfjxh.html

PHP:  implode(", ", $arr);
来源：http://hz.xuetiantiany.cn/gtrnsfdqbx.html

JS:   arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtjkkdtyai.html

TS:   arr.join(", ")
来源：http://hz.yanxiufei.cn/gtevroamqy.html

Java: String.join(", ", list)
来源：http://hz.yvedp.cn/gtgxidlwuv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nanxuanxn.top/gtveryggdl.html

Ruby: arr.join(", ")
来源：http://hz.ydjk.org.cn/gtolwbiusd.html

C#:   string.Join(", ", list)
来源：http://hz.birdmap.top/gthmaskser.html

================================================================================
来源：http://hz.jinqigufen.top/gtafdheynk.html

E. 字符串处理
来源：http://hz.jinqigfzy.top/gtbuxnvnud.html

================================================================================
来源：http://hz.zhongyouzk.top/gtccnwqkrk.html

[E01] 拼接字符串
来源：http://hz.yuanzhike.top/gtdzrvgmsb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhijiandao.cn/gtwmfhpspb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.chenjidiqi.icu/gtfnbgsyeh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuanzx.com/gterdafefw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.smart0.xyz/gtocfrajnh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.smart0.xyz/gtccukmgtj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jqgufenzy.top/gtwwjbqrui.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sysykeji.top/gtlnrxukus.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.aizwys.cn/gtaamsnpje.html

[E02] 重复字符串
来源：http://hz.cashguo.top/gthtsnzoin.html

Py:   "ab" * 3
来源：http://hz.feifeiyinyue.top/gtlckfhlpi.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ppjwa.cn/gtyjmifcfn.html

JS:   "ab".repeat(3)
来源：http://hz.birdmap.top/gtakexvinq.html

TS:   "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtekhjqxbs.html

Java: "ab".repeat(3)
来源：http://hz.xuanzx.com/gtvwnvvwno.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hywenlv.cn/gtlythenbh.html

Ruby: "ab" * 3
来源：http://hz.xinyue.icu/gtqxicvtnb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yvedp.cn/gtcoaowsym.html

[E03] 截取子串
来源：http://hz.havefunace.top/gtqmesuoeu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tianlin.xyz/gtrojcacwb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gzhubu.top/gtueoaehus.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtwcsbwwze.html

TS:   s.slice(1, 4)
来源：http://hz.zhoulong.xyz/gtvkucdzfd.html

Java: s.substring(1, 4)
来源：http://hz.jinqigfzy.top/gtoatfnvvh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.aibaodan.cn/gtkiuccycu.html


<!-- 参考信息 -->