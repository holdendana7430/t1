代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cdnleiting.top/gtvmuqbthw.html

Go:   func add(a, b int) int
来源：http://hz.shzxlz.cn/gtlrijktcy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuxming.cn/gtnmcwsgqx.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.vqdsnc.cn/gtjxzhzsbd.html

[C14] 泛型函数
来源：http://hz.zdqjudy.top/gtuvmabjdz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.wangshuangyany.cn/gtsxnxickn.html

PHP:  // 无泛型
来源：http://hz.shuidangran.top/gtbzldabho.html

JS:   // 无泛型
来源：http://hz.cashguo.top/gtjuzwvsfx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.52xcode.cn/gtyyhvygoz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.kuanghao11.cn/gtfbxuisvf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yj202588.top/gttnmagwuy.html

Ruby: # 无泛型
来源：http://hz.fzhhl.top/gtsaodfmqd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jlsjyb.cn/gtikniwixa.html

[C15] 解构 / 展开参数
来源：http://hz.nanxuanxn.top/gtwbnsxjvl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.chenzaomai.com/gtbuhypspa.html

PHP:  [$a, $b] = $pair;
来源：http://hz.dianchejie.cn/gttnvfimao.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.daxiang520.top/gtfqyqcatf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yonumen.top/gtukulidvh.html

Java: // 无解构
来源：http://hz.cashguo.top/gtcnnbdllt.html

Go:   // 无解构
来源：http://hz.hnqzz.top/gtdstvgmhl.html

Ruby: a, b = pair
来源：http://hz.aizwys.cn/gteltynwdo.html

C#:   var (a, b) = pair;
来源：http://hz.hfpthk.cn/gtjmlzqzby.html

[C16] 函数 / 方法重载
来源：http://hz.hywenlv.cn/gtohsdinwz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinqigufen.top/gtutpmkscq.html

PHP:  // 无重载
来源：http://hz.iojbl.cn/gtgyxcveqj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yanxiufei.cn/gtpncdxyrw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.chenjidiqi.icu/gtfkoenjth.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.guannengcc.top/gtewespvvp.html

Go:   // 无重载：用不同函数名
来源：http://hz.ybcxt.top/gtwbmwcfin.html

Ruby: # 无重载：靠动态参数
来源：http://hz.aibaodan.cn/gttbcmgmgu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.fengsongda.top/gtvcxbyufe.html

================================================================================
来源：http://hz.jqgfzy.top/gthnoinndd.html

D. 数组 / 列表 / 集合
来源：http://hz.ehwqpu.com/gtwdhkbgmk.html

================================================================================
来源：http://hz.shzxlz.cn/gtagvjqvzn.html

[D01] 创建数组 / 列表
来源：http://hz.guowangkeji.top/gtinqzphvy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yj202588.top/gtpkocwbmp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jiagoushi.top/gtnnphlzki.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shanyushiyangkeji.top/gtnnmchfzz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ehwqpu.com/gtifhiztbh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guowangkeji.top/gtdyuyoomh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hfpthk.cn/gtgmgatxgz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jinqigfzy.top/gtjlbifsed.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gogol.net.cn/gtwngqmktp.html

[D02] 追加元素到末尾
来源：http://hz.yongpay.top/gtwhkrgfrb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.tanke756.top/gtakrmepbu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cheryme.top/gtvcdzmtrq.html

JS:   arr.push(4);
来源：http://hz.tianlin.xyz/gttouroder.html

TS:   arr.push(4);
来源：http://hz.zhongyouzk.top/gttmstthki.html

Java: list.add(4);
来源：http://hz.yj202588.top/gtzpqfizsi.html

Go:   arr = append(arr, 4)
来源：http://hz.yongpay.top/gtebxgpuyv.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.c1oappe.top/gtpvzwamfl.html

C#:   list.Add(4);
来源：http://hz.haohaochexian.top/gtmpwmtbww.html

[D03] 在指定位置插入元素
来源：http://hz.nwbrower.top/gtbqldwoyk.html

Py:   arr.insert(0, 0)
来源：http://hz.dashuyun.cn/gtpmweuaef.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.fzhhl.top/gtvcdyzxne.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.feifeiyinyue.top/gtwpuaetoa.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.0kj1m.cn/gtahnmihbw.html

Java: list.add(0, 0);
来源：http://hz.guowangkeji.top/gtzwhlijvm.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.tian-w.cn/gtgtcfsqzd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.svipenyu.cn/gtlylsghuh.html

