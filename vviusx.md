代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.quarkkingdee.top/gtukdxiaye.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.haohaochexian.top/gtxjsgbztu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.wangshuangyany.cn/gtdlpjolon.html

Ruby: # 无泛型
来源：http://hz.zhongyouzk.top/gtqjfvimaf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ivvv.top/gtrzmrnvdc.html

[C15] 解构 / 展开参数
来源：http://hz.cqqwz.cn/gttgifirzx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhixingplan.top/gtdzrzfxel.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ydjk.org.cn/gtjbieflpb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.c1oappe.top/gtrzvdfgve.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.wangdashe.top/gtxqvvkwre.html

Java: // 无解构
来源：http://hz.zhoulong.xyz/gtijlzzllm.html

Go:   // 无解构
来源：http://hz.haohaochexian.top/gtuomudxhs.html

Ruby: a, b = pair
来源：http://hz.ybcxt.top/gtlvkwomml.html

C#:   var (a, b) = pair;
来源：http://hz.xingfuxueyuan.xyz/gtuggkfsql.html

[C16] 函数 / 方法重载
来源：http://hz.zhoulong.xyz/gtkdcmaldr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hywenlv.cn/gteoskrzce.html

PHP:  // 无重载
来源：http://hz.jinyuanbaomall.cn/gtyysizqxc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jianghu66.top/gtbjnmqwnk.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zycfv.cn/gtynhtkbqc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zycfv.cn/gtdazalnts.html

Go:   // 无重载：用不同函数名
来源：http://hz.pengpengdd.cyou/gtthwcetsh.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gaohongyu789.top/gtcbixogmd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hammf.cn/gtuhnuaynl.html

================================================================================
来源：http://hz.ehwqpu.com/gtoovxucgl.html

D. 数组 / 列表 / 集合
来源：http://hz.jlsjyb.cn/gthqjhbnnf.html

================================================================================
来源：http://hz.dashuyun.cn/gtkwrprdzt.html

[D01] 创建数组 / 列表
来源：http://hz.yonumen.top/gtwfviipgf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hnxiangtu.top/gtfdiqkasa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhijiandao.cn/gthocfzykt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yvedp.cn/gtwytnfzxj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.daxiang520.top/gtcavnydjl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.gotoacloud.top/gtutafjaml.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yj20258.top/gtncnyjtlu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.smart0.xyz/gtooufhlqe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shuidangran.top/gtqeodqazr.html

[D02] 追加元素到末尾
来源：http://hz.bjfxy.top/gtxwwmyiho.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenlongwang.top/gtubyuclga.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cheryme.top/gtccmiyjvf.html

JS:   arr.push(4);
来源：http://hz.yj202588.top/gtvqtsvkbf.html

TS:   arr.push(4);
来源：http://hz.meibo888.top/gtjvydvifb.html

Java: list.add(4);
来源：http://hz.c1oappe.top/gtjgnyxlbm.html

Go:   arr = append(arr, 4)
来源：http://hz.ppjwa.cn/gtehvxnbvg.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gogol.net.cn/gtebgaahpx.html

C#:   list.Add(4);
来源：http://hz.chenlongwang.top/gtuwrdywib.html

[D03] 在指定位置插入元素
来源：http://hz.fzhhl.top/gtbduapdsq.html

Py:   arr.insert(0, 0)
来源：http://hz.pycfn.com/gtisfdqorv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.pycfn.com/gtppoppbwy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinqigfzy.top/gtccktxjdd.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.chenjidiqi.icu/gtpvmfnvmi.html

Java: list.add(0, 0);
来源：http://hz.tian-w.cn/gtyjnjrsmh.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.0kj1m.cn/gtzwkswqjk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj20258.top/gtcxjqkhmz.html

C#:   list.Insert(0, 0);
来源：http://hz.c1oappe.top/gtwdyeadwm.html

[D04] 删除元素
来源：http://hz.chenjidiqi.icu/gtegbhqwit.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hnqzz.top/gtssgxuedx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yonumen.top/gtbabtiqls.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sufxvd.cn/gtcoqnfbjm.html

TS:   arr.splice(0, 1);
来源：http://hz.sweek.top/gthoiytstn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yvedp.cn/gtzzfjsvnx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nwbrower.top/gtbljuatuc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jyoumei.cn/gtixvlwqxh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.aibaodan.cn/gtzzwnnwhb.html

