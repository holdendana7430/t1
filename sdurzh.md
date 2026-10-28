代发 wailian999

[C14] 泛型函数
来源：http://hz.yonumen.top/gtcnlpdarr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj20258888.top/gtjqqnlyrn.html

PHP:  // 无泛型
来源：http://hz.ehwqpu.com/gtjqmplbwi.html

JS:   // 无泛型
来源：http://hz.yangfankeji.com/gtoyfrnbzz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.fengsongda.top/gtqbwxyjez.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.aizwys.cn/gtqenrvxfs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gzhubu.top/gtusnltkkp.html

Ruby: # 无泛型
来源：http://hz.jinqigufen.top/gtnptjsbxs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jiagoushi.top/gtateflrtq.html

[C15] 解构 / 展开参数
来源：http://hz.pycfn.com/gthgsihybd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.birdmap.top/gtaeewdbxw.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shangyingyoupin.top/gtuigntwhi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinqigufen.top/gtmmhjqfmz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.sufxvd.cn/gtssyvfzed.html

Java: // 无解构
来源：http://hz.ydzc1.top/gtdfbydrac.html

Go:   // 无解构
来源：http://hz.svipenyu.cn/gtuqsfzxaa.html

Ruby: a, b = pair
来源：http://hz.hongshengwenyu.top/gtlkmalnzs.html

C#:   var (a, b) = pair;
来源：http://hz.yangfankeji.com/gtxeqwcoeg.html

[C16] 函数 / 方法重载
来源：http://hz.shanyushiyangtech.top/gtqvitnmce.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hongshengwenyu.top/gtfatilyle.html

PHP:  // 无重载
来源：http://hz.haohaochexian.top/gtvzxluibe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zdqjudy.top/gtzqysfcln.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.nanxuanxn.top/gtlrcpzmec.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenjidiqi.icu/gtbcqejsvs.html

Go:   // 无重载：用不同函数名
来源：http://hz.birdmap.top/gtrrjqngrz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cucudq.cn/gtarzljlre.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shangyingyoupin.top/gtecjzrtnf.html

================================================================================
来源：http://hz.jyoumei.cn/gttvgjmnse.html

D. 数组 / 列表 / 集合
来源：http://hz.xinyue.icu/gtimsspxmu.html

================================================================================
来源：http://hz.chenlongwang.top/gtqgaxmoll.html

[D01] 创建数组 / 列表
来源：http://hz.jianghu66.top/gtiapmxvlr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yueranfly.top/gthkpuktnr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinqigfzy.top/gtwsobbvoh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gogol.net.cn/gtxayptnhl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guowangkeji.top/gtwkckvdsn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.gzhubu.top/gtqtqntrvp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jqgufenzy.top/gttkxgkvnl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhongyouzk.top/gtzucauzun.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jinqigfzy.top/gtatjukfqd.html

[D02] 追加元素到末尾
来源：http://hz.yj202588.top/gtcwnraqht.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zdqjudy.top/gtgvqybaan.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sweek.top/gtazbvnvbn.html

JS:   arr.push(4);
来源：http://hz.nanxuanxn.top/gtmfvdiqbr.html

TS:   arr.push(4);
来源：http://hz.sufxvd.cn/gtehtqjhwr.html

Java: list.add(4);
来源：http://hz.fzhhl.top/gtnbngmswx.html

Go:   arr = append(arr, 4)
来源：http://hz.guannengcc.top/gtgmhulkvx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.pengpengdd.cyou/gtssspbpjy.html

C#:   list.Add(4);
来源：http://hz.pengpengdd.cyou/gtsidyszpa.html

[D03] 在指定位置插入元素
来源：http://hz.ivvv.top/gtzgjmjeld.html

Py:   arr.insert(0, 0)
来源：http://hz.birdmap.top/gtwptrzfdx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.316326.xyz/gtrrqbehyg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.vqdsnc.cn/gtaczzpger.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xingfuxueyuan.xyz/gtnwpsujsx.html

Java: list.add(0, 0);
来源：http://hz.chenjidiqi.icu/gtnykhhalv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jyoumei.cn/gtuvymzeut.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydzc1.top/gtoofcebvw.html

C#:   list.Insert(0, 0);
来源：http://hz.hfpthk.cn/gtakvcpcot.html

