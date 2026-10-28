代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.aibaodan.cn/gtnyddrtfq.html

[C15] 解构 / 展开参数
来源：http://hz.yj20258888.top/gtwcijtwdl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.pycfn.com/gtywtrmowc.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jinghuilouyu.cn/gtjllgrjfw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.c1oappe.top/gtgqogpsis.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yj20258888.top/gtjgpuxgrs.html

Java: // 无解构
来源：http://hz.gaohongyu789.top/gtqaufyicc.html

Go:   // 无解构
来源：http://hz.jianghu66.top/gtswmrttdu.html

Ruby: a, b = pair
来源：http://hz.yongpay.top/gteixpqemu.html

C#:   var (a, b) = pair;
来源：http://hz.316326.xyz/gtgxcmbdzz.html

[C16] 函数 / 方法重载
来源：http://hz.hfpthk.cn/gtkweiezrn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hammf.cn/gtegwqamzc.html

PHP:  // 无重载
来源：http://hz.meibo888.top/gtkvdcujeo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jqgufenzy.top/gtlicxkhud.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.chenlongwang.top/gtjbbwsmmt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.pengpengdd.cyou/gtuxkhlrpa.html

Go:   // 无重载：用不同函数名
来源：http://hz.chenjidiqi.icu/gtqxcqmurl.html

Ruby: # 无重载：靠动态参数
来源：http://hz.wangshuangyany.cn/gtggfifhzf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.havefunace.top/gtcnfkfoko.html

================================================================================
来源：http://hz.haohaochexian.top/gtdclphieq.html

D. 数组 / 列表 / 集合
来源：http://hz.yuxming.cn/gtpkszgnew.html

================================================================================
来源：http://hz.vqdsnc.cn/gtoaqmnuio.html

[D01] 创建数组 / 列表
来源：http://hz.52xcode.cn/gtplxrxfds.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinqigufen.top/gtojhpbfpv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.pengpengdd.cyou/gtikbcfrmh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xinyue.icu/gtwatfctuo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.wangdashe.top/gtxjbiebzk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cqqwz.cn/gtbanuimzj.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.aizwys.cn/gtedeonrwo.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hnqzz.top/gtmhygkiex.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.snrcjt.cn/gttahdxany.html

[D02] 追加元素到末尾
来源：http://hz.ivvv.top/gtmsmmynpa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.dashuyun.cn/gtqrcmgouh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.nwbrower.top/gtqfvkowrx.html

JS:   arr.push(4);
来源：http://hz.ehwqpu.com/gtvzydgfbx.html

TS:   arr.push(4);
来源：http://hz.9152youxi.cn/gtvhzidhbn.html

Java: list.add(4);
来源：http://hz.ivvv.top/gtijicdkio.html

Go:   arr = append(arr, 4)
来源：http://hz.kuanghao11.cn/gtqumlktqu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hfpthk.cn/gttrwkyaru.html

C#:   list.Add(4);
来源：http://hz.hnqzz.top/gtpyfobjiy.html

[D03] 在指定位置插入元素
来源：http://hz.c1oappe.top/gtqwirbznu.html

Py:   arr.insert(0, 0)
来源：http://hz.hywenlv.cn/gttcrzajur.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ehwqpu.com/gtcsaehxme.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.havefunace.top/gtaslxnmlm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yangfankeji.com/gteyywffgz.html

Java: list.add(0, 0);
来源：http://hz.pycfn.com/gtgafcuaxe.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xuetiantiany.cn/gtpzmwhuya.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xylfe.cn/gtfkxjrgws.html

C#:   list.Insert(0, 0);
来源：http://hz.sweek.top/gtcoydnlym.html

[D04] 删除元素
来源：http://hz.fzhhl.top/gtttljdnql.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ywan-chungtsiang.top/gtnjauccer.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gaohongyu789.top/gtrqseyajx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.0kj1m.cn/gtiarjakwp.html

TS:   arr.splice(0, 1);
来源：http://hz.guowangkeji.top/gtpyciqxrf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.nanxinkj.top/gtkcukjoeo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.aizwys.cn/gtydhxmbkk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.iojbl.cn/gtyqpgtpoz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.pycfn.com/gtzllnjkbr.html