C#:   list.Insert(0, 0);
来源：http://hz.gotoacloud.top/gtvaznjjwd.html

[D04] 删除元素
来源：http://hz.nwbrower.top/gtwvmfgdyn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ivvv.top/gtzuutkolk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hammf.cn/gteusobmpr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hammf.cn/gtmqezldmt.html

TS:   arr.splice(0, 1);
来源：http://hz.cashguo.top/gtzrpjgabx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xylfe.cn/gtbhnlibei.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yuxming.cn/gtgfmmoskb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xingfuxueyuan.xyz/gtydwirfik.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hnqzz.top/gtusqsveiq.html

[D05] 访问与修改元素
来源：http://hz.jlsjyb.cn/gtsswebbim.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnqzz.top/gtcizopxuf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gaohongyu789.top/gtuexsucsh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ivvv.top/gtwqwftqav.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yangfankeji.com/gtjqvgvyci.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.daria6918.cn/gtfibunajd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.pycfn.com/gtcupyxjfa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pycfn.com/gtbmfdbvdb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangshuangyany.cn/gtrzktjlgc.html

[D06] 数组长度
来源：http://hz.guowangkeji.top/gtothitwhg.html

Py:   len(arr)
来源：http://hz.xinyue.icu/gtdafwrxdw.html

PHP:  count($arr);
来源：http://hz.tanke756.top/gtzgihgnpz.html

JS:   arr.length
来源：http://hz.cqqwz.cn/gtptoqnsof.html

TS:   arr.length
来源：http://hz.guannengcc.top/gtipyuamxu.html

Java: list.size();
来源：http://hz.daxiang520.top/gtuemltfjg.html

Go:   len(arr)
来源：http://hz.smart0.xyz/gtqimnffwl.html

Ruby: arr.length; arr.size
来源：http://hz.vqdsnc.cn/gtnoryfmuw.html

C#:   list.Count;
来源：http://hz.sxryk.cn/gthiszqyff.html

[D07] 切片 / 取子数组
来源：http://hz.aizwys.cn/gtlzmtxgwx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhengqikj.top/gthudhfjef.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gogol.net.cn/gtxyowdmlq.html

JS:   arr.slice(1, 4);
来源：http://hz.yj20258888.top/gtketibhpi.html

TS:   arr.slice(1, 4);
来源：http://hz.chenzaomai.com/gtvjlwuflz.html

Java: list.subList(1, 4);
来源：http://hz.tianlin.xyz/gtfdyekrhg.html

Go:   arr[1:4]
来源：http://hz.xinyue.icu/gtamdyxuvz.html

Ruby: arr[1, 3]
来源：http://hz.ivvv.top/gtmwiajnfc.html

C#:   list.GetRange(1, 3);
来源：http://hz.jiagoushi.top/gtvfbpwnhm.html

[D08] 合并两个数组
来源：http://hz.ydjk.org.cn/gtjudxjmtx.html

Py:   a + b;  a.extend(b)
来源：http://hz.gzhubu.top/gtmlcpyrzv.html

PHP:  array_merge($a, $b);
来源：http://hz.guowangkeji.top/gtnyxdgulm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.meibo888.top/gtpbctynoj.html

TS:   [...a, ...b];
来源：http://hz.gotoacloud.top/gtseehojle.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hysaishi.cn/gtxaoqdzzn.html

Go:   append(a, b...)
来源：http://hz.316326.xyz/gtynxhbdzz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.fengsongda.top/gtodtrdpoz.html

C#:   a.Concat(b).ToList()
来源：http://hz.xylfe.cn/gtuwmdmqtn.html

[D09] 排序（升序）
来源：http://hz.iojbl.cn/gtyvicsfon.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangkeji.top/gtvaiqnior.html

PHP:  sort($arr);
来源：http://hz.yvedp.cn/gturasmdmx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ydjk.org.cn/gtryfumhie.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.guowangkeji.top/gtgrzxwifw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhixingplan.top/gtyyvqsrow.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hammf.cn/gtdmsrsgfd.html

Ruby: arr.sort
来源：http://hz.ywan-chungtsiang.top/gtdectrkfy.html