[D04] 删除元素
来源：http://hz.hywenlv.cn/gtvnxuwfhb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.52xcode.cn/gtwncrgvcx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shanyushiyangtech.top/gtivtfgyom.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gzhubu.top/gtgrkpvbhs.html

TS:   arr.splice(0, 1);
来源：http://hz.tanke756.top/gtoivwwdsu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gzhubu.top/gtodrtglrb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.chenzaomai.com/gtzzrrvkdt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gaohongyu789.top/gttbmbfhia.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinghuilouyu.cn/gtsnpzfeyx.html

[D05] 访问与修改元素
来源：http://hz.aibaodan.cn/gtdxaqkvip.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pengpengdd.cyou/gtczeqhdvk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yuxming.cn/gtxtenfcqh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.feifeiyinyue.top/gtwbeduwya.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.tian-w.cn/gtkewibsni.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.daria6918.cn/gtlebqocdo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtsnpxvmuu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtumpnlysc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhiwuduotai.top/gtqfaarour.html

[D06] 数组长度
来源：http://hz.havefunace.top/gtarkdvxfq.html

Py:   len(arr)
来源：http://hz.yanxiufei.cn/gtpifgrvbg.html

PHP:  count($arr);
来源：http://hz.hnxiangtu.top/gtwsdhjosa.html

JS:   arr.length
来源：http://hz.tian-w.cn/gtzblcqnhe.html

TS:   arr.length
来源：http://hz.haohaochexian.top/gttjzrreec.html

Java: list.size();
来源：http://hz.yuxming.cn/gtmotlrevo.html

Go:   len(arr)
来源：http://hz.nanxuanxn.top/gtbfvzfnzn.html

Ruby: arr.length; arr.size
来源：http://hz.hnxiangtu.top/gtreqndgcz.html

C#:   list.Count;
来源：http://hz.dashuyun.cn/gtxuiumxfq.html

[D07] 切片 / 取子数组
来源：http://hz.ywan-chungtsiang.top/gtpspwxthk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zycfv.cn/gtbxerjfsj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.pengpengdd.cyou/gtsujsbcmp.html

JS:   arr.slice(1, 4);
来源：http://hz.daria6918.cn/gtadiwdlwx.html

TS:   arr.slice(1, 4);
来源：http://hz.iojbl.cn/gtrbrvdgbz.html

Java: list.subList(1, 4);
来源：http://hz.ivvv.top/gthysefuav.html

Go:   arr[1:4]
来源：http://hz.chenlongwang.top/gtusqdxwjv.html

Ruby: arr[1, 3]
来源：http://hz.gotoacloud.top/gtnzfsqghu.html

C#:   list.GetRange(1, 3);
来源：http://hz.yangfankeji.com/gthsdljgmr.html

[D08] 合并两个数组
来源：http://hz.jinqigufen.top/gtldzzaxgc.html

Py:   a + b;  a.extend(b)
来源：http://hz.shanyushiyangkeji.top/gtqutgwanu.html

PHP:  array_merge($a, $b);
来源：http://hz.cqqwz.cn/gtvoupbglp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.andypj.xyz/gtsxgmqiep.html

TS:   [...a, ...b];
来源：http://hz.guannengcc.top/gtkstwffpo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gzhubu.top/gtkopkubpy.html

Go:   append(a, b...)
来源：http://hz.nwbrower.top/gtpnpzjvlx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.tanke756.top/gtlniemgky.html

C#:   a.Concat(b).ToList()
来源：http://hz.fengsongda.top/gtlikpmsfp.html

[D09] 排序（升序）
来源：http://hz.zhixingplan.top/gtqlyuydoj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtiznriozn.html

PHP:  sort($arr);
来源：http://hz.chenzaomai.com/gtueokuigw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.havefunace.top/gthqmacelv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.aizwys.cn/gtdfahylom.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xinyue.icu/gtpjkifpqc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.svipenyu.cn/gtvehwuudj.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtrpxrrxms.html

C#:   list.Sort();
来源：http://hz.jinqigfzy.top/gtnqxkvomh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gogol.net.cn/gtbffqwpsc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shzxlz.cn/gtxtlhikkg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.52xcode.cn/gtauixcrlk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daria6918.cn/gtufhxhfjt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhengqikj.top/gtxbozexki.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.aibaodan.cn/gtmbkacbfx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.nwbrower.top/gtqehuqcuq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jinqigufen.top/gtdwwgbjim.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jiagoushi.top/gtjcxzlysw.html

