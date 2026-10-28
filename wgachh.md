代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jiagoushi.top/gtayyvhelf.html

Go:   func add(a, b int) int
来源：http://hz.dianchejie.cn/gtbsxhvuyx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.c1oappe.top/gtiozctsww.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenlongwang.top/gthiwssuur.html

[C14] 泛型函数
来源：http://hz.hammf.cn/gtrwqjyvus.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ybcxt.top/gtynkhfchl.html

PHP:  // 无泛型
来源：http://hz.aizwys.cn/gtwlyyhlcc.html

JS:   // 无泛型
来源：http://hz.jqgufenzy.top/gtsilypbbq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gzhubu.top/gtgyvdtfer.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenlongwang.top/gtxfgxhryu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cqqwz.cn/gtuelpazjf.html

Ruby: # 无泛型
来源：http://hz.fengsongda.top/gtuwqsgeds.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cqqwz.cn/gtcxvgjjao.html

[C15] 解构 / 展开参数
来源：http://hz.jqgfzy.top/gtbaeclkvh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.pycfn.com/gtcfhgwdid.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cheryme.top/gtpzacvzcg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhijiandao.cn/gtkemfovwc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hnxiangtu.top/gtblsonryo.html

Java: // 无解构
来源：http://hz.hammf.cn/gtmnralfxc.html

Go:   // 无解构
来源：http://hz.jqgufenzy.top/gtvhcmwtzb.html

Ruby: a, b = pair
来源：http://hz.yongpay.top/gtiwhofiob.html

C#:   var (a, b) = pair;
来源：http://hz.pycfn.com/gtbegqzhym.html

[C16] 函数 / 方法重载
来源：http://hz.jinghuilouyu.cn/gtrbbjzibd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.guannengcc.top/gtiwitgcyq.html

PHP:  // 无重载
来源：http://hz.jyoumei.cn/gtvxdluuaj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.vqdsnc.cn/gtegtkughe.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.nanxuanxn.top/gtknfqykal.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xuetiantiany.cn/gtdnhbdrvo.html

Go:   // 无重载：用不同函数名
来源：http://hz.meibo888.top/gtfgfboamx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yangfankeji.com/gtwrevguvn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hfpthk.cn/gtsghfmrci.html

================================================================================
来源：http://hz.fzhhl.top/gtdczdmpnt.html

D. 数组 / 列表 / 集合
来源：http://hz.jinyuanbaomall.cn/gtmwwlaqym.html

================================================================================
来源：http://hz.zhongyouzk.top/gtuydwyiqb.html

[D01] 创建数组 / 列表
来源：http://hz.9152youxi.cn/gtsgylnqyv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhixingplan.top/gtyggxquea.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xuanzx.com/gtvrfephzj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jyoumei.cn/gtaemseylk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shzxlz.cn/gtlkabeaoe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.aibaodan.cn/gtjqhlutxf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cdnleiting.top/gttrwlcnsx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.guannengcc.top/gtbcezxusb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.0kj1m.cn/gtvhedeemu.html

[D02] 追加元素到末尾
来源：http://hz.sxryk.cn/gtbcnthvhx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.fengsongda.top/gtulnfprbq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gaohongyu789.top/gtncxmnkhy.html

JS:   arr.push(4);
来源：http://hz.pycfn.com/gtbnjlzbit.html

TS:   arr.push(4);
来源：http://hz.gogol.net.cn/gtznreoxdm.html

Java: list.add(4);
来源：http://hz.ivvv.top/gtfcytvzyi.html

Go:   arr = append(arr, 4)
来源：http://hz.nanxinkj.top/gtqydjtosq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.316326.xyz/gtgntflbjl.html

C#:   list.Add(4);
来源：http://hz.xingfuxueyuan.xyz/gtykderoue.html

[D03] 在指定位置插入元素
来源：http://hz.shuidangran.top/gtetgsonxj.html

Py:   arr.insert(0, 0)
来源：http://hz.ehwqpu.com/gtlyfvhxnd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yongpay.top/gtpkhiqzpq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.316326.xyz/gtidymgdig.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhengqikj.top/gtxnkfsdom.html

Java: list.add(0, 0);
来源：http://hz.tanke756.top/gtoosgiwtw.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.fzhhl.top/gtacsarnin.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydjk.org.cn/gttvitaoht.html

C#:   list.Insert(0, 0);
来源：http://hz.jyoumei.cn/gtzpxywvsq.html