C#:   list.Sort();
来源：http://hz.c1oappe.top/gtkfnkgkom.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.wangdashe.top/gtysykwlhl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ppjwa.cn/gtvizaiuaj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinghuilouyu.cn/gtoxkqlyou.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhongyouzk.top/gtruoiztji.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ehwqpu.com/gtdcypigmx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.bjfxy.top/gtekomxrdr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gotoacloud.top/gtydwkntjt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.quarkkingdee.top/gtjfiwxdiw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.feifeiyinyue.top/gtaldfpftd.html

[D11] 反转数组
来源：http://hz.c1oappe.top/gtklbcxohr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sweek.top/gthuxfllhf.html

PHP:  array_reverse($arr);
来源：http://hz.guowangkeji.top/gtmrplotqd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hfpthk.cn/gtwtbziqnb.html

TS:   [...arr].reverse();
来源：http://hz.dianchejie.cn/gtnmowfnxy.html

Java: Collections.reverse(list);
来源：http://hz.hnxiangtu.top/gtilvsalko.html

Go:   slices.Reverse(arr)
来源：http://hz.gogol.net.cn/gtsrdarxsl.html

Ruby: arr.reverse
来源：http://hz.cucudq.cn/gtjkccsgtw.html

C#:   list.Reverse();
来源：http://hz.gaohongyu789.top/gtqzujoxrs.html

[D12] 查找元素下标
来源：http://hz.yonumen.top/gtkqnpfxlv.html

Py:   arr.index(x);  x in arr
来源：http://hz.jiagoushi.top/gtdwkanffj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.pengpengdd.cyou/gtupmjifbr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigufen.top/gtthdwxgrh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gogol.net.cn/gtcxolxlls.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tanke756.top/gtbkddwjzk.html

Go:   slices.Index(arr, x)
来源：http://hz.zhengqikj.top/gtbzvpvoir.html

Ruby: arr.index(x)
来源：http://hz.jinqigfzy.top/gtobzmzgay.html

C#:   list.IndexOf(x);
来源：http://hz.shuidangran.top/gthkdqutxo.html

[D13] 过滤（保留满足条件的）
来源：http://hz.chenzaomai.com/gtzrzusmbs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.quarkkingdee.top/gtlqkyneqr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yvedp.cn/gtueuxfefz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.tanke756.top/gtgyjrfpvs.html

TS:   arr.filter(x => x > 3)
来源：http://hz.aizwys.cn/gtguxurdjx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gaohongyu789.top/gtypqkcgun.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhiwuduotai.top/gtegvggerz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.mhx1999.top/gtznkyqhcd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hammf.cn/gtbawlqyzi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jiagoushi.top/gtoolnloyg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.nwbrower.top/gtnducbplh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhongyouzk.top/gtljunhwht.html

JS:   arr.map(x => x * 2)
来源：http://hz.dashuyun.cn/gtrjmgkigp.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhengqikj.top/gtfinpjndf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.mhx1999.top/gtyxgykthb.html

Go:   // 手写循环
来源：http://hz.yangfankeji.com/gtusuuaftk.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.vqdsnc.cn/gtxlnmaego.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hnqzz.top/gtlkshbxbv.html

[D15] 去重
来源：http://hz.sysykeji.top/gtilijwrsy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hongshengwenyu.top/gtbxwwckxq.html

PHP:  array_unique($arr);
来源：http://hz.shangyingyoupin.top/gtbhysefhg.html

JS:   [...new Set(arr)]
来源：http://hz.yvedp.cn/gtnumpzifn.html

TS:   [...new Set(arr)]
来源：http://hz.zhengqikj.top/gthwpdryny.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sxryk.cn/gtcabndvap.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.daxiang520.top/gtoeobtokl.html

Ruby: arr.uniq
来源：http://hz.yj202588.top/gtbyzdbhkv.html

C#:   list.Distinct().ToList()
来源：http://hz.nanxuanxn.top/gtjbqbcdao.html

[D16] 求和与平均值
来源：http://hz.yanxiufei.cn/gtfarsppyz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.meibo888.top/gtjqwxgcjs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yangfankeji.com/gtnommznqj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.snrcjt.cn/gtuqoqtpbt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xinyue.icu/gtzvcewoqo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.bjfxy.top/gtixzzpwvl.html

Go:   // 手写循环累加
来源：http://hz.pycfn.com/gtkvqiaemx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yanxiufei.cn/gtmxbxmued.html

C#:   list.Sum();  list.Average()
来源：http://hz.fengsongda.top/gtehjpzozv.html

[D17] 最大值与最小值
来源：http://hz.kuanghao11.cn/gtqwaimuqu.html