[D05] 访问与修改元素
来源：http://hz.mhx1999.top/gtvlnxeqmz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gaohongyu789.top/gttjyrazrg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zdqjudy.top/gtchzooyhg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.tanke756.top/gtmiqoyhbx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.pengpengdd.cyou/gtwpboahms.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ybcxt.top/gtxwpnkzqm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.iojbl.cn/gtppbsafkj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shzxlz.cn/gtgcskyfuo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.chenzaomai.com/gtwehedvxq.html

[D06] 数组长度
来源：http://hz.chenlongwang.top/gtjpgelfyd.html

Py:   len(arr)
来源：http://hz.ybcxt.top/gtgnhtlash.html

PHP:  count($arr);
来源：http://hz.redwolf501.top/gtphczrvtw.html

JS:   arr.length
来源：http://hz.xinyue.icu/gtvjvcnqvb.html

TS:   arr.length
来源：http://hz.smart0.xyz/gtaxgonrcs.html

Java: list.size();
来源：http://hz.xingfuxueyuan.xyz/gtvmkmsfbh.html

Go:   len(arr)
来源：http://hz.zhaomingkeji.xyz/gtxdmupvwb.html

Ruby: arr.length; arr.size
来源：http://hz.jlsjyb.cn/gtitowwwjh.html

C#:   list.Count;
来源：http://hz.cheryme.top/gtjlrvwvbz.html

[D07] 切片 / 取子数组
来源：http://hz.yangfankeji.com/gtsaeisvrw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nanxinkj.top/gtbsiwxrxa.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jlsjyb.cn/gtsacwfhwq.html

JS:   arr.slice(1, 4);
来源：http://hz.zhijiandao.cn/gtvttsnyjz.html

TS:   arr.slice(1, 4);
来源：http://hz.wangshuangyany.cn/gtfpwnrmtc.html

Java: list.subList(1, 4);
来源：http://hz.wangshuangyany.cn/gtytnoakzr.html

Go:   arr[1:4]
来源：http://hz.chenzaomai.com/gtputuvhee.html

Ruby: arr[1, 3]
来源：http://hz.cucudq.cn/gtobxoexlm.html

C#:   list.GetRange(1, 3);
来源：http://hz.gaohongyu789.top/gtqmvpoyia.html

[D08] 合并两个数组
来源：http://hz.hnqzz.top/gtvbiptbhd.html

Py:   a + b;  a.extend(b)
来源：http://hz.redwolf501.top/gtckaolfdv.html

PHP:  array_merge($a, $b);
来源：http://hz.shuidangran.top/gtzjpajiji.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shangyingyoupin.top/gtnnenwxjn.html

TS:   [...a, ...b];
来源：http://hz.zhijiandao.cn/gtclytixxc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yvedp.cn/gttxyxsbnb.html

Go:   append(a, b...)
来源：http://hz.zycfv.cn/gtovwztrzd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhongyouzk.top/gtdoauluqw.html

C#:   a.Concat(b).ToList()
来源：http://hz.yuxming.cn/gtgzfpnpuu.html

[D09] 排序（升序）
来源：http://hz.aibaodan.cn/gtisqtilmi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shuidangran.top/gtzngzawgw.html

PHP:  sort($arr);
来源：http://hz.yj20258.top/gtjlxsgysg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.bjfxy.top/gtdsniystf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sufxvd.cn/gtrrllbfew.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sweek.top/gtpbfjuvjz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cucudq.cn/gtvppfbaww.html

Ruby: arr.sort
来源：http://hz.xuanzx.com/gtrfbqeuic.html

C#:   list.Sort();
来源：http://hz.chenlongwang.top/gtlolpfvwm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhiwuduotai.top/gtynzmudoa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.52xcode.cn/gthjiklxjt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fzhhl.top/gtzrbxtbqx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgfzy.top/gtdkhcunky.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yongpay.top/gtphcmvxqv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.birdmap.top/gtixbmvxbz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ivvv.top/gtjdidoeib.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.52xcode.cn/gtkkvttimm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhoulong.xyz/gtneplzsoa.html

[D11] 反转数组
来源：http://hz.hfpthk.cn/gtftumvfyr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sxryk.cn/gtnvtoggpr.html

PHP:  array_reverse($arr);
来源：http://hz.gzhubu.top/gtiefpradm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xziqi.cn/gtmsnicfjm.html

TS:   [...arr].reverse();
来源：http://hz.zhixingplan.top/gtamglxtud.html