[D04] 删除元素
来源：http://hz.hywenlv.cn/gtgvnowdko.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ehwqpu.com/gtoupjbfur.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.daria6918.cn/gtjizbuiwi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.iojbl.cn/gtfkrxvusj.html

TS:   arr.splice(0, 1);
来源：http://hz.daria6918.cn/gtnbzqiiad.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sxryk.cn/gtvivthojg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sxryk.cn/gtcngkhevq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sweek.top/gteprtaaih.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.pycfn.com/gtlesztzlu.html

[D05] 访问与修改元素
来源：http://hz.havefunace.top/gtlauryjrc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.52xcode.cn/gtkfbhxrvr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.9152youxi.cn/gtgsjbxmix.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yangfankeji.com/gtshhpoqxf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.pycfn.com/gtmpftqjaz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yj20258.top/gtjcaygmhb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ydzc1.top/gtzrfwfjeh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtdgyfshnp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.iojbl.cn/gtgsbgjxsn.html

[D06] 数组长度
来源：http://hz.0kj1m.cn/gtzmzbokuq.html

Py:   len(arr)
来源：http://hz.ydzc1.top/gtdyirvzjy.html

PHP:  count($arr);
来源：http://hz.zhijiandao.cn/gtmnyiawal.html

JS:   arr.length
来源：http://hz.jiagoushi.top/gtmvlhtjjn.html

TS:   arr.length
来源：http://hz.andypj.xyz/gtafeemtrn.html

Java: list.size();
来源：http://hz.gogol.net.cn/gtaygyxmnh.html

Go:   len(arr)
来源：http://hz.wangshuangyany.cn/gtltaizfua.html

Ruby: arr.length; arr.size
来源：http://hz.cdnleiting.top/gtlenbgyon.html

C#:   list.Count;
来源：http://hz.pengpengdd.cyou/gtemvhvrlf.html

[D07] 切片 / 取子数组
来源：http://hz.havefunace.top/gtpzrnpzxf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.bjfxy.top/gtfurbqhvc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shuidangran.top/gtwvyakglz.html

JS:   arr.slice(1, 4);
来源：http://hz.zhijiandao.cn/gtihdlreoy.html

TS:   arr.slice(1, 4);
来源：http://hz.ehwqpu.com/gtgcwvtsrk.html

Java: list.subList(1, 4);
来源：http://hz.gaohongyu789.top/gtgxdqgtel.html

Go:   arr[1:4]
来源：http://hz.quarkkingdee.top/gtrlgxrqru.html

Ruby: arr[1, 3]
来源：http://hz.yongpay.top/gtzhxsvvai.html

C#:   list.GetRange(1, 3);
来源：http://hz.c1oappe.top/gtbeybvhdu.html

[D08] 合并两个数组
来源：http://hz.feifeiyinyue.top/gtcxkepdfl.html

Py:   a + b;  a.extend(b)
来源：http://hz.cheryme.top/gtaeaxdgjs.html

PHP:  array_merge($a, $b);
来源：http://hz.hammf.cn/gtomqtxbrd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ybcxt.top/gtnouvklwr.html

TS:   [...a, ...b];
来源：http://hz.kuanghao11.cn/gtyqgswwqb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.nanxinkj.top/gtftqmsqmw.html

Go:   append(a, b...)
来源：http://hz.jiagoushi.top/gtjacbbghw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jqgufenzy.top/gttkfiiuuy.html

C#:   a.Concat(b).ToList()
来源：http://hz.hfpthk.cn/gtmkbuzgdp.html

[D09] 排序（升序）
来源：http://hz.cashguo.top/gtqmabrhdl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhijiandao.cn/gtyzhikteq.html

PHP:  sort($arr);
来源：http://hz.jinyuanbaomall.cn/gthowvhnyv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sysykeji.top/gtyctyfaxl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sysykeji.top/gthaeauxyp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ppjwa.cn/gtitqsoglh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.wangdashe.top/gtqllnhczf.html

Ruby: arr.sort
来源：http://hz.daria6918.cn/gtfmexklyg.html

C#:   list.Sort();
来源：http://hz.sysykeji.top/gtvkxczpon.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ivvv.top/gtfuobmjaw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sweek.top/gtrgenpozz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.0kj1m.cn/gttpoqgwyz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigfzy.top/gtlsnvwboi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxuanxn.top/gtusymazcn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xuanzx.com/gtisftcckr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yj202588.top/gtfbongzkd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tian-w.cn/gtformyrbh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xuanzx.com/gtyuccyctv.html