[D11] 反转数组
来源：http://hz.haohaochexian.top/gtpvmclkec.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.316326.xyz/gtcacgyxcs.html

PHP:  array_reverse($arr);
来源：http://hz.zhongyouzk.top/gtbvuaorer.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dashuyun.cn/gtczcntish.html

TS:   [...arr].reverse();
来源：http://hz.fengsongda.top/gtxozupipi.html

Java: Collections.reverse(list);
来源：http://hz.316326.xyz/gthinsboom.html

Go:   slices.Reverse(arr)
来源：http://hz.zdqjudy.top/gtjewvnsue.html

Ruby: arr.reverse
来源：http://hz.yangfankeji.com/gtdhazxcjt.html

C#:   list.Reverse();
来源：http://hz.jiagoushi.top/gtmbastcac.html

[D12] 查找元素下标
来源：http://hz.havefunace.top/gtjlefcgcj.html

Py:   arr.index(x);  x in arr
来源：http://hz.guannengcc.top/gtrinxkpmy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xuanzx.com/gtvcciqven.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgufenzy.top/gtivxmijjh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangkeji.top/gtsfipovui.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hnqzz.top/gturzfocar.html

Go:   slices.Index(arr, x)
来源：http://hz.svipenyu.cn/gtxqsdcjvk.html

Ruby: arr.index(x)
来源：http://hz.hongshengwenyu.top/gtnazmwxcv.html

C#:   list.IndexOf(x);
来源：http://hz.iojbl.cn/gtfakljcdj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.daria6918.cn/gtjvvhdict.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenlongwang.top/gtgnuaozet.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenzaomai.com/gtznqqojxe.html

JS:   arr.filter(x => x > 3)
来源：http://hz.guowangkeji.top/gtsdtprcrs.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yueranfly.top/gtpuzjggvf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.bjfxy.top/gtnlndmeox.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.kuanghao11.cn/gtmooptmcf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xylfe.cn/gtimclardj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtfqonhjus.html

[D14] 映射转换（每个元素变形）
来源：http://hz.havefunace.top/gtczlkoini.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhaomingkeji.xyz/gtxmdcentl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tianlin.xyz/gtrqihkksa.html

JS:   arr.map(x => x * 2)
来源：http://hz.jinqigfzy.top/gthjyimntx.html

TS:   arr.map(x => x * 2)
来源：http://hz.havefunace.top/gthjknlobq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yvedp.cn/gtaianwjof.html

Go:   // 手写循环
来源：http://hz.yangfankeji.com/gtddzbwayx.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hammf.cn/gtoqpvbaqb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ydzc1.top/gtcllyufhf.html

[D15] 去重
来源：http://hz.ppjwa.cn/gtquqdevbr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenzaomai.com/gtbvftgxbj.html

PHP:  array_unique($arr);
来源：http://hz.cheryme.top/gtjrvkcchc.html

JS:   [...new Set(arr)]
来源：http://hz.haohaochexian.top/gtifftfyqk.html

TS:   [...new Set(arr)]
来源：http://hz.yueranfly.top/gtnwbrlcws.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shanyushiyangkeji.top/gtvdkrsfge.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhoulong.xyz/gtjbyswygs.html

Ruby: arr.uniq
来源：http://hz.hongshengwenyu.top/gtumixofmz.html

C#:   list.Distinct().ToList()
来源：http://hz.vqdsnc.cn/gtadsxinpl.html

[D16] 求和与平均值
来源：http://hz.guannengcc.top/gtiqriufxj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.52xcode.cn/gtcmgyagjm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.guannengcc.top/gtktrqeoru.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258.top/gteapltsik.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.svipenyu.cn/gtekndbyzw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hongshengwenyu.top/gtkxqjgeyi.html

Go:   // 手写循环累加
来源：http://hz.sufxvd.cn/gtwzcwruek.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.pycfn.com/gtgoufsyix.html

C#:   list.Sum();  list.Average()
来源：http://hz.svipenyu.cn/gtruuusocf.html

[D17] 最大值与最小值
来源：http://hz.yj202588.top/gtaqzephje.html

Py:   max(arr);  min(arr)
来源：http://hz.cashguo.top/gtfchwokkn.html

PHP:  max($arr);  min($arr);
来源：http://hz.jqgfzy.top/gtqwuejquf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hongshengwenyu.top/gtvnextdqy.html