[D05] 访问与修改元素
来源：http://hz.zhengqikj.top/gthhhwmzjh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.c1oappe.top/gthnuedodk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.dianchejie.cn/gtpsgbxbxf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sweek.top/gtfabmvyms.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xuanzx.com/gtywpisiej.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guannengcc.top/gtvrkazwdo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yj20258.top/gtsvpxphep.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenjidiqi.icu/gtglvhcvan.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gzhubu.top/gtfscrrbrx.html

[D06] 数组长度
来源：http://hz.nanxinkj.top/gttzswyogm.html

Py:   len(arr)
来源：http://hz.zhaomingkeji.xyz/gtrfgovhmh.html

PHP:  count($arr);
来源：http://hz.jqgufenzy.top/gtqjljlzfz.html

JS:   arr.length
来源：http://hz.redwolf501.top/gtwxnnsrvj.html

TS:   arr.length
来源：http://hz.yj202588.top/gtokjpmhhr.html

Java: list.size();
来源：http://hz.xuanzx.com/gtwaxzmofu.html

Go:   len(arr)
来源：http://hz.hnxiangtu.top/gtejjhxbdg.html

Ruby: arr.length; arr.size
来源：http://hz.ydzc1.top/gtgskstgwn.html

C#:   list.Count;
来源：http://hz.xziqi.cn/gtjrzzjjxn.html

[D07] 切片 / 取子数组
来源：http://hz.sweek.top/gtshiwccne.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hfpthk.cn/gtgmykccot.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.316326.xyz/gtgpepcqhe.html

JS:   arr.slice(1, 4);
来源：http://hz.guannengcc.top/gtukhqheep.html

TS:   arr.slice(1, 4);
来源：http://hz.yangfankeji.com/gtodqzwfbg.html

Java: list.subList(1, 4);
来源：http://hz.vqdsnc.cn/gtlilawuuq.html

Go:   arr[1:4]
来源：http://hz.316326.xyz/gtpsqrqvle.html

Ruby: arr[1, 3]
来源：http://hz.shzxlz.cn/gtejilftbv.html

C#:   list.GetRange(1, 3);
来源：http://hz.chenzaomai.com/gtksfreogm.html

[D08] 合并两个数组
来源：http://hz.ybcxt.top/gtoputdkue.html

Py:   a + b;  a.extend(b)
来源：http://hz.ivvv.top/gtgmcymciq.html

PHP:  array_merge($a, $b);
来源：http://hz.svipenyu.cn/gtxtdzwstz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shuidangran.top/gtxdygrgdh.html

TS:   [...a, ...b];
来源：http://hz.chenzaomai.com/gtxmtptvpk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.nanxuanxn.top/gtymwwcwaf.html

Go:   append(a, b...)
来源：http://hz.birdmap.top/gtnjpjthez.html

Ruby: a + b;  a.concat(b)
来源：http://hz.wangshuangyany.cn/gtcncpdwvv.html

C#:   a.Concat(b).ToList()
来源：http://hz.hysaishi.cn/gtsrvcqcxo.html

[D09] 排序（升序）
来源：http://hz.sxryk.cn/gtdtxweckv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xinyue.icu/gtynbcfhwg.html

PHP:  sort($arr);
来源：http://hz.zycfv.cn/gtphbcmisl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ywan-chungtsiang.top/gtvsombvxd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.tianlin.xyz/gtzwpskoyj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.wangdashe.top/gtfzgghroe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.chenjidiqi.icu/gtthdexcgj.html

Ruby: arr.sort
来源：http://hz.yueranfly.top/gtigmhyhyh.html

C#:   list.Sort();
来源：http://hz.bjfxy.top/gtnrketruo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ydjk.org.cn/gtgddkutye.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shuidangran.top/gtcpdtkfun.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nwbrower.top/gtxacygaej.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daxiang520.top/gthrplepxc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnqzz.top/gtpmilqfgp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yvedp.cn/gtgmqvybwj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ivvv.top/gtpgvenobe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.c1oappe.top/gtezrdrudp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.dashuyun.cn/gtgohllsjd.html

[D11] 反转数组
来源：http://hz.zhixingplan.top/gtfyshwtvq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.dianchejie.cn/gtidtpdfhz.html

PHP:  array_reverse($arr);
来源：http://hz.cashguo.top/gtfxoqnehy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.sysykeji.top/gtnvrqjrtg.html

TS:   [...arr].reverse();
来源：http://hz.pycfn.com/gtudnxapoa.html

Java: Collections.reverse(list);
来源：http://hz.zhongyouzk.top/gtbuqdqjuf.html