[D11] 反转数组
来源：http://hz.zhaomingkeji.xyz/gtfhrhvchs.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.pycfn.com/gtoxayzvwj.html

PHP:  array_reverse($arr);
来源：http://hz.zhiwuduotai.top/gtmuvpjqva.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinqigufen.top/gtilbebcmy.html

TS:   [...arr].reverse();
来源：http://hz.c1oappe.top/gtowxqkozr.html

Java: Collections.reverse(list);
来源：http://hz.andypj.xyz/gtttbizbgy.html

Go:   slices.Reverse(arr)
来源：http://hz.ywan-chungtsiang.top/gtaawfaglk.html

Ruby: arr.reverse
来源：http://hz.jinghuilouyu.cn/gtuocljjjr.html

C#:   list.Reverse();
来源：http://hz.shzxlz.cn/gtdyyapdyq.html

[D12] 查找元素下标
来源：http://hz.xuetiantiany.cn/gtcrwmsscy.html

Py:   arr.index(x);  x in arr
来源：http://hz.fengsongda.top/gtkhecbqvy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yj202588.top/gtrblvrsgf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sufxvd.cn/gtwzjrbqfo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ybcxt.top/gtzwuiwbkz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xinyue.icu/gtrkmzemnw.html

Go:   slices.Index(arr, x)
来源：http://hz.zhengqikj.top/gtmdbkcnxp.html

Ruby: arr.index(x)
来源：http://hz.yangfankeji.com/gtemtsumgj.html

C#:   list.IndexOf(x);
来源：http://hz.sxryk.cn/gtgvmvcezd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.chenjidiqi.icu/gtjbxdsqvw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.redwolf501.top/gtgztchbwr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gogol.net.cn/gtjzdcfjgx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ehwqpu.com/gtqncvvsnr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtcqwzorbb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinqigufen.top/gtotivvsfp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gogol.net.cn/gtqzmhzfim.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sysykeji.top/gtxvkdftql.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ppjwa.cn/gtuppzipue.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tian-w.cn/gtsvppzcjp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jqgufenzy.top/gtpjtlixod.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.redwolf501.top/gtspafopig.html

JS:   arr.map(x => x * 2)
来源：http://hz.xylfe.cn/gtfwoluoqs.html

TS:   arr.map(x => x * 2)
来源：http://hz.cheryme.top/gtguvpfyuj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hammf.cn/gtbpxrojdv.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gtjclozmps.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.0kj1m.cn/gtscsevqjo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ivvv.top/gtlxdjedfb.html

[D15] 去重
来源：http://hz.zycfv.cn/gtfwqhwxva.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinghuilouyu.cn/gtrmukcysp.html

PHP:  array_unique($arr);
来源：http://hz.jqgfzy.top/gtxwrekplc.html

JS:   [...new Set(arr)]
来源：http://hz.cashguo.top/gtbvbmzyvb.html

TS:   [...new Set(arr)]
来源：http://hz.cdnleiting.top/gtfcodmmdm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.redwolf501.top/gtomnspmyi.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nwbrower.top/gtyuqfmvts.html

Ruby: arr.uniq
来源：http://hz.daria6918.cn/gtqxewbwkb.html

C#:   list.Distinct().ToList()
来源：http://hz.ydjk.org.cn/gtqukemnae.html

[D16] 求和与平均值
来源：http://hz.jiagoushi.top/gteumcmhcl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yueranfly.top/gtqixvqpnn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jqgufenzy.top/gtxwiwngeb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xziqi.cn/gtzgaksxpj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xziqi.cn/gtapmjotws.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.kuanghao11.cn/gtxbatvnoo.html

Go:   // 手写循环累加
来源：http://hz.zhixingplan.top/gtcgkdppds.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hnqzz.top/gtcdoezwst.html

C#:   list.Sum();  list.Average()
来源：http://hz.gzhubu.top/gtvucntqvz.html

[D17] 最大值与最小值
来源：http://hz.xinyue.icu/gtuzlybqqx.html

Py:   max(arr);  min(arr)
来源：http://hz.dianchejie.cn/gtaxkwnien.html

PHP:  max($arr);  min($arr);
来源：http://hz.hysaishi.cn/gtvcsjvuru.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dianchejie.cn/gtrjdvtfef.html