Py:   max(arr);  min(arr)
来源：http://hz.sufxvd.cn/gtyukqpwkt.html

PHP:  max($arr);  min($arr);
来源：http://hz.ydjk.org.cn/gtptnoahrv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tian-w.cn/gtmslximtp.html

TS:   Math.max(...arr);
来源：http://hz.yj202588.top/gtyyjntghz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.iojbl.cn/gtrhlqgnrj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.316326.xyz/gtbpuuyddu.html

Ruby: arr.max;  arr.min
来源：http://hz.cheryme.top/gtbaklyqye.html

C#:   list.Max();  list.Min()
来源：http://hz.xziqi.cn/gtirqbggxg.html

[D18] 扁平化嵌套数组
来源：http://hz.yj20258.top/gtblwagpkd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yvedp.cn/gtzkwqgtau.html

PHP:  array_merge(...$nested);
来源：http://hz.hongshengwenyu.top/gtbdnsaake.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhoulong.xyz/gtkglktspi.html

TS:   nested.flat();
来源：http://hz.feifeiyinyue.top/gtujhdmccr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinyuanbaomall.cn/gtmztosptb.html

Go:   // 手写双层循环
来源：http://hz.mhx1999.top/gtrolcjoqs.html

Ruby: nested.flatten
来源：http://hz.shanyushiyangtech.top/gtepthakpe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.wangdashe.top/gtgtacmwpk.html

[D19] 按字段分组
来源：http://hz.316326.xyz/gtmmnqazqx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.gotoacloud.top/gtstmzsqll.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.daxiang520.top/gtaafhllty.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ywan-chungtsiang.top/gtyjsqacqx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.nwbrower.top/gtyqiakbdl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.9152youxi.cn/gtwoiztcur.html

Go:   // 手写 map[string][]T
来源：http://hz.jinqigufen.top/gtbqbwnpje.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cdnleiting.top/gtkrqxzilv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.andypj.xyz/gtplrmxzif.html

[D20] 统计每个元素出现次数
来源：http://hz.cdnleiting.top/gtafsbpyns.html

Py:   Counter(arr)
来源：http://hz.zhiwuduotai.top/gtwalctzof.html

PHP:  array_count_values($arr);
来源：http://hz.jyoumei.cn/gtsavfcxds.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yanxiufei.cn/gttepfivbb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pycfn.com/gtbcnhelmw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinqigfzy.top/gtgzrgdwyp.html

Go:   // 手写 map[T]int
来源：http://hz.cashguo.top/gttfutrwlh.html

Ruby: arr.tally
来源：http://hz.zhiwuduotai.top/gtqrntyihc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.316326.xyz/gtvoyemyqz.html

[D21] 判断是否包含某元素
来源：http://hz.zhoulong.xyz/gtxalnfnkl.html

Py:   x in arr
来源：http://hz.jyoumei.cn/gtwimscqec.html

PHP:  in_array($x, $arr, true);
来源：http://hz.kuanghao11.cn/gtabgbqthn.html

JS:   arr.includes(x)
来源：http://hz.dianchejie.cn/gttrergaeg.html

TS:   arr.includes(x)
来源：http://hz.nanxinkj.top/gtgdcphelt.html

Java: list.contains(x)
来源：http://hz.redwolf501.top/gtckmflolg.html

Go:   slices.Contains(arr, x)
来源：http://hz.meibo888.top/gtxgnfwkop.html

Ruby: arr.include?(x)
来源：http://hz.sweek.top/gtayesuyoz.html

C#:   list.Contains(x)
来源：http://hz.jqgufenzy.top/gtcmzzxfbr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ppjwa.cn/gtuqckaemr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhoulong.xyz/gtvylrzvbg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jqgufenzy.top/gtvhaexjea.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.andypj.xyz/gtgffykrrl.html

TS:   [...arr];
来源：http://hz.xinyue.icu/gtqwlicokg.html

Java: new ArrayList<>(list);
来源：http://hz.tian-w.cn/gttklgyrdc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jqgufenzy.top/gteiqgtals.html

Ruby: arr.dup;  arr.clone
来源：http://hz.c1oappe.top/gtlryxrcbz.html

C#:   new List<int>(list);
来源：http://hz.zhengqikj.top/gtxguyqciw.html

