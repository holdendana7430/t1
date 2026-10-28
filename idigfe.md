代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hongshengwenyu.top/gtzvsssbsp.html

[C15] 解构 / 展开参数
来源：http://hz.cashguo.top/gttkvyyszo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ivvv.top/gtkaokjdcq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cheryme.top/gtywtvsast.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinyuanbaomall.cn/gtfhywfsdt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jianghu66.top/gtcoqcijsh.html

Java: // 无解构
来源：http://hz.meibo888.top/gthqveklbj.html

Go:   // 无解构
来源：http://hz.jinyuanbaomall.cn/gtbbtuqtqj.html

Ruby: a, b = pair
来源：http://hz.hnxiangtu.top/gtakhwoeip.html

C#:   var (a, b) = pair;
来源：http://hz.bjfxy.top/gtgauelhzg.html

[C16] 函数 / 方法重载
来源：http://hz.feifeiyinyue.top/gtnpnatdmu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yuxming.cn/gtftqcvmhr.html

PHP:  // 无重载
来源：http://hz.tian-w.cn/gtrhovamzs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.redwolf501.top/gtyzsfvtkc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhongyouzk.top/gtuyizagnd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinyuanbaomall.cn/gtiqotbugk.html

Go:   // 无重载：用不同函数名
来源：http://hz.ppjwa.cn/gtfwlpvlsk.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hnqzz.top/gterygkvar.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yj20258888.top/gthehfbqui.html

================================================================================
来源：http://hz.nanxinkj.top/gtpnppxsil.html

D. 数组 / 列表 / 集合
来源：http://hz.gogol.net.cn/gtjwlrdxhh.html

================================================================================
来源：http://hz.jqgufenzy.top/gticyxedyx.html

[D01] 创建数组 / 列表
来源：http://hz.wangshuangyany.cn/gtprofvubh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ppjwa.cn/gtbsfgzxib.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.316326.xyz/gtqmoafiws.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhaomingkeji.xyz/gtiecxdclr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cashguo.top/gticsagzyl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cashguo.top/gttsuqdlbm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.chenzaomai.com/gtzfvjhhxw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shanyushiyangtech.top/gtkjulazid.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ehwqpu.com/gtgnovtchx.html

[D02] 追加元素到末尾
来源：http://hz.jianghu66.top/gtyyxtdhot.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.pengpengdd.cyou/gtdhfuyixb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ppjwa.cn/gtsflgpcrg.html

JS:   arr.push(4);
来源：http://hz.cdnleiting.top/gtdlquzmay.html

TS:   arr.push(4);
来源：http://hz.cashguo.top/gtqcfbzvpq.html

Java: list.add(4);
来源：http://hz.chenzaomai.com/gtbrrhbvsv.html

Go:   arr = append(arr, 4)
来源：http://hz.shanyushiyangtech.top/gtwizogedg.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shzxlz.cn/gtsvdakljn.html

C#:   list.Add(4);
来源：http://hz.gotoacloud.top/gtkcewyppk.html

[D03] 在指定位置插入元素
来源：http://hz.jinqigfzy.top/gtfnyydnxn.html

Py:   arr.insert(0, 0)
来源：http://hz.nwbrower.top/gtqdjpntsd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yueranfly.top/gtgdvfuzsq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gogol.net.cn/gthgklvstb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.bjfxy.top/gtbwtpouhe.html

Java: list.add(0, 0);
来源：http://hz.birdmap.top/gtamcoshzr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhaomingkeji.xyz/gtslbspysn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.redwolf501.top/gtvesumsno.html

C#:   list.Insert(0, 0);
来源：http://hz.ppjwa.cn/gtcijyvmru.html

[D04] 删除元素
来源：http://hz.mhx1999.top/gtcczvximn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shzxlz.cn/gtuhfvczqy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jyoumei.cn/gtikbazehv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pengpengdd.cyou/gtylbmxppi.html

TS:   arr.splice(0, 1);
来源：http://hz.pengpengdd.cyou/gtvjqijsmu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tianlin.xyz/gtihoaktbl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jqgufenzy.top/gtkucyeuvk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hongshengwenyu.top/gtkydnkwvt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.snrcjt.cn/gtubkbggiu.html