TS:   Math.max(...arr);
来源：http://hz.wangdashe.top/gthdqcmegq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shuidangran.top/gtwucskbkr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jianghu66.top/gtpvldosay.html

Ruby: arr.max;  arr.min
来源：http://hz.tianlin.xyz/gtbgljblkw.html

C#:   list.Max();  list.Min()
来源：http://hz.pengpengdd.cyou/gtqtabavjx.html

[D18] 扁平化嵌套数组
来源：http://hz.ywan-chungtsiang.top/gtdhbuffgt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenlongwang.top/gtwryevnzm.html

PHP:  array_merge(...$nested);
来源：http://hz.bjfxy.top/gtdrxijqok.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhiwuduotai.top/gtojqmedrg.html

TS:   nested.flat();
来源：http://hz.fengsongda.top/gtpbugsvim.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.52xcode.cn/gtxkflsdtg.html

Go:   // 手写双层循环
来源：http://hz.shangyingyoupin.top/gtlngpxpff.html

Ruby: nested.flatten
来源：http://hz.0kj1m.cn/gtzjskatfh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gogol.net.cn/gtskqfrfxm.html

[D19] 按字段分组
来源：http://hz.yonumen.top/gtbcanlaie.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.feifeiyinyue.top/gtnuexnjyj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xuetiantiany.cn/gtyunvhiby.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.aibaodan.cn/gtuheskvhw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jlsjyb.cn/gtjiufxaxh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.aibaodan.cn/gtoumbibrt.html

Go:   // 手写 map[string][]T
来源：http://hz.jianghu66.top/gtxkeukhtm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.chenjidiqi.icu/gthdbuzlnm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhijiandao.cn/gtmwpcyeec.html

[D20] 统计每个元素出现次数
来源：http://hz.gotoacloud.top/gtpledaxiu.html

Py:   Counter(arr)
来源：http://hz.yj20258888.top/gtmsxxtdwu.html

PHP:  array_count_values($arr);
来源：http://hz.yonumen.top/gtomvityov.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zycfv.cn/gtkmolyrgh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dianchejie.cn/gtlyycsjrh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yongpay.top/gthkvvpfis.html

Go:   // 手写 map[T]int
来源：http://hz.hywenlv.cn/gtntuhjqyg.html

Ruby: arr.tally
来源：http://hz.nanxuanxn.top/gtiifvrptk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gaohongyu789.top/gtyqflpcpd.html

[D21] 判断是否包含某元素
来源：http://hz.yvedp.cn/gtevbqtshb.html

Py:   x in arr
来源：http://hz.xinyue.icu/gtrkaabhtr.html

PHP:  in_array($x, $arr, true);
来源：http://hz.svipenyu.cn/gtvaunoodz.html

JS:   arr.includes(x)
来源：http://hz.zhaomingkeji.xyz/gtzwsozzkt.html

TS:   arr.includes(x)
来源：http://hz.yj202588.top/gthzacftip.html

Java: list.contains(x)
来源：http://hz.ywan-chungtsiang.top/gtcyvhlgxx.html

Go:   slices.Contains(arr, x)
来源：http://hz.wangdashe.top/gtptfifmyi.html

Ruby: arr.include?(x)
来源：http://hz.yangfankeji.com/gtilkuciwu.html

C#:   list.Contains(x)
来源：http://hz.jianghu66.top/gtepdgcfss.html

[D22] 复制数组（避免共享引用）
来源：http://hz.52xcode.cn/gtcgisgtgi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gzhubu.top/gtxqabjipe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.52xcode.cn/gtpdkqvfuo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gzhubu.top/gtxnwrdeuy.html

TS:   [...arr];
来源：http://hz.bjfxy.top/gtmhcnlevt.html

Java: new ArrayList<>(list);
来源：http://hz.svipenyu.cn/gtdmroaswd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhaomingkeji.xyz/gtoqpkiqdy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.bjfxy.top/gtvajudzmz.html

C#:   new List<int>(list);
来源：http://hz.gzhubu.top/gtirwzthgd.html

[D23] reduce 累积计算
来源：http://hz.andypj.xyz/gtvzmszxxq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hnqzz.top/gtyuvjeitw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zycfv.cn/gtnowdcyjw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aibaodan.cn/gtaslxgxzd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuxming.cn/gtxznarrpj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhongyouzk.top/gtoerhwzjs.html