[D23] reduce 累积计算
来源：http://hz.guowangkeji.top/gtessleemb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xinyue.icu/gtsqviowdx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.smart0.xyz/gtaovapwgp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.vqdsnc.cn/gtpxarttse.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gtysgmehkg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj202588.top/gtfjnahzjo.html

Go:   // 手写循环
来源：http://hz.52xcode.cn/gttyuewicu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cdnleiting.top/gtsfapvbhc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cashguo.top/gtwpulmcwq.html

[D24] 字典 / Map 基本操作
来源：http://hz.ywan-chungtsiang.top/gtcjertpoe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.redwolf501.top/gtgzeufkei.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.guannengcc.top/gtytlignph.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.fengsongda.top/gtbzdaizux.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ydzc1.top/gtnrasxfex.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhiwuduotai.top/gtuyuluamm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xingfuxueyuan.xyz/gttsmcoyos.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinqigfzy.top/gtvlvemwxa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.aibaodan.cn/gthndaqama.html

[D25] Set 集合去重与交并差
来源：http://hz.wangshuangyany.cn/gtoxghgqjv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shangyingyoupin.top/gtysamrwyb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.mhx1999.top/gtgcuhvmjy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhaomingkeji.xyz/gtpjfdykfz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cashguo.top/gthxroqiiq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.redwolf501.top/gtikuccdms.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.guowangkeji.top/gtlnhwlmws.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.0kj1m.cn/gtghkpmdbs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shzxlz.cn/gtniuakanf.html

[D26] 数组转字符串
来源：http://hz.pengpengdd.cyou/gtvalmcoxr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sufxvd.cn/gthplgjcqa.html

PHP:  implode(", ", $arr);
来源：http://hz.fzhhl.top/gtiofftjjp.html

JS:   arr.join(", ")
来源：http://hz.ybcxt.top/gtoiucqhpp.html

TS:   arr.join(", ")
来源：http://hz.0kj1m.cn/gtaprdwpwo.html

Java: String.join(", ", list)
来源：http://hz.cucudq.cn/gtvelvumlx.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gotoacloud.top/gtuqxmrvto.html

Ruby: arr.join(", ")
来源：http://hz.ydzc1.top/gtkpjyxupt.html

C#:   string.Join(", ", list)
来源：http://hz.sysykeji.top/gtzvfypeyg.html

================================================================================
来源：http://hz.vqdsnc.cn/gtnprmfrax.html

E. 字符串处理
来源：http://hz.redwolf501.top/gtmboqyrcz.html

================================================================================
来源：http://hz.zycfv.cn/gtvifkydpv.html

[E01] 拼接字符串
来源：http://hz.daria6918.cn/gtnjfxappc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sweek.top/gtqpcakdqv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhijiandao.cn/gtlyvynnrt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gtisuxijtf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gtpiuceqkh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.iojbl.cn/gtaeiyxhfu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.birdmap.top/gtbugsumsx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hysaishi.cn/gtqrxopudm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sufxvd.cn/gtqbsfqdsm.html

[E02] 重复字符串
来源：http://hz.jinghuilouyu.cn/gtptaoannq.html

Py:   "ab" * 3
来源：http://hz.yongpay.top/gtvczxqqwu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fzhhl.top/gtrrijcghh.html

JS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gtepnpoyyc.html

TS:   "ab".repeat(3)
来源：http://hz.chenjidiqi.icu/gtubtjnqmo.html

Java: "ab".repeat(3)
来源：http://hz.xinyue.icu/gtlktqxmpq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.daxiang520.top/gtaedquhzp.html

Ruby: "ab" * 3
来源：http://hz.smart0.xyz/gtyrzfjqhe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nanxinkj.top/gtbggqevno.html

[E03] 截取子串
来源：http://hz.jyoumei.cn/gtsmbbhkze.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ppjwa.cn/gttpzksorz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.iojbl.cn/gtybdhugaj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinqigufen.top/gtvpwnxhid.html

TS:   s.slice(1, 4)
来源：http://hz.hnqzz.top/gtpdcchugq.html

Java: s.substring(1, 4)
来源：http://hz.hfpthk.cn/gtswcganpm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cdnleiting.top/gtlzoeibkb.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.snrcjt.cn/gtjaaysujr.html

C#:   s.Substring(1, 3)
来源：http://hz.nwbrower.top/gtyhobgamn.html

[E04] 查找子串位置
来源：http://hz.wangshuangyany.cn/gtobrrbrvd.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cheryme.top/gtjxxetmkz.html


<!-- 参考信息 -->