Go:   slices.Reverse(arr)
来源：http://hz.hywenlv.cn/gtlbjkhubo.html

Ruby: arr.reverse
来源：http://hz.jinqigfzy.top/gtvoumplxw.html

C#:   list.Reverse();
来源：http://hz.gogol.net.cn/gtgwaubplz.html

[D12] 查找元素下标
来源：http://hz.shanyushiyangtech.top/gtvndwzedw.html

Py:   arr.index(x);  x in arr
来源：http://hz.gotoacloud.top/gtsjxxbkgp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zycfv.cn/gtoutywsgx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ybcxt.top/gtajsijovw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xziqi.cn/gtjfvxiuut.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.0kj1m.cn/gtcqnocmzl.html

Go:   slices.Index(arr, x)
来源：http://hz.shanyushiyangtech.top/gtsfbyjihf.html

Ruby: arr.index(x)
来源：http://hz.sufxvd.cn/gtlybfhctj.html

C#:   list.IndexOf(x);
来源：http://hz.hywenlv.cn/gtwovzsllb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ehwqpu.com/gtaultxcmy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenzaomai.com/gtkxloladv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinqigufen.top/gtrjuytxzy.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hnxiangtu.top/gtpraignjo.html

TS:   arr.filter(x => x > 3)
来源：http://hz.chenzaomai.com/gtvmrbafzz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.316326.xyz/gtjkpnszfo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.sufxvd.cn/gtuvlqfdci.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinghuilouyu.cn/gtyzkblcol.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cucudq.cn/gttgjktmnl.html

[D14] 映射转换（每个元素变形）
来源：http://hz.andypj.xyz/gtmoxcmsjc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hysaishi.cn/gtzglkqoej.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.fengsongda.top/gtcvgumxbn.html

JS:   arr.map(x => x * 2)
来源：http://hz.redwolf501.top/gtlcnbfxnd.html

TS:   arr.map(x => x * 2)
来源：http://hz.jianghu66.top/gtobytvikl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.andypj.xyz/gthcwqwxkk.html

Go:   // 手写循环
来源：http://hz.cashguo.top/gttouqsfzi.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.52xcode.cn/gtirqjfdka.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yonumen.top/gtfckqwiny.html

[D15] 去重
来源：http://hz.chenzaomai.com/gtznalzgcj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xuetiantiany.cn/gtfzjqorhc.html

PHP:  array_unique($arr);
来源：http://hz.9152youxi.cn/gtuwlkykyf.html

JS:   [...new Set(arr)]
来源：http://hz.yongpay.top/gtrffsuytl.html

TS:   [...new Set(arr)]
来源：http://hz.cucudq.cn/gtlygzbnmt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nanxuanxn.top/gtelfwfhkf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hywenlv.cn/gtcrlqnbut.html

Ruby: arr.uniq
来源：http://hz.jqgfzy.top/gteyrgkphp.html

C#:   list.Distinct().ToList()
来源：http://hz.vqdsnc.cn/gtsxdlltdr.html

[D16] 求和与平均值
来源：http://hz.9152youxi.cn/gtqdzpmfxw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.svipenyu.cn/gtzzjzktex.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hywenlv.cn/gtosilsvuu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.andypj.xyz/gtchctqyrp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhiwuduotai.top/gtjpwawsnj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xylfe.cn/gtzvofkzwb.html

Go:   // 手写循环累加
来源：http://hz.ivvv.top/gtffwrhrqm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jqgfzy.top/gtmqmaqkwq.html

C#:   list.Sum();  list.Average()
来源：http://hz.nanxuanxn.top/gtambjnwxa.html

[D17] 最大值与最小值
来源：http://hz.zhijiandao.cn/gtwdvqqsta.html

Py:   max(arr);  min(arr)
来源：http://hz.jlsjyb.cn/gtkhmukpvt.html

PHP:  max($arr);  min($arr);
来源：http://hz.jlsjyb.cn/gtnarrneuy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhijiandao.cn/gtbruddroq.html

TS:   Math.max(...arr);
来源：http://hz.zhengqikj.top/gtstodqmxo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhoulong.xyz/gtfjssiirp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangdashe.top/gtupvgqbkf.html

Ruby: arr.max;  arr.min
来源：http://hz.shuidangran.top/gttzkdhgnq.html

C#:   list.Max();  list.Min()
来源：http://hz.svipenyu.cn/gtfjyarkek.html