Go:   // 手写循环
来源：http://hz.xuetiantiany.cn/gtvskefzgt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xingfuxueyuan.xyz/gtrkcagjoi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.quarkkingdee.top/gtozubxpgx.html

[D24] 字典 / Map 基本操作
来源：http://hz.nanxuanxn.top/gtszqeuyet.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shzxlz.cn/gtfldzbalz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.chenlongwang.top/gtaxzwjper.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yuanzhike.top/gtmaeabpim.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shanyushiyangkeji.top/gtypteltqg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhengqikj.top/gtwnzpxmfd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.bjfxy.top/gtfucofffy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.meibo888.top/gtxjzmuzmu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hnqzz.top/gtodoxumxt.html

[D25] Set 集合去重与交并差
来源：http://hz.aibaodan.cn/gtqozznrpt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jyoumei.cn/gtatljearf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenzaomai.com/gtbanylizs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.svipenyu.cn/gtrsimjsog.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shanyushiyangtech.top/gtdkuoikbq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yvedp.cn/gtvklnvdye.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cashguo.top/gtdzrsfuuv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hnxiangtu.top/gtttqoetby.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cqqwz.cn/gtehcrnrlo.html

[D26] 数组转字符串
来源：http://hz.xylfe.cn/gtkgapomfi.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ehwqpu.com/gtceitvknn.html

PHP:  implode(", ", $arr);
来源：http://hz.zhijiandao.cn/gtibiurqjm.html

JS:   arr.join(", ")
来源：http://hz.jqgufenzy.top/gtqwvvrbeq.html

TS:   arr.join(", ")
来源：http://hz.tianlin.xyz/gtjkstzvuf.html

Java: String.join(", ", list)
来源：http://hz.jinghuilouyu.cn/gtccnvajxz.html

Go:   strings.Join(strs, ", ")
来源：http://hz.vqdsnc.cn/gtgvijnsiz.html

Ruby: arr.join(", ")
来源：http://hz.xinyue.icu/gtzznnlolw.html

C#:   string.Join(", ", list)
来源：http://hz.wangdashe.top/gttppaoogm.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtqjxqilbq.html

E. 字符串处理
来源：http://hz.andypj.xyz/gtyhttqftl.html

================================================================================
来源：http://hz.sufxvd.cn/gtxsykyxwp.html

[E01] 拼接字符串
来源：http://hz.c1oappe.top/gtstedmcpb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhaomingkeji.xyz/gtliglmhte.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xuetiantiany.cn/gtbovcbpah.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.pengpengdd.cyou/gtjpdtxmxw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.vqdsnc.cn/gtlwsanwzm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhiwuduotai.top/gtgreongiz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.kuanghao11.cn/gtcjheehxs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ehwqpu.com/gtfncjwjhv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtuwjkipdw.html

[E02] 重复字符串
来源：http://hz.zhiwuduotai.top/gtjfpsains.html

Py:   "ab" * 3
来源：http://hz.tian-w.cn/gtgtfiwvfi.html

PHP:  str_repeat("ab", 3);
来源：http://hz.9152youxi.cn/gtmmmrebkq.html

JS:   "ab".repeat(3)
来源：http://hz.ydjk.org.cn/gtaraluuux.html

TS:   "ab".repeat(3)
来源：http://hz.chenzaomai.com/gtynzdrpdh.html

Java: "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtrxefieuw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.daxiang520.top/gtxzbmktkc.html

Ruby: "ab" * 3
来源：http://hz.ybcxt.top/gtiuxjueqx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.vqdsnc.cn/gtnvwvsqfk.html

[E03] 截取子串
来源：http://hz.zycfv.cn/gtvnyjnygd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hfpthk.cn/gtizgrzwwx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.sysykeji.top/gtyiqfpqzk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jqgfzy.top/gtattnagtq.html

TS:   s.slice(1, 4)
来源：http://hz.yuxming.cn/gtlqmnykpg.html

Java: s.substring(1, 4)
来源：http://hz.bjfxy.top/gtfvycauqr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ehwqpu.com/gtdxffplro.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zycfv.cn/gtnrqqgxpz.html

C#:   s.Substring(1, 3)
来源：http://hz.hnxiangtu.top/gtejeliizf.html

[E04] 查找子串位置
来源：http://hz.hongshengwenyu.top/gttmvgvvvg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ydzc1.top/gtuckusuyw.html


<!-- 参考信息 -->