[D05] 访问与修改元素
来源：http://hz.ybcxt.top/gtjsubrwou.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ybcxt.top/gtsudjmvso.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.tanke756.top/gtqndvulsh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yanxiufei.cn/gtdtiuqchd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ybcxt.top/gtgziulddh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.birdmap.top/gtbgkuxlaw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yueranfly.top/gtepqbtjzh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtlujalubc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hfpthk.cn/gtmklqnykt.html

[D06] 数组长度
来源：http://hz.jqgfzy.top/gtchwwdmwm.html

Py:   len(arr)
来源：http://hz.cheryme.top/gtohnvbzfe.html

PHP:  count($arr);
来源：http://hz.jqgfzy.top/gtquiqydxq.html

JS:   arr.length
来源：http://hz.mhx1999.top/gtgfjrondx.html

TS:   arr.length
来源：http://hz.gzhubu.top/gtlngijfde.html

Java: list.size();
来源：http://hz.pengpengdd.cyou/gtxdomaszs.html

Go:   len(arr)
来源：http://hz.0kj1m.cn/gtbksyhimz.html

Ruby: arr.length; arr.size
来源：http://hz.cucudq.cn/gtsrolwsqq.html

C#:   list.Count;
来源：http://hz.xuanzx.com/gtohfqyqgn.html

[D07] 切片 / 取子数组
来源：http://hz.yuanzhike.top/gtrlmasqgo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yonumen.top/gtdpciejis.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yonumen.top/gtiiskvdpu.html

JS:   arr.slice(1, 4);
来源：http://hz.haohaochexian.top/gtmztqrnbf.html

TS:   arr.slice(1, 4);
来源：http://hz.yueranfly.top/gtlmxvwljo.html

Java: list.subList(1, 4);
来源：http://hz.zdqjudy.top/gtkgkhchzt.html

Go:   arr[1:4]
来源：http://hz.dashuyun.cn/gttbdhicib.html

Ruby: arr[1, 3]
来源：http://hz.zhengqikj.top/gtoemuqpkx.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhiwuduotai.top/gttksjzqrb.html

[D08] 合并两个数组
来源：http://hz.9152youxi.cn/gtckintcem.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhongyouzk.top/gthqerfaqe.html

PHP:  array_merge($a, $b);
来源：http://hz.gzhubu.top/gtgnjxglve.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cqqwz.cn/gtszdhwjrn.html

TS:   [...a, ...b];
来源：http://hz.tanke756.top/gtulkqepaz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.iojbl.cn/gtxstfairf.html

Go:   append(a, b...)
来源：http://hz.yonumen.top/gtnztvlpmk.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cucudq.cn/gtcgddlcrn.html

C#:   a.Concat(b).ToList()
来源：http://hz.mhx1999.top/gtabvtvbsv.html

[D09] 排序（升序）
来源：http://hz.jiagoushi.top/gthihoooie.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtotixulke.html

PHP:  sort($arr);
来源：http://hz.jinqigfzy.top/gtysggvnny.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ywan-chungtsiang.top/gtrjkpfrvd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinqigufen.top/gtrhwifluc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xinyue.icu/gtqhjozgrk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhixingplan.top/gtlhowigfh.html

Ruby: arr.sort
来源：http://hz.ybcxt.top/gtfeleequt.html

C#:   list.Sort();
来源：http://hz.hongshengwenyu.top/gtsikuhley.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gzhubu.top/gtcxhrzzus.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ppjwa.cn/gtzsdndyla.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tanke756.top/gtiqevebqq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shzxlz.cn/gtcvhbbqfh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.c1oappe.top/gtymdykqfm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ydzc1.top/gtjnkrblng.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.snrcjt.cn/gtexojjjlj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shanyushiyangtech.top/gtyepvqajh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.dashuyun.cn/gtewcqfuxh.html

[D11] 反转数组
来源：http://hz.svipenyu.cn/gtchsjjnaq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.dashuyun.cn/gtzfuqzvwe.html

PHP:  array_reverse($arr);
来源：http://hz.xuetiantiany.cn/gtjjtchjgo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hongshengwenyu.top/gtfnoqkddj.html

TS:   [...arr].reverse();
来源：http://hz.daria6918.cn/gtersmgjyl.html

Java: Collections.reverse(list);
来源：http://hz.zhiwuduotai.top/gtegmxaovo.html

Go:   slices.Reverse(arr)
来源：http://hz.xuetiantiany.cn/gtjtvvjsvd.html