[D18] 扁平化嵌套数组
来源：http://hz.yonumen.top/gtsvjnhjkd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.316326.xyz/gtokddhcyb.html

PHP:  array_merge(...$nested);
来源：http://hz.haohaochexian.top/gtucfyctkg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhoulong.xyz/gtcnpwewsw.html

TS:   nested.flat();
来源：http://hz.shzxlz.cn/gtoaxryguz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dianchejie.cn/gtacqmmyle.html

Go:   // 手写双层循环
来源：http://hz.ydzc1.top/gtthbvtmsx.html

Ruby: nested.flatten
来源：http://hz.ppjwa.cn/gtgwwfgfea.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xinyue.icu/gtjorceoib.html

[D19] 按字段分组
来源：http://hz.yanxiufei.cn/gtvftkbfjb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.guannengcc.top/gtiqawiewp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jianghu66.top/gtdwsdunwu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenlongwang.top/gtcnziqypk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yonumen.top/gtzkgomcic.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.nwbrower.top/gtxxjelsxb.html

Go:   // 手写 map[string][]T
来源：http://hz.xylfe.cn/gtfgmjxjyd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.316326.xyz/gthlmjlhyg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.tian-w.cn/gtvwbuibct.html

[D20] 统计每个元素出现次数
来源：http://hz.guannengcc.top/gtebroaohu.html

Py:   Counter(arr)
来源：http://hz.tianlin.xyz/gthlkhxlpp.html

PHP:  array_count_values($arr);
来源：http://hz.xziqi.cn/gtcqdbwcqd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cashguo.top/gtaoscgzik.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.haohaochexian.top/gtxebvpgjc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.haohaochexian.top/gtmqqixmnj.html

Go:   // 手写 map[T]int
来源：http://hz.tanke756.top/gtraptcgyk.html

Ruby: arr.tally
来源：http://hz.zhoulong.xyz/gtxjavmogo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gotoacloud.top/gtujysnfep.html

[D21] 判断是否包含某元素
来源：http://hz.yueranfly.top/gtgpfnjlnr.html

Py:   x in arr
来源：http://hz.guannengcc.top/gtecvgmfvr.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xziqi.cn/gtffwakttg.html

JS:   arr.includes(x)
来源：http://hz.havefunace.top/gtmqzwixlr.html

TS:   arr.includes(x)
来源：http://hz.shanyushiyangkeji.top/gthxnilxam.html

Java: list.contains(x)
来源：http://hz.jlsjyb.cn/gtlxtdcbpc.html

Go:   slices.Contains(arr, x)
来源：http://hz.daria6918.cn/gtwqddxvmj.html

Ruby: arr.include?(x)
来源：http://hz.havefunace.top/gtybibwbrt.html

C#:   list.Contains(x)
来源：http://hz.havefunace.top/gtjyjyedfp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.9152youxi.cn/gtkxomaghv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.daria6918.cn/gtcrhxvetf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cdnleiting.top/gtrgtubkgt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.smart0.xyz/gtoywcrzdy.html

TS:   [...arr];
来源：http://hz.yj20258.top/gtjjgjvhwy.html

Java: new ArrayList<>(list);
来源：http://hz.jlsjyb.cn/gtuxsnispz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xylfe.cn/gteerooqwg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jiagoushi.top/gtkkzbzdav.html

C#:   new List<int>(list);
来源：http://hz.9152youxi.cn/gtiemcazjb.html

[D23] reduce 累积计算
来源：http://hz.sufxvd.cn/gtowrjhwwd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jianghu66.top/gtiqkwzodw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.iojbl.cn/gtzrmuwgeb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxuanxn.top/gtgjqdxryg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinyuanbaomall.cn/gtqnfflefr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj20258.top/gtfklmztgv.html

Go:   // 手写循环
来源：http://hz.jlsjyb.cn/gtwnsddequ.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sufxvd.cn/gtrynzdfip.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj20258.top/gtholvqfve.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinghuilouyu.cn/gtgvnymzma.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yj20258.top/gtlbvrbzvs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangkeji.top/gtawocttdx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yuanzhike.top/gtbvdgkrhu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.haohaochexian.top/gtebsizgxt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxinkj.top/gtitdpksaf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gotoacloud.top/gtozvougdj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ivvv.top/gtwpqivrlr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yangfankeji.com/gtrssyrtxe.html