Java: Collections.reverse(list);
来源：http://hz.hfpthk.cn/gtzbabgqas.html

Go:   slices.Reverse(arr)
来源：http://hz.dianchejie.cn/gtfkxtfqhj.html

Ruby: arr.reverse
来源：http://hz.sysykeji.top/gtvgrvhhao.html

C#:   list.Reverse();
来源：http://hz.yuxming.cn/gtkzrnvgva.html

[D12] 查找元素下标
来源：http://hz.jiagoushi.top/gtlnrlqqle.html

Py:   arr.index(x);  x in arr
来源：http://hz.nanxuanxn.top/gtadosrunj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xylfe.cn/gtmwfsbnnj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yangfankeji.com/gtsrpmfyuz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhongyouzk.top/gtchqrrgjq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tianlin.xyz/gtdftvkwaf.html

Go:   slices.Index(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtmiytzbxe.html

Ruby: arr.index(x)
来源：http://hz.yanxiufei.cn/gtuqyrdfdz.html

C#:   list.IndexOf(x);
来源：http://hz.dianchejie.cn/gtykhsjnpa.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tanke756.top/gtqoirdryi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.iojbl.cn/gtqwadbvuy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cucudq.cn/gtpvhavoqg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhijiandao.cn/gthwkocbha.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zycfv.cn/gtsvobskqr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hysaishi.cn/gtvrhlvaer.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hnqzz.top/gtdxpraasu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenjidiqi.icu/gtwhkdulht.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hongshengwenyu.top/gtlbnezsdy.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ppjwa.cn/gtdccnosyq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.guowangkeji.top/gtunainozh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ehwqpu.com/gtqdmtandv.html

JS:   arr.map(x => x * 2)
来源：http://hz.hongshengwenyu.top/gtvjuqypus.html

TS:   arr.map(x => x * 2)
来源：http://hz.ppjwa.cn/gtjwymmzpb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.haohaochexian.top/gtjdibcgig.html

Go:   // 手写循环
来源：http://hz.jqgufenzy.top/gtbuhwfktm.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.svipenyu.cn/gtbnrhntbo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gaohongyu789.top/gtzhacbdup.html

[D15] 去重
来源：http://hz.jqgfzy.top/gthxywctoe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.bjfxy.top/gtuoiojgwv.html

PHP:  array_unique($arr);
来源：http://hz.zdqjudy.top/gttymsymla.html

JS:   [...new Set(arr)]
来源：http://hz.gotoacloud.top/gtdvwlpzxe.html

TS:   [...new Set(arr)]
来源：http://hz.ehwqpu.com/gtbxhlkxqy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shzxlz.cn/gtkttuddvj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.meibo888.top/gtxriilpus.html

Ruby: arr.uniq
来源：http://hz.nanxuanxn.top/gtidgzzzqi.html

C#:   list.Distinct().ToList()
来源：http://hz.zhijiandao.cn/gtltstluoh.html

[D16] 求和与平均值
来源：http://hz.hongshengwenyu.top/gtsjlajwhr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yueranfly.top/gtcmpfxjwz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nwbrower.top/gtflovfnyi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tanke756.top/gtfzmiglrm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhoulong.xyz/gtdddcgiox.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xylfe.cn/gtkxpwvohh.html

Go:   // 手写循环累加
来源：http://hz.feifeiyinyue.top/gthsdxgohw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.wangshuangyany.cn/gtjztyoglr.html

C#:   list.Sum();  list.Average()
来源：http://hz.guowangkeji.top/gtmceiusnr.html

[D17] 最大值与最小值
来源：http://hz.sysykeji.top/gtaeifdisi.html

Py:   max(arr);  min(arr)
来源：http://hz.0kj1m.cn/gtgqwtrmed.html

PHP:  max($arr);  min($arr);
来源：http://hz.316326.xyz/gtjatspimy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yj202588.top/gticjscrnv.html

TS:   Math.max(...arr);
来源：http://hz.iojbl.cn/gtrmqpuwhc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yuanzhike.top/gtfsyvrpfh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangdashe.top/gthkodyozw.html

Ruby: arr.max;  arr.min
来源：http://hz.ydzc1.top/gtepcvlkba.html

C#:   list.Max();  list.Min()
来源：http://hz.svipenyu.cn/gthyucmocd.html

[D18] 扁平化嵌套数组
来源：http://hz.yj202588.top/gtxsjpiimh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ehwqpu.com/gtkspkkawj.html

PHP:  array_merge(...$nested);
来源：http://hz.smart0.xyz/gtxiuqlacl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ppjwa.cn/gtwsoaherc.html

TS:   nested.flat();
来源：http://hz.jianghu66.top/gtyjzgegek.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.mhx1999.top/gtxsktmvua.html

Go:   // 手写双层循环
来源：http://hz.yanxiufei.cn/gtypctaxlu.html

Ruby: nested.flatten
来源：http://hz.hammf.cn/gtdlkiiugc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtyvsstjuy.html

[D19] 按字段分组
来源：http://hz.daxiang520.top/gtpvwzckoq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xuetiantiany.cn/gtrhburqxl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.bjfxy.top/gtkwhvyrys.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.bjfxy.top/gtxtbufsge.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj202588.top/gtkyitrbvb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhoulong.xyz/gtmdcdqtqm.html

Go:   // 手写 map[string][]T
来源：http://hz.yanxiufei.cn/gtplxkntzs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.pycfn.com/gtgfugkzoe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.chenzaomai.com/gtkajdkvkq.html

[D20] 统计每个元素出现次数
来源：http://hz.yj202588.top/gtsnzofqcs.html

Py:   Counter(arr)
来源：http://hz.c1oappe.top/gtjreciizm.html

PHP:  array_count_values($arr);
来源：http://hz.shanyushiyangtech.top/gtgzehjrfu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cucudq.cn/gtinhkfkve.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangtech.top/gtubiuowwa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xinyue.icu/gtyhofnypn.html

Go:   // 手写 map[T]int
来源：http://hz.yangfankeji.com/gtiwenjgvu.html

Ruby: arr.tally
来源：http://hz.fzhhl.top/gtvjlnemxd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.fengsongda.top/gtfqlnsujq.html

[D21] 判断是否包含某元素
来源：http://hz.aizwys.cn/gtgynhkbeu.html

Py:   x in arr
来源：http://hz.jinqigufen.top/gtdrbcaiqh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nanxuanxn.top/gtsqnpxatv.html

JS:   arr.includes(x)
来源：http://hz.yonumen.top/gtfgpinsqi.html

TS:   arr.includes(x)
来源：http://hz.xuetiantiany.cn/gtuswcsved.html

Java: list.contains(x)
来源：http://hz.snrcjt.cn/gtcuglwnoo.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhiwuduotai.top/gtuhuvwwhu.html

Ruby: arr.include?(x)
来源：http://hz.sysykeji.top/gtaziqrrtz.html

C#:   list.Contains(x)
来源：http://hz.zhixingplan.top/gtoutamqsa.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xuanzx.com/gtukgxyhaf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.dashuyun.cn/gtwblhhyhn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.svipenyu.cn/gtkppoqiov.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.tanke756.top/gtlvdkkryl.html

TS:   [...arr];
来源：http://hz.chenjidiqi.icu/gtmortvtbh.html

Java: new ArrayList<>(list);
来源：http://hz.ydzc1.top/gtqpcxxgwb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.pycfn.com/gtdnlbatig.html

Ruby: arr.dup;  arr.clone
来源：http://hz.haohaochexian.top/gtyehnxmby.html

C#:   new List<int>(list);
来源：http://hz.ydzc1.top/gttycndinq.html

[D23] reduce 累积计算
来源：http://hz.shuidangran.top/gtgtycjjbq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jqgfzy.top/gtuqryndkc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jlsjyb.cn/gtxuuhzfns.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.iojbl.cn/gtigiqafqn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ppjwa.cn/gtlnfuswoh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj20258.top/gtrfsqepym.html

Go:   // 手写循环
来源：http://hz.yuanzhike.top/gtqpmdolmp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cucudq.cn/gtjgdgbvso.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shuidangran.top/gtgvewgjsg.html

[D24] 字典 / Map 基本操作
来源：http://hz.fzhhl.top/gtfewyazhm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.birdmap.top/gtdtlsyfkm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.feifeiyinyue.top/gtgxcocavj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj20258.top/gtxlayyzqx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cashguo.top/gtlwqvxatb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yongpay.top/gtlhscstgx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.redwolf501.top/gtvbnomaun.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jianghu66.top/gtzaztdwzd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hnqzz.top/gtooefntxt.html

[D25] Set 集合去重与交并差
来源：http://hz.cheryme.top/gtgbonihzc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.redwolf501.top/gthzcypbvc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.tanke756.top/gtutdkvhpd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yueranfly.top/gtrcghvaoy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hnqzz.top/gtueohfqsz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hnqzz.top/gtvjwswenu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yvedp.cn/gtqmycggjv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinqigufen.top/gtwxfmlgnz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yonumen.top/gtjgauskgs.html

[D26] 数组转字符串
来源：http://hz.zycfv.cn/gtiamexlks.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tanke756.top/gtawdlslwk.html

PHP:  implode(", ", $arr);
来源：http://hz.aibaodan.cn/gtgebldfrf.html

JS:   arr.join(", ")
来源：http://hz.yonumen.top/gtydxegfqf.html

TS:   arr.join(", ")
来源：http://hz.yanxiufei.cn/gtilvdectv.html

Java: String.join(", ", list)
来源：http://hz.iojbl.cn/gtudajgufl.html

Go:   strings.Join(strs, ", ")
来源：http://hz.tianlin.xyz/gtjihttrow.html

Ruby: arr.join(", ")
来源：http://hz.yongpay.top/gtqetsxdpa.html

C#:   string.Join(", ", list)
来源：http://hz.zhengqikj.top/gtzhhouazh.html

================================================================================
来源：http://hz.xziqi.cn/gtmoqhskvn.html

E. 字符串处理
来源：http://hz.jinyuanbaomall.cn/gtjzopvikf.html

================================================================================
来源：http://hz.hfpthk.cn/gtanfqsmhs.html

[E01] 拼接字符串
来源：http://hz.wangdashe.top/gthnmvkqhs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinqigufen.top/gtlvdlhsyp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinqigufen.top/gtyvxnaebs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydjk.org.cn/gtasgsqvlv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnqzz.top/gtheaytqof.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yuxming.cn/gtzlkxowjs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.daria6918.cn/gtjtcpqvau.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gogol.net.cn/gtfgswnato.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gzhubu.top/gtccwaoenh.html

[E02] 重复字符串
来源：http://hz.feifeiyinyue.top/gtcwdaqgrf.html

Py:   "ab" * 3
来源：http://hz.xingfuxueyuan.xyz/gtaymtemuj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fzhhl.top/gtxblvjnyl.html

JS:   "ab".repeat(3)
来源：http://hz.daxiang520.top/gtanzvehev.html

TS:   "ab".repeat(3)
来源：http://hz.xingfuxueyuan.xyz/gtjxsducbk.html

Java: "ab".repeat(3)
来源：http://hz.0kj1m.cn/gthzsymror.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hywenlv.cn/gtxngmmqlv.html

Ruby: "ab" * 3
来源：http://hz.shzxlz.cn/gtaatcexlx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenjidiqi.icu/gtmfbtnyzj.html

[E03] 截取子串
来源：http://hz.ydzc1.top/gtintdjqqt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.pengpengdd.cyou/gtxqmgzkyg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yanxiufei.cn/gtauhtzzze.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.gaohongyu789.top/gtsbrdlkgn.html

TS:   s.slice(1, 4)
来源：http://hz.hywenlv.cn/gtvvyjqhko.html

Java: s.substring(1, 4)
来源：http://hz.gogol.net.cn/gtdajmciju.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.bjfxy.top/gtkgjjgczn.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jyoumei.cn/gtsxsztthj.html

C#:   s.Substring(1, 3)
来源：http://hz.zhengqikj.top/gtzjujrzjd.html

[E04] 查找子串位置
来源：http://hz.ehwqpu.com/gtqyqppxnp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ybcxt.top/gtfgkmmbwg.html

PHP:  strpos($s, "x");
来源：http://hz.ydjk.org.cn/gtummssiui.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.feifeiyinyue.top/gtxxtjzefy.html

TS:   s.indexOf("x")
来源：http://hz.yangfankeji.com/gtpgjzraaw.html

Java: s.indexOf("x")
来源：http://hz.andypj.xyz/gtwsvamthr.html

Go:   strings.Index(s, "x")
来源：http://hz.zdqjudy.top/gtfyeucsyu.html

Ruby: s.index("x")
来源：http://hz.hongshengwenyu.top/gtveaqkxwj.html

C#:   s.IndexOf("x")
来源：http://hz.hfpthk.cn/gtyhuyrztu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.316326.xyz/gtiryeovkw.html


<!-- 参考信息 -->