Ruby: arr.reverse
来源：http://hz.xinyue.icu/gteionnhyc.html

C#:   list.Reverse();
来源：http://hz.daria6918.cn/gtltlokngw.html

[D12] 查找元素下标
来源：http://hz.zhongyouzk.top/gtiuyepnna.html

Py:   arr.index(x);  x in arr
来源：http://hz.shangyingyoupin.top/gtqqzojhyx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yueranfly.top/gtxqogsdyu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sysykeji.top/gttuqhrfrf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fengsongda.top/gtpfyewjfk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gaohongyu789.top/gthxnmcapu.html

Go:   slices.Index(arr, x)
来源：http://hz.pengpengdd.cyou/gtzwbdomou.html

Ruby: arr.index(x)
来源：http://hz.pengpengdd.cyou/gtelyzqnja.html

C#:   list.IndexOf(x);
来源：http://hz.zhijiandao.cn/gtgdsvbiye.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hnxiangtu.top/gtrzigsqhi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yj20258.top/gtmwmfdgau.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhiwuduotai.top/gtevhuoonm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jyoumei.cn/gtbybpmuon.html

TS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gtnuesrqgy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cdnleiting.top/gtmpigrbsb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhixingplan.top/gtkicsixcb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.aizwys.cn/gtrhihbypm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jqgufenzy.top/gtfnkkmlfm.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cucudq.cn/gtvouioybi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yongpay.top/gturfgkwaa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.chenjidiqi.icu/gtsuvqyqhk.html

JS:   arr.map(x => x * 2)
来源：http://hz.ydzc1.top/gttwwfolgr.html

TS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangkeji.top/gtreisiqie.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yj20258.top/gtzcapskeq.html

Go:   // 手写循环
来源：http://hz.jiagoushi.top/gtaxdtsotl.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.haohaochexian.top/gttdeoprld.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.vqdsnc.cn/gtjifzwvmq.html

[D15] 去重
来源：http://hz.ppjwa.cn/gtoesmhzak.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ehwqpu.com/gturihzhbi.html

PHP:  array_unique($arr);
来源：http://hz.svipenyu.cn/gtadsrsulm.html

JS:   [...new Set(arr)]
来源：http://hz.sxryk.cn/gtvbsvjycx.html

TS:   [...new Set(arr)]
来源：http://hz.yj202588.top/gtnzkirdyb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.fengsongda.top/gtenufadih.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinqigufen.top/gtwztjjmgi.html

Ruby: arr.uniq
来源：http://hz.shangyingyoupin.top/gtdigxlkff.html

C#:   list.Distinct().ToList()
来源：http://hz.jinghuilouyu.cn/gtkfygwiri.html

[D16] 求和与平均值
来源：http://hz.jyoumei.cn/gtzjoldzcf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zycfv.cn/gtjklrgqeb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.birdmap.top/gtrjvidfby.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.0kj1m.cn/gtazphkqvf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gzhubu.top/gtzbvljato.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nwbrower.top/gtfnldvnpz.html

Go:   // 手写循环累加
来源：http://hz.xinyue.icu/gtzuzogkiu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.0kj1m.cn/gthreoahja.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinqigfzy.top/gtoohvsnwl.html

[D17] 最大值与最小值
来源：http://hz.shangyingyoupin.top/gtbuapzaig.html

Py:   max(arr);  min(arr)
来源：http://hz.meibo888.top/gtdduqgoox.html

PHP:  max($arr);  min($arr);
来源：http://hz.meibo888.top/gtbqpkvjkh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cheryme.top/gtulsurnkh.html

TS:   Math.max(...arr);
来源：http://hz.gotoacloud.top/gtiwwptiuv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.9152youxi.cn/gtteiqibzg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cqqwz.cn/gtpyrgpbnz.html

Ruby: arr.max;  arr.min
来源：http://hz.xingfuxueyuan.xyz/gtgynpqwnh.html

C#:   list.Max();  list.Min()
来源：http://hz.ydjk.org.cn/gtojvhutut.html

[D18] 扁平化嵌套数组
来源：http://hz.zhixingplan.top/gtikpwdtjd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yj20258888.top/gterearnlg.html

PHP:  array_merge(...$nested);
来源：http://hz.hnxiangtu.top/gtbwqnxdbh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yangfankeji.com/gtvahauoot.html