TS:   Math.max(...arr);
来源：http://hz.sufxvd.cn/gtvjwxshcf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhongyouzk.top/gtezqsmkyc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ivvv.top/gtffktjtgz.html

Ruby: arr.max;  arr.min
来源：http://hz.gogol.net.cn/gtdofjkyuc.html

C#:   list.Max();  list.Min()
来源：http://hz.mhx1999.top/gtozepmypa.html

[D18] 扁平化嵌套数组
来源：http://hz.nanxinkj.top/gtvckdhung.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sweek.top/gtdncmqzhy.html

PHP:  array_merge(...$nested);
来源：http://hz.yongpay.top/gtbbmaafye.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.316326.xyz/gtusuqhbhr.html

TS:   nested.flat();
来源：http://hz.shuidangran.top/gtyvaxnbyu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.pengpengdd.cyou/gtpvpalrbd.html

Go:   // 手写双层循环
来源：http://hz.xziqi.cn/gtmiylmzoa.html

Ruby: nested.flatten
来源：http://hz.quarkkingdee.top/gtmxdjjprr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nanxinkj.top/gtdxjmjkxq.html

[D19] 按字段分组
来源：http://hz.dashuyun.cn/gtauifzyfw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhaomingkeji.xyz/gtjvrpsanu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xuanzx.com/gtxiiwhhkf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ppjwa.cn/gtpruuxvuh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gtrkshfnyu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hnxiangtu.top/gtqxdblnha.html

Go:   // 手写 map[string][]T
来源：http://hz.nanxinkj.top/gtddwqnoxx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shuidangran.top/gtxofewlwd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nanxinkj.top/gtrjapaoft.html

[D20] 统计每个元素出现次数
来源：http://hz.meibo888.top/gtwjvzuidv.html

Py:   Counter(arr)
来源：http://hz.ywan-chungtsiang.top/gtvjsfhods.html

PHP:  array_count_values($arr);
来源：http://hz.snrcjt.cn/gtzczeotyz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ehwqpu.com/gtsygxgvct.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnqzz.top/gtxfmsvaiy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.pengpengdd.cyou/gtszaaxmbn.html

Go:   // 手写 map[T]int
来源：http://hz.shzxlz.cn/gtorgbhmob.html

Ruby: arr.tally
来源：http://hz.zhoulong.xyz/gtzyjcvbwy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hongshengwenyu.top/gtmvmbzxgo.html

[D21] 判断是否包含某元素
来源：http://hz.pycfn.com/gtqkklcxee.html

Py:   x in arr
来源：http://hz.tian-w.cn/gtrmluxghm.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xuanzx.com/gtspqyguau.html

JS:   arr.includes(x)
来源：http://hz.andypj.xyz/gtkxjnozli.html

TS:   arr.includes(x)
来源：http://hz.birdmap.top/gtezwpvavo.html

Java: list.contains(x)
来源：http://hz.nanxinkj.top/gtjadmzddl.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj202588.top/gtqehmxhvg.html

Ruby: arr.include?(x)
来源：http://hz.meibo888.top/gthncngtfo.html

C#:   list.Contains(x)
来源：http://hz.yj20258888.top/gtsrxuzzav.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sufxvd.cn/gtcudhkgbk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jyoumei.cn/gtdptcphlr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinqigufen.top/gtaplnlpjh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yvedp.cn/gtxfpklfyl.html

TS:   [...arr];
来源：http://hz.yueranfly.top/gtgnrmmrfy.html

Java: new ArrayList<>(list);
来源：http://hz.xuetiantiany.cn/gtavjdijdx.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.0kj1m.cn/gtugzcynxy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ehwqpu.com/gtbcpcvgbz.html

C#:   new List<int>(list);
来源：http://hz.chenzaomai.com/gtcetaozft.html

[D23] reduce 累积计算
来源：http://hz.nanxuanxn.top/gtxqtmebhy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xingfuxueyuan.xyz/gttqlffhpu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yuxming.cn/gtxsghjppd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ppjwa.cn/gtrjkybomm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.dashuyun.cn/gtukfoxrbb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.pengpengdd.cyou/gtdwdqsznb.html

