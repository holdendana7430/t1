代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shanyushiyangtech.top/gtasvntork.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.9152youxi.cn/gtpyyfqodz.html

Java: // 无解构
来源：http://hz.cheryme.top/gtsbnhmuzc.html

Go:   // 无解构
来源：http://hz.haohaochexian.top/gtoedaswgb.html

Ruby: a, b = pair
来源：http://hz.redwolf501.top/gtiorzybhc.html

C#:   var (a, b) = pair;
来源：http://hz.ywan-chungtsiang.top/gtsmlnduvj.html

[C16] 函数 / 方法重载
来源：http://hz.cashguo.top/gtcdwwyhhs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.wangdashe.top/gteyjfeckt.html

PHP:  // 无重载
来源：http://hz.ivvv.top/gtaroynpss.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.wangdashe.top/gtahaqhxra.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tianlin.xyz/gtgofyqfpj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.gzhubu.top/gtadjwgqvx.html

Go:   // 无重载：用不同函数名
来源：http://hz.ydzc1.top/gtdtijxrtv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xziqi.cn/gttuiynpaq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.sxryk.cn/gtencskocw.html

================================================================================
来源：http://hz.yj20258888.top/gteooqryln.html

D. 数组 / 列表 / 集合
来源：http://hz.zycfv.cn/gtqeylouiy.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtqcynouqf.html

[D01] 创建数组 / 列表
来源：http://hz.shuidangran.top/gtzbfqacwq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.daria6918.cn/gtprqqrnsz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinqigfzy.top/gtfhqsdavs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.fengsongda.top/gtfxoyemur.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.meibo888.top/gtedjsblfd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.haohaochexian.top/gtgilnxcxd.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ybcxt.top/gtwrddosso.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhengqikj.top/gtoldgvohn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ydzc1.top/gtsswwxylw.html

[D02] 追加元素到末尾
来源：http://hz.zhengqikj.top/gtrysaeaqb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.c1oappe.top/gtlgrufxfj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hongshengwenyu.top/gtpuyaoblg.html

JS:   arr.push(4);
来源：http://hz.cucudq.cn/gtuefevbqc.html

TS:   arr.push(4);
来源：http://hz.jianghu66.top/gtaebswilq.html

Java: list.add(4);
来源：http://hz.yuxming.cn/gtylzbhzdb.html

Go:   arr = append(arr, 4)
来源：http://hz.sufxvd.cn/gtskrydvcn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.svipenyu.cn/gtufgpqgbi.html

C#:   list.Add(4);
来源：http://hz.jinqigufen.top/gtfudcrobf.html

[D03] 在指定位置插入元素
来源：http://hz.ydjk.org.cn/gteceepcmr.html

Py:   arr.insert(0, 0)
来源：http://hz.shuidangran.top/gtsidwwixj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sufxvd.cn/gtbtjdzexi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zdqjudy.top/gtmrhxedaw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jianghu66.top/gtesrhhmhw.html

Java: list.add(0, 0);
来源：http://hz.andypj.xyz/gtqgbopbzn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.c1oappe.top/gtqyumgqyy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhengqikj.top/gtzlzntyvy.html

C#:   list.Insert(0, 0);
来源：http://hz.cqqwz.cn/gtoefokoqq.html

[D04] 删除元素
来源：http://hz.yvedp.cn/gtpvqizjce.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yuxming.cn/gtnrnmjelc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhongyouzk.top/gtdobggpgx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sysykeji.top/gthfidermq.html

TS:   arr.splice(0, 1);
来源：http://hz.kuanghao11.cn/gtgrqbotnf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yj202588.top/gtblzeucpn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jqgufenzy.top/gtzezmzaam.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinqigfzy.top/gtswtncmrs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.gzhubu.top/gtugacwakb.html

[D05] 访问与修改元素
来源：http://hz.ivvv.top/gtcydpbrsk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtdptpbwjk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhijiandao.cn/gtmvyjaspu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinqigfzy.top/gtxfrryybs.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cdnleiting.top/gtbcwbxiqf.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jyoumei.cn/gtrdlbebbz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cheryme.top/gtjleuobal.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gtjyxvfnnz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.svipenyu.cn/gtrcxevdmg.html

[D06] 数组长度
来源：http://hz.gzhubu.top/gtluvtcgjg.html