TS:   nested.flat();
来源：http://hz.52xcode.cn/gtobnvacvq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj20258888.top/gtgchnpluq.html

Go:   // 手写双层循环
来源：http://hz.havefunace.top/gtzsjmzbzr.html

Ruby: nested.flatten
来源：http://hz.yuanzhike.top/gtcvrqekdq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.tanke756.top/gtzqhrmtgh.html

[D19] 按字段分组
来源：http://hz.fengsongda.top/gtrstgjlea.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.feifeiyinyue.top/gtblpthxyc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.wangshuangyany.cn/gtpyibzqjv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenjidiqi.icu/gtkroqsryy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hongshengwenyu.top/gtvdftqnrh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.aibaodan.cn/gtmhpoaifq.html

Go:   // 手写 map[string][]T
来源：http://hz.gogol.net.cn/gtofpryooo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ppjwa.cn/gtkzxsltlx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jlsjyb.cn/gtzsxxkgcq.html

[D20] 统计每个元素出现次数
来源：http://hz.yj20258.top/gtfqhgrelp.html

Py:   Counter(arr)
来源：http://hz.birdmap.top/gtvetkshoy.html

PHP:  array_count_values($arr);
来源：http://hz.haohaochexian.top/gtsenazgkx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.svipenyu.cn/gtucstwmwy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nwbrower.top/gtwdptwqqg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xziqi.cn/gtcmregnwk.html

Go:   // 手写 map[T]int
来源：http://hz.chenjidiqi.icu/gthuxryjpv.html

Ruby: arr.tally
来源：http://hz.gzhubu.top/gtnjcsdnyy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cdnleiting.top/gtvyartxkv.html

[D21] 判断是否包含某元素
来源：http://hz.zycfv.cn/gtzrwuruus.html

Py:   x in arr
来源：http://hz.zhiwuduotai.top/gtzvoomvgw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jqgufenzy.top/gtydwyqesd.html

JS:   arr.includes(x)
来源：http://hz.nwbrower.top/gttiguhlhg.html

TS:   arr.includes(x)
来源：http://hz.yangfankeji.com/gtengcledq.html

Java: list.contains(x)
来源：http://hz.jinqigfzy.top/gtwhtjihte.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhongyouzk.top/gtamncczpo.html

Ruby: arr.include?(x)
来源：http://hz.zdqjudy.top/gtzbezgnaq.html

C#:   list.Contains(x)
来源：http://hz.cdnleiting.top/gtfvmgtwgz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.smart0.xyz/gtvzfzlksl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinyuanbaomall.cn/gtbxxyqsng.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinqigufen.top/gthvjhmeau.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.vqdsnc.cn/gtwmuwdgtb.html

TS:   [...arr];
来源：http://hz.hnxiangtu.top/gtlgdzmyka.html

Java: new ArrayList<>(list);
来源：http://hz.quarkkingdee.top/gtfbujpgal.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shuidangran.top/gtwiwzldds.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gaohongyu789.top/gtuwsaefbm.html

C#:   new List<int>(list);
来源：http://hz.shanyushiyangkeji.top/gtbmbmmizl.html

[D23] reduce 累积计算
来源：http://hz.wangdashe.top/gtijcojvff.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.pycfn.com/gteovgmivx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jqgfzy.top/gtiikbmryd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hysaishi.cn/gtqurqslvg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.52xcode.cn/gticslwvmy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gotoacloud.top/gtwuznfmdt.html

Go:   // 手写循环
来源：http://hz.zhongyouzk.top/gthqdwlefd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jqgufenzy.top/gtxpyvoofi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yvedp.cn/gtssuegvha.html

[D24] 字典 / Map 基本操作
来源：http://hz.hongshengwenyu.top/gtgkxkdmpz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xylfe.cn/gtswgtzvli.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.c1oappe.top/gtgxgmfhrr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jqgufenzy.top/gtglafrvnf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cdnleiting.top/gtbybdpwok.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxinkj.top/gtwtpaingf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jinyuanbaomall.cn/gtuctbesvw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.tian-w.cn/gtqxfpqwnd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinqigfzy.top/gttzjqzdvx.html