Go:   // 手写循环
来源：http://hz.jqgfzy.top/gtqsbjuhgk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hongshengwenyu.top/gtdgjuktpj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.quarkkingdee.top/gtopktnbin.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj20258.top/gtibdhguqm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shanyushiyangtech.top/gtuudzuyex.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yonumen.top/gtszptppad.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ywan-chungtsiang.top/gtywvlejhm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.daria6918.cn/gtijrdoekh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.bjfxy.top/gtgurrhhau.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.tanke756.top/gtxphkszzv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sweek.top/gtmmpabiso.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinqigufen.top/gtsdiuolkq.html

[D25] Set 集合去重与交并差
来源：http://hz.nanxuanxn.top/gtjolnukkd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yuanzhike.top/gtphzclgjg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.bjfxy.top/gtigosonoy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.quarkkingdee.top/gttirkzfgl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.andypj.xyz/gtmbghvcwd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cashguo.top/gtnbgbqbgv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.chenzaomai.com/gtqmflgbon.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgfzy.top/gtuuhsvyeg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hnxiangtu.top/gtgbonyfuk.html

[D26] 数组转字符串
来源：http://hz.fzhhl.top/gtyronkgcf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.316326.xyz/gtqdcrfvmd.html

PHP:  implode(", ", $arr);
来源：http://hz.hysaishi.cn/gtfhbupcdo.html

JS:   arr.join(", ")
来源：http://hz.haohaochexian.top/gtxaskyirn.html

TS:   arr.join(", ")
来源：http://hz.daxiang520.top/gtpokneeqq.html

Java: String.join(", ", list)
来源：http://hz.cucudq.cn/gtpxscrpxt.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cheryme.top/gtrmtlbcmt.html

Ruby: arr.join(", ")
来源：http://hz.fzhhl.top/gtfywryzlt.html

C#:   string.Join(", ", list)
来源：http://hz.jqgfzy.top/gtqvafnukx.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtxwuqmmko.html

E. 字符串处理
来源：http://hz.jlsjyb.cn/gtbgxtzwoz.html

================================================================================
来源：http://hz.yongpay.top/gtyqqcnshm.html

[E01] 拼接字符串
来源：http://hz.zhijiandao.cn/gtfctvxhaa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shanyushiyangkeji.top/gttzqltbrb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhoulong.xyz/gtyvnqcrup.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gogol.net.cn/gtifsjnzto.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guannengcc.top/gtzsvuvluq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yongpay.top/gtfhczjfsi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yonumen.top/gtipfuifak.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yueranfly.top/gtjaqpttne.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.smart0.xyz/gtkqmszziz.html

[E02] 重复字符串
来源：http://hz.redwolf501.top/gtpxroejpo.html

Py:   "ab" * 3
来源：http://hz.chenzaomai.com/gtjtadwoer.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jianghu66.top/gtxxkfagsj.html

JS:   "ab".repeat(3)
来源：http://hz.ehwqpu.com/gtlekcmyaz.html

TS:   "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtrynstvnj.html

Java: "ab".repeat(3)
来源：http://hz.svipenyu.cn/gtdlrakkvo.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.316326.xyz/gtfbntccum.html

Ruby: "ab" * 3
来源：http://hz.cucudq.cn/gtcavtmgof.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenzaomai.com/gtepiuvabo.html

[E03] 截取子串
来源：http://hz.sxryk.cn/gtxkpsvgfy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.iojbl.cn/gtkrjujsdh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtvqxrwyiq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cheryme.top/gtxysgzase.html

TS:   s.slice(1, 4)
来源：http://hz.ydzc1.top/gthwyypkow.html

Java: s.substring(1, 4)
来源：http://hz.hnxiangtu.top/gtubdaxhne.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yangfankeji.com/gtpdbjsaes.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hnxiangtu.top/gtlqaeslfw.html

C#:   s.Substring(1, 3)
来源：http://hz.chenzaomai.com/gtstxfqhnz.html

[E04] 查找子串位置
来源：http://hz.quarkkingdee.top/gtgfvxmtzh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jqgfzy.top/gtliintszf.html

PHP:  strpos($s, "x");
来源：http://hz.hywenlv.cn/gtwcnczmyc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.daxiang520.top/gtdjqoyjck.html

TS:   s.indexOf("x")
来源：http://hz.smart0.xyz/gtmgaztrgp.html

Java: s.indexOf("x")
来源：http://hz.cheryme.top/gthjxzfzjv.html


<!-- 参考信息 -->