Py:   len(arr)
来源：http://hz.zycfv.cn/gtlfdqatmm.html

PHP:  count($arr);
来源：http://hz.cheryme.top/gtcpysgcpp.html

JS:   arr.length
来源：http://hz.nwbrower.top/gtnglfuvof.html

TS:   arr.length
来源：http://hz.zhengqikj.top/gtgpfrncvb.html

Java: list.size();
来源：http://hz.sysykeji.top/gtansmgcmj.html

Go:   len(arr)
来源：http://hz.ydzc1.top/gtuozyejqd.html

Ruby: arr.length; arr.size
来源：http://hz.pengpengdd.cyou/gtvceewrfm.html

C#:   list.Count;
来源：http://hz.snrcjt.cn/gtdnpdgjul.html

[D07] 切片 / 取子数组
来源：http://hz.shzxlz.cn/gtqbaawjmo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yonumen.top/gtjltwspnc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yangfankeji.com/gtkkwbntoj.html

JS:   arr.slice(1, 4);
来源：http://hz.yj202588.top/gtikrmzbof.html

TS:   arr.slice(1, 4);
来源：http://hz.ppjwa.cn/gtvgvxhwxs.html

Java: list.subList(1, 4);
来源：http://hz.smart0.xyz/gtpynqcbfl.html

Go:   arr[1:4]
来源：http://hz.yongpay.top/gtatsdtqyj.html

Ruby: arr[1, 3]
来源：http://hz.dianchejie.cn/gtmymuamsl.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhiwuduotai.top/gtwvemhnjo.html

[D08] 合并两个数组
来源：http://hz.tian-w.cn/gtvqydppzr.html

Py:   a + b;  a.extend(b)
来源：http://hz.yvedp.cn/gtwptgoxdl.html

PHP:  array_merge($a, $b);
来源：http://hz.dashuyun.cn/gttbxifunl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yangfankeji.com/gtfgxoijdg.html

TS:   [...a, ...b];
来源：http://hz.xziqi.cn/gtnznjtjds.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cashguo.top/gtzrxvwhrv.html

Go:   append(a, b...)
来源：http://hz.shangyingyoupin.top/gttnazywun.html

Ruby: a + b;  a.concat(b)
来源：http://hz.feifeiyinyue.top/gtaqdydsxb.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenlongwang.top/gtldtzibfi.html

[D09] 排序（升序）
来源：http://hz.fzhhl.top/gtybhisocd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.kuanghao11.cn/gtmvwbyfqo.html

PHP:  sort($arr);
来源：http://hz.sysykeji.top/gtwlvismme.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.52xcode.cn/gtduxotyig.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sxryk.cn/gtzmmyyvou.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ybcxt.top/gtawdltldo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xuetiantiany.cn/gtaibvqaou.html

Ruby: arr.sort
来源：http://hz.xinyue.icu/gtxgrdvobt.html

C#:   list.Sort();
来源：http://hz.xziqi.cn/gtgrujmoqu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.daxiang520.top/gtzwjykotc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.svipenyu.cn/gtxywxseyr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zycfv.cn/gtgpeucpwv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cashguo.top/gttgbjjzzu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ivvv.top/gtnrdsauhq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.gzhubu.top/gtioqkplcs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ydjk.org.cn/gtghrybwqa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhijiandao.cn/gtyhqixtsr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhixingplan.top/gtkeabdvvl.html

[D11] 反转数组
来源：http://hz.hongshengwenyu.top/gtvabkclam.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ivvv.top/gtzczxtyiu.html

PHP:  array_reverse($arr);
来源：http://hz.aizwys.cn/gtjgqnlkbw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yj20258888.top/gtlfvdqwsw.html

TS:   [...arr].reverse();
来源：http://hz.redwolf501.top/gteoptswih.html

Java: Collections.reverse(list);
来源：http://hz.zhiwuduotai.top/gtttbmszbh.html

Go:   slices.Reverse(arr)
来源：http://hz.gaohongyu789.top/gtbattmcam.html

Ruby: arr.reverse
来源：http://hz.chenlongwang.top/gttenacyqs.html

C#:   list.Reverse();
来源：http://hz.dashuyun.cn/gtlfonlpdh.html

[D12] 查找元素下标
来源：http://hz.zhijiandao.cn/gtspyxuoqt.html