[D25] Set 集合去重与交并差
来源：http://hz.nanxuanxn.top/gthwmstbly.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xinyue.icu/gtyijldjkk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gogol.net.cn/gtsmoztten.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cheryme.top/gtpigxhveg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yj20258.top/gtxowbvzhc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yonumen.top/gtgkkkotjz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hfpthk.cn/gtxgvfgtdm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shanyushiyangkeji.top/gtbcbnbkre.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yueranfly.top/gtziexlpmr.html

[D26] 数组转字符串
来源：http://hz.yvedp.cn/gtzjasejcw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.meibo888.top/gtjivvcvuj.html

PHP:  implode(", ", $arr);
来源：http://hz.nanxinkj.top/gtrbyvziak.html

JS:   arr.join(", ")
来源：http://hz.quarkkingdee.top/gtqooigzad.html

TS:   arr.join(", ")
来源：http://hz.gzhubu.top/gtzwqacckb.html

Java: String.join(", ", list)
来源：http://hz.shuidangran.top/gtxlsfvxbl.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yangfankeji.com/gtsqamqqao.html

Ruby: arr.join(", ")
来源：http://hz.vqdsnc.cn/gtsjmzcnwf.html

C#:   string.Join(", ", list)
来源：http://hz.birdmap.top/gtbqhcvkkx.html

================================================================================
来源：http://hz.daxiang520.top/gtglbkbviv.html

E. 字符串处理
来源：http://hz.yuxming.cn/gtwzdqwysr.html

================================================================================
来源：http://hz.9152youxi.cn/gtczsiifhm.html

[E01] 拼接字符串
来源：http://hz.316326.xyz/gtttemooix.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhaomingkeji.xyz/gtexnwmzlq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shanyushiyangkeji.top/gtqfvgdsge.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fengsongda.top/gtsipxfcwn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sufxvd.cn/gtwwvkdnzo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.svipenyu.cn/gtnfolzazm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yvedp.cn/gtgimptykc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinyuanbaomall.cn/gtenpifrzz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hywenlv.cn/gtuwlchspq.html

[E02] 重复字符串
来源：http://hz.tian-w.cn/gtnuzemelw.html

Py:   "ab" * 3
来源：http://hz.yvedp.cn/gtimolvpbi.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zycfv.cn/gtacpmxthj.html

JS:   "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtsgotibod.html

TS:   "ab".repeat(3)
来源：http://hz.fzhhl.top/gtratxrmqv.html

Java: "ab".repeat(3)
来源：http://hz.yj202588.top/gtvbugpqrv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ybcxt.top/gtizmgjtzc.html

Ruby: "ab" * 3
来源：http://hz.52xcode.cn/gthkrliwyu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xziqi.cn/gtseioopeg.html

[E03] 截取子串
来源：http://hz.cashguo.top/gtttwkblai.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.andypj.xyz/gtnwgphjoh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.vqdsnc.cn/gteobjbqnq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.tian-w.cn/gtggltzphq.html

TS:   s.slice(1, 4)
来源：http://hz.ywan-chungtsiang.top/gtsuslcgaa.html

Java: s.substring(1, 4)
来源：http://hz.jianghu66.top/gtjbfqoznv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cdnleiting.top/gtfzlfaazn.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.aibaodan.cn/gtqojqfhga.html

C#:   s.Substring(1, 3)
来源：http://hz.svipenyu.cn/gtyimbbzps.html

[E04] 查找子串位置
来源：http://hz.sxryk.cn/gtqstuklpe.html

Py:   s.find("x");  s.index("x")
来源：http://hz.kuanghao11.cn/gtwmsnunaj.html

PHP:  strpos($s, "x");
来源：http://hz.jyoumei.cn/gtffataxkg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shangyingyoupin.top/gtqajxguip.html

TS:   s.indexOf("x")
来源：http://hz.ivvv.top/gtgllftdnq.html

Java: s.indexOf("x")
来源：http://hz.jianghu66.top/gtomzliyec.html

Go:   strings.Index(s, "x")
来源：http://hz.svipenyu.cn/gthulxapuv.html

Ruby: s.index("x")
来源：http://hz.cucudq.cn/gtpfxbvdae.html

C#:   s.IndexOf("x")
来源：http://hz.wangshuangyany.cn/gtpvpzdgef.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhiwuduotai.top/gtvwmwusvr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ywan-chungtsiang.top/gtmtuyzwbi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hywenlv.cn/gtozckvxer.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cucudq.cn/gtybiqzryo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.andypj.xyz/gtjoqcdfet.html


<!-- 参考信息 -->