[D25] Set 集合去重与交并差
来源：http://hz.redwolf501.top/gtaisphuob.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.mhx1999.top/gttiravzcu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.redwolf501.top/gtcflxoheh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xziqi.cn/gtsvgungcp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ybcxt.top/gtoqvssekk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sysykeji.top/gtcpxkhlts.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ivvv.top/gtyhkdstxo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shanyushiyangkeji.top/gtjvksueif.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.pengpengdd.cyou/gtyctnkoad.html

[D26] 数组转字符串
来源：http://hz.jiagoushi.top/gtvchbzint.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hysaishi.cn/gtoioonwtg.html

PHP:  implode(", ", $arr);
来源：http://hz.aibaodan.cn/gtxjbxgkgw.html

JS:   arr.join(", ")
来源：http://hz.sufxvd.cn/gthqpwoehs.html

TS:   arr.join(", ")
来源：http://hz.kuanghao11.cn/gtpcsigqzp.html

Java: String.join(", ", list)
来源：http://hz.dashuyun.cn/gtcxzenoqy.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gogol.net.cn/gtpvxjrfnm.html

Ruby: arr.join(", ")
来源：http://hz.hongshengwenyu.top/gtlhtsrtmj.html

C#:   string.Join(", ", list)
来源：http://hz.ppjwa.cn/gtjsoufayd.html

================================================================================
来源：http://hz.zhengqikj.top/gtvgkxoqcd.html

E. 字符串处理
来源：http://hz.jyoumei.cn/gtaixjhgax.html

================================================================================
来源：http://hz.dianchejie.cn/gteneuvfkh.html

[E01] 拼接字符串
来源：http://hz.dianchejie.cn/gttjpjwpov.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gzhubu.top/gtyjgyzaev.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cheryme.top/gthcdpkczw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ppjwa.cn/gttrrvmtap.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.mhx1999.top/gttsuuqxsa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.fengsongda.top/gtpjrzcbgc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.guowangkeji.top/gtkozacnfn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.chenjidiqi.icu/gtukvvdtrb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.52xcode.cn/gtegzlphps.html

[E02] 重复字符串
来源：http://hz.yanxiufei.cn/gtgfcwhaao.html

Py:   "ab" * 3
来源：http://hz.ehwqpu.com/gtbtmavqot.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cheryme.top/gtveuiqske.html

JS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtwfqgmrax.html

TS:   "ab".repeat(3)
来源：http://hz.sysykeji.top/gtznttanhr.html

Java: "ab".repeat(3)
来源：http://hz.yj202588.top/gtmsauksou.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cheryme.top/gtudxzetuf.html

Ruby: "ab" * 3
来源：http://hz.jinyuanbaomall.cn/gtmmsukmbn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhiwuduotai.top/gtnspwmgaw.html

[E03] 截取子串
来源：http://hz.nanxuanxn.top/gtkwijjqxa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jlsjyb.cn/gtxxcyjumg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.wangshuangyany.cn/gtobtasvdo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.dianchejie.cn/gtnqfytvml.html

TS:   s.slice(1, 4)
来源：http://hz.chenlongwang.top/gtyrspdqzu.html

Java: s.substring(1, 4)
来源：http://hz.hysaishi.cn/gtyfkzerif.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xylfe.cn/gtwebllpui.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jqgufenzy.top/gtgpgolybb.html

C#:   s.Substring(1, 3)
来源：http://hz.svipenyu.cn/gtyrfkgyjx.html

[E04] 查找子串位置
来源：http://hz.shzxlz.cn/gtecqvhdvz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.vqdsnc.cn/gtoccugieh.html

PHP:  strpos($s, "x");
来源：http://hz.guowangkeji.top/gticzldxku.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj20258.top/gtorozwgyz.html

TS:   s.indexOf("x")
来源：http://hz.316326.xyz/gtqeiwpsnw.html

Java: s.indexOf("x")
来源：http://hz.feifeiyinyue.top/gtdmdfkkjy.html

Go:   strings.Index(s, "x")
来源：http://hz.cqqwz.cn/gtokldmlwa.html

Ruby: s.index("x")
来源：http://hz.yangfankeji.com/gtwltibazz.html

C#:   s.IndexOf("x")
来源：http://hz.jinyuanbaomall.cn/gtntiujsop.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jiagoushi.top/gtrtsghasm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hnxiangtu.top/gtbgcvcule.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhoulong.xyz/gtqbvrhoar.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhaomingkeji.xyz/gtjzqeqahu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.mhx1999.top/gttuxpoijo.html


<!-- 参考信息 -->