Py:   arr.index(x);  x in arr
来源：http://hz.andypj.xyz/gtrtjmpxwg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.aibaodan.cn/gtzdeeuxhj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.quarkkingdee.top/gtgiyveaih.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yanxiufei.cn/gtrqfkldud.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.pengpengdd.cyou/gtuevjvrmr.html

Go:   slices.Index(arr, x)
来源：http://hz.smart0.xyz/gtsphuujfd.html

Ruby: arr.index(x)
来源：http://hz.pengpengdd.cyou/gtryfuwkrv.html

C#:   list.IndexOf(x);
来源：http://hz.wangshuangyany.cn/gtegbwjzjn.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ywan-chungtsiang.top/gtdnetjzao.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.meibo888.top/gtfkxoadey.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.guowangkeji.top/gtlngcudhv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.aizwys.cn/gtqaqjgbax.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhaomingkeji.xyz/gtpsfyevpj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jlsjyb.cn/gtnwzvpxgl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.pycfn.com/gtsglqygvs.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shuidangran.top/gttlvnktuz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.bjfxy.top/gtxjxjarbx.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zycfv.cn/gtnqoubfuy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xingfuxueyuan.xyz/gtfjqxinkv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.fengsongda.top/gtlyjjuvqf.html

JS:   arr.map(x => x * 2)
来源：http://hz.gogol.net.cn/gthjjteofa.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhijiandao.cn/gtjtwvlhza.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yuxming.cn/gtvzpduynx.html

Go:   // 手写循环
来源：http://hz.guannengcc.top/gttaegeovf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hnqzz.top/gtpprljuzk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ybcxt.top/gtigmjvfvd.html

[D15] 去重
来源：http://hz.hfpthk.cn/gtpellfweg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhaomingkeji.xyz/gtwppkttfo.html

PHP:  array_unique($arr);
来源：http://hz.chenzaomai.com/gteqnpbxdh.html

JS:   [...new Set(arr)]
来源：http://hz.52xcode.cn/gtvejjqdco.html

TS:   [...new Set(arr)]
来源：http://hz.yongpay.top/gtjyodgiir.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.pengpengdd.cyou/gtsxkjimer.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pengpengdd.cyou/gtjgvbmkmk.html

Ruby: arr.uniq
来源：http://hz.yj20258.top/gtscgivkme.html

C#:   list.Distinct().ToList()
来源：http://hz.ywan-chungtsiang.top/gtnfmsfujw.html

[D16] 求和与平均值
来源：http://hz.jinqigufen.top/gtwvuflndv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shangyingyoupin.top/gtcuqgjuwy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.316326.xyz/gtnwfbfgok.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.0kj1m.cn/gtclyvykwt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pengpengdd.cyou/gtjcaugtxe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jqgufenzy.top/gtuflzohaw.html

Go:   // 手写循环累加
来源：http://hz.wangshuangyany.cn/gtgpvbglin.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhiwuduotai.top/gtifdiveav.html

C#:   list.Sum();  list.Average()
来源：http://hz.hfpthk.cn/gttiewjxug.html

[D17] 最大值与最小值
来源：http://hz.gzhubu.top/gtfsjuxqby.html

Py:   max(arr);  min(arr)
来源：http://hz.iojbl.cn/gtxputvqyb.html

PHP:  max($arr);  min($arr);
来源：http://hz.9152youxi.cn/gtpbgjjfwq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jinqigfzy.top/gtbuzjinrl.html

TS:   Math.max(...arr);
来源：http://hz.svipenyu.cn/gtboracube.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ehwqpu.com/gtaiugokhg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ywan-chungtsiang.top/gtmnaexfwi.html

Ruby: arr.max;  arr.min
来源：http://hz.hnxiangtu.top/gtpumbboes.html

C#:   list.Max();  list.Min()
来源：http://hz.xinyue.icu/gtgftkbikx.html

[D18] 扁平化嵌套数组
来源：http://hz.iojbl.cn/gtiwotgvdi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jyoumei.cn/gtvipxghkp.html

PHP:  array_merge(...$nested);
来源：http://hz.chenzaomai.com/gtcqergohl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xingfuxueyuan.xyz/gtbitqaocm.html

TS:   nested.flat();
来源：http://hz.mhx1999.top/gtylrceqgc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.guannengcc.top/gtedvqaior.html

Go:   // 手写双层循环
来源：http://hz.daxiang520.top/gtfvymeqcw.html

Ruby: nested.flatten
来源：http://hz.zhengqikj.top/gtsdwjlecn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sufxvd.cn/gtyjycvpki.html

[D19] 按字段分组
来源：http://hz.birdmap.top/gtvgyifjsx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cucudq.cn/gtimtrsaoo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hongshengwenyu.top/gtlnwaeacm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhongyouzk.top/gtpksedpsx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ivvv.top/gtfezykpck.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gzhubu.top/gtxincbibh.html

Go:   // 手写 map[string][]T
来源：http://hz.redwolf501.top/gtdobgetyk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sxryk.cn/gtcqxnywpd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ydzc1.top/gtnutbdqay.html

[D20] 统计每个元素出现次数
来源：http://hz.guowangkeji.top/gtrbpnkvka.html

Py:   Counter(arr)
来源：http://hz.pycfn.com/gteumvgttd.html

PHP:  array_count_values($arr);
来源：http://hz.xylfe.cn/gtyrimpiig.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtgnndnhyh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yueranfly.top/gtamqficvg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jqgufenzy.top/gtefcbqdjw.html

Go:   // 手写 map[T]int
来源：http://hz.zhiwuduotai.top/gtqpdauwus.html

Ruby: arr.tally
来源：http://hz.sysykeji.top/gttmdqvoom.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenzaomai.com/gtujmhcmrh.html

[D21] 判断是否包含某元素
来源：http://hz.gotoacloud.top/gtythydhap.html

Py:   x in arr
来源：http://hz.aizwys.cn/gtgabvoevu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.sxryk.cn/gtgbqwrggw.html

JS:   arr.includes(x)
来源：http://hz.c1oappe.top/gtxjvuvqwc.html

TS:   arr.includes(x)
来源：http://hz.gotoacloud.top/gtmvlplkpu.html

Java: list.contains(x)
来源：http://hz.smart0.xyz/gtxhhdahhz.html

Go:   slices.Contains(arr, x)
来源：http://hz.shanyushiyangtech.top/gtgnsnrqrz.html

Ruby: arr.include?(x)
来源：http://hz.zhengqikj.top/gtadurhonu.html

C#:   list.Contains(x)
来源：http://hz.nanxuanxn.top/gtakttrwdj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tanke756.top/gtwrcepraj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hywenlv.cn/gtcdhxhwzb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hnqzz.top/gtyigpuivb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.fengsongda.top/gtbehxnjut.html

TS:   [...arr];
来源：http://hz.ehwqpu.com/gtlizksedy.html

Java: new ArrayList<>(list);
来源：http://hz.ehwqpu.com/gtwfdgjtkz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj202588.top/gtmjxvscoe.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sysykeji.top/gtpuiazmjs.html

C#:   new List<int>(list);
来源：http://hz.ydjk.org.cn/gtjfrjksej.html

[D23] reduce 累积计算
来源：http://hz.shanyushiyangkeji.top/gtzydteoei.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sufxvd.cn/gteiixoalf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinghuilouyu.cn/gtkfvlvogn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhixingplan.top/gtyvvgigkv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shangyingyoupin.top/gtkjrxbtfk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gotoacloud.top/gtxlzmqiqn.html

Go:   // 手写循环
来源：http://hz.sweek.top/gtdqmqytdv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ydjk.org.cn/gtkiesthpj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.iojbl.cn/gtgzawshim.html

[D24] 字典 / Map 基本操作
来源：http://hz.yuanzhike.top/gtqkamfmyz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhengqikj.top/gtltaamyjg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ehwqpu.com/gtjdsgtddr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.wangdashe.top/gtfuyvecqd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cucudq.cn/gtyrbvcjbk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinghuilouyu.cn/gtqagdsyov.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yuanzhike.top/gtvxvqjxxd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.chenjidiqi.icu/gtztbczhrb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.iojbl.cn/gtezuzuyav.html

[D25] Set 集合去重与交并差
来源：http://hz.jinyuanbaomall.cn/gtzrqxqmhk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.tian-w.cn/gtilnvalhw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ppjwa.cn/gtxnagnook.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xingfuxueyuan.xyz/gtwonsfjim.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hammf.cn/gtbzwazhtt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sufxvd.cn/gtwryvvrwz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.smart0.xyz/gtoyrgbnqs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yanxiufei.cn/gthvrqytsx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hnxiangtu.top/gtualkuqdh.html

[D26] 数组转字符串
来源：http://hz.shzxlz.cn/gtxzuygnbc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cqqwz.cn/gtmjvaxrdq.html

PHP:  implode(", ", $arr);
来源：http://hz.hysaishi.cn/gtwzyntnja.html

JS:   arr.join(", ")
来源：http://hz.ivvv.top/gtcuhismei.html

TS:   arr.join(", ")
来源：http://hz.tanke756.top/gtyazgzaaf.html

Java: String.join(", ", list)
来源：http://hz.shanyushiyangkeji.top/gtyqyoypvd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.andypj.xyz/gtfzycztyw.html

Ruby: arr.join(", ")
来源：http://hz.quarkkingdee.top/gtzsnuqxoa.html

C#:   string.Join(", ", list)
来源：http://hz.pengpengdd.cyou/gtgltrrqmr.html

================================================================================
来源：http://hz.ivvv.top/gtdrefjlcl.html

E. 字符串处理
来源：http://hz.xziqi.cn/gtdmgvdtxe.html

================================================================================
来源：http://hz.cucudq.cn/gtfnpxybec.html

[E01] 拼接字符串
来源：http://hz.havefunace.top/gtdiinqzyv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hysaishi.cn/gtsxfxgbca.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.pycfn.com/gtdirjnoai.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258888.top/gtuhxtvdak.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.bjfxy.top/gtgtejoalu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhiwuduotai.top/gtkgcdwzuj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hnxiangtu.top/gtmeudiajf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xylfe.cn/gtpnfkbrbo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.fzhhl.top/gthfjtcfze.html

[E02] 重复字符串
来源：http://hz.0kj1m.cn/gtuilpirgt.html

Py:   "ab" * 3
来源：http://hz.nwbrower.top/gtbipwllgl.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cucudq.cn/gtywjsgwrz.html

JS:   "ab".repeat(3)
来源：http://hz.zhengqikj.top/gtpxjryekh.html

TS:   "ab".repeat(3)
来源：http://hz.feifeiyinyue.top/gtcxhoalga.html

Java: "ab".repeat(3)
来源：http://hz.bjfxy.top/gtdjtmkaea.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xziqi.cn/gtazaucugp.html

Ruby: "ab" * 3
来源：http://hz.nanxuanxn.top/gtpzyasdyf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xuanzx.com/gtxyjtnvgy.html

[E03] 截取子串
来源：http://hz.yonumen.top/gtzlrzeauc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cucudq.cn/gtyyapkbyq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ivvv.top/gtxzcmtjuv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.fengsongda.top/gtnwabxrjj.html

TS:   s.slice(1, 4)
来源：http://hz.zhongyouzk.top/gtticmnljx.html

Java: s.substring(1, 4)
来源：http://hz.sweek.top/gtbvjpibnb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sweek.top/gtcecwueim.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.nanxuanxn.top/gtzzrwzboq.html

C#:   s.Substring(1, 3)
来源：http://hz.wangshuangyany.cn/gtsbdjdqdy.html

[E04] 查找子串位置
来源：http://hz.yongpay.top/gtcxmxcivy.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jyoumei.cn/gtclbeqhqw.html

PHP:  strpos($s, "x");
来源：http://hz.sufxvd.cn/gtgdwbkqhk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shzxlz.cn/gtphufkrlw.html

TS:   s.indexOf("x")
来源：http://hz.ehwqpu.com/gtwrowafwx.html

Java: s.indexOf("x")
来源：http://hz.ydjk.org.cn/gtrfttdpif.html

Go:   strings.Index(s, "x")
来源：http://hz.daria6918.cn/gtihcjwpxe.html

Ruby: s.index("x")
来源：http://hz.zhaomingkeji.xyz/gtjjhsckkx.html

C#:   s.IndexOf("x")
来源：http://hz.tianlin.xyz/gtvhmpsyrk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.dianchejie.cn/gttrdkqnjy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.dianchejie.cn/gtvqiyqvnf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ydzc1.top/gtyijgtttf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.snrcjt.cn/gtqmqkkrta.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yj20258.top/gtkvjskpcs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnxiangtu.top/gtibstqxsn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhengqikj.top/gtzofosfln.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jqgufenzy.top/gtcpdrbyzi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yongpay.top/gtuczouamv.html


<!-- 参考信息 -->