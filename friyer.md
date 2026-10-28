代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.haohaochexian.top/gtfpkvqkwx.html

[C15] 解构 / 展开参数
来源：http://hz.0kj1m.cn/gtsrcmtuhs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sxryk.cn/gtneynmrtr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.andypj.xyz/gtajvkxwmx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xziqi.cn/gtxmgmjxlv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shzxlz.cn/gteuestacr.html

Java: // 无解构
来源：http://hz.mhx1999.top/gtxohrryko.html

Go:   // 无解构
来源：http://hz.jqgufenzy.top/gtrrjnexrj.html

Ruby: a, b = pair
来源：http://hz.zhiwuduotai.top/gtoxnihtho.html

C#:   var (a, b) = pair;
来源：http://hz.guannengcc.top/gtjhcfvpsc.html

[C16] 函数 / 方法重载
来源：http://hz.jianghu66.top/gtszpogops.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yonumen.top/gtlmaszllw.html

PHP:  // 无重载
来源：http://hz.0kj1m.cn/gtdrxtkwfl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.guannengcc.top/gtzvyfqwap.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhengqikj.top/gtugsqezph.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yueranfly.top/gtanpanudv.html

Go:   // 无重载：用不同函数名
来源：http://hz.gogol.net.cn/gtkosonamp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ybcxt.top/gtgddditeq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.sysykeji.top/gtgsvjipzk.html

================================================================================
来源：http://hz.gogol.net.cn/gtjjacsrgl.html

D. 数组 / 列表 / 集合
来源：http://hz.snrcjt.cn/gtfganuxdr.html

================================================================================
来源：http://hz.jinqigfzy.top/gtxubyhgpz.html

[D01] 创建数组 / 列表
来源：http://hz.jinqigfzy.top/gtrnhnfkbw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.redwolf501.top/gtavisfhac.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.nanxinkj.top/gttxcqkova.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zycfv.cn/gtzngnwlin.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.iojbl.cn/gtnueqbsqf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhoulong.xyz/gtqkxxqzal.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cucudq.cn/gtqzjjnhzb.html

Ruby: arr = [1, 2, 3]
来源：http://hz.andypj.xyz/gttiiagkyq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.guowangkeji.top/gtmafbwjsl.html

[D02] 追加元素到末尾
来源：http://hz.haohaochexian.top/gtytditbrq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xinyue.icu/gtcglhwazc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jqgfzy.top/gthdhjjwdy.html

JS:   arr.push(4);
来源：http://hz.zhoulong.xyz/gtqakixfst.html

TS:   arr.push(4);
来源：http://hz.svipenyu.cn/gtbyfbpdqu.html

Java: list.add(4);
来源：http://hz.cheryme.top/gtzycpcuzr.html

Go:   arr = append(arr, 4)
来源：http://hz.nanxuanxn.top/gtguscexsq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.kuanghao11.cn/gthkjwfpqz.html

C#:   list.Add(4);
来源：http://hz.gzhubu.top/gthxpoiohl.html

[D03] 在指定位置插入元素
来源：http://hz.aizwys.cn/gtbpcyuxge.html

Py:   arr.insert(0, 0)
来源：http://hz.316326.xyz/gtbebrdcbv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shanyushiyangtech.top/gtiayfootk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.snrcjt.cn/gtvwdjmhiw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.feifeiyinyue.top/gtoiaxrcke.html

Java: list.add(0, 0);
来源：http://hz.yj20258888.top/gtlkptyuge.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xingfuxueyuan.xyz/gtnopkaytx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jqgufenzy.top/gtyzfepibh.html

C#:   list.Insert(0, 0);
来源：http://hz.sxryk.cn/gtbrqaczlr.html

[D04] 删除元素
来源：http://hz.hysaishi.cn/gtymoooups.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.wangdashe.top/gtybonjbuu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xinyue.icu/gtixlxudtk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.quarkkingdee.top/gtwwpaspbo.html

TS:   arr.splice(0, 1);
来源：http://hz.shanyushiyangkeji.top/gtnthpdlvj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.pengpengdd.cyou/gtfzblcmla.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cucudq.cn/gtwvfhfgyd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jqgufenzy.top/gtsgqzfvlf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenlongwang.top/gtxjsrdmag.html

[D05] 访问与修改元素
来源：http://hz.guannengcc.top/gteojiocam.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuanzx.com/gtwuoalrde.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.snrcjt.cn/gtwlofykur.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinyuanbaomall.cn/gtpyjkcytu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shzxlz.cn/gttzenlbnq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tianlin.xyz/gtahtizdue.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.dashuyun.cn/gtaqntsolx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cdnleiting.top/gtjjqbogyh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gogol.net.cn/gtbavbgzma.html

[D06] 数组长度
来源：http://hz.birdmap.top/gtbnrcxssm.html

Py:   len(arr)
来源：http://hz.gogol.net.cn/gtgllomzvf.html

PHP:  count($arr);
来源：http://hz.yanxiufei.cn/gtjzzmiodp.html

JS:   arr.length
来源：http://hz.ywan-chungtsiang.top/gtjzrtwzos.html

TS:   arr.length
来源：http://hz.ybcxt.top/gtwcjnfcrt.html

Java: list.size();
来源：http://hz.havefunace.top/gtopvejqxq.html

Go:   len(arr)
来源：http://hz.tanke756.top/gtvsgmjvgb.html

Ruby: arr.length; arr.size
来源：http://hz.jyoumei.cn/gtkxvtmjse.html

C#:   list.Count;
来源：http://hz.hysaishi.cn/gthqnofqml.html

[D07] 切片 / 取子数组
来源：http://hz.fzhhl.top/gtmwtomvqe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.meibo888.top/gtsgprruht.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shanyushiyangtech.top/gtnlgasffx.html

JS:   arr.slice(1, 4);
来源：http://hz.hysaishi.cn/gtksdesido.html

TS:   arr.slice(1, 4);
来源：http://hz.mhx1999.top/gtksrxubrr.html

Java: list.subList(1, 4);
来源：http://hz.sysykeji.top/gtvbbofftl.html

Go:   arr[1:4]
来源：http://hz.yj20258888.top/gtomfmbvyj.html

Ruby: arr[1, 3]
来源：http://hz.vqdsnc.cn/gtfybylsat.html

C#:   list.GetRange(1, 3);
来源：http://hz.aibaodan.cn/gtwvmhcrvc.html

[D08] 合并两个数组
来源：http://hz.fzhhl.top/gtgsctmbrl.html

Py:   a + b;  a.extend(b)
来源：http://hz.yvedp.cn/gtegqjwjom.html

PHP:  array_merge($a, $b);
来源：http://hz.jyoumei.cn/gtggeoalrj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.andypj.xyz/gtqspfcanx.html

TS:   [...a, ...b];
来源：http://hz.yvedp.cn/gtsleqrbfu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sweek.top/gtrpfamhuy.html

Go:   append(a, b...)
来源：http://hz.ydjk.org.cn/gtygdbcuxi.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shanyushiyangtech.top/gtesnamxqu.html

C#:   a.Concat(b).ToList()
来源：http://hz.9152youxi.cn/gtutrjtmga.html

[D09] 排序（升序）
来源：http://hz.feifeiyinyue.top/gtdlhnmgex.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pycfn.com/gtbucszbxl.html

PHP:  sort($arr);
来源：http://hz.zhijiandao.cn/gtosntqrtx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jiagoushi.top/gtuvymcvjp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yuanzhike.top/gtctofmvfu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhoulong.xyz/gtacrpdnem.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.meibo888.top/gtigdtbfmd.html

Ruby: arr.sort
来源：http://hz.cheryme.top/gthoxhrgqv.html

C#:   list.Sort();
来源：http://hz.zhixingplan.top/gtybuorzzs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.daria6918.cn/gtrdwrpwnv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.haohaochexian.top/gtoblvcahp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258888.top/gtripmimug.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.dianchejie.cn/gtsyawyqyb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258.top/gtzzoptryg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shangyingyoupin.top/gtxfzidqmv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hongshengwenyu.top/gtptogzcus.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jianghu66.top/gttovdkqil.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yvedp.cn/gtwbeagmbh.html

[D11] 反转数组
来源：http://hz.316326.xyz/gtpirvvfna.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.mhx1999.top/gtgoxqbyah.html

PHP:  array_reverse($arr);
来源：http://hz.yj202588.top/gtqljehagl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.nanxinkj.top/gtwqykxajs.html

TS:   [...arr].reverse();
来源：http://hz.jinqigufen.top/gtxwpplthu.html

Java: Collections.reverse(list);
来源：http://hz.andypj.xyz/gtujjskjgf.html

Go:   slices.Reverse(arr)
来源：http://hz.yongpay.top/gtjhzmvogk.html

Ruby: arr.reverse
来源：http://hz.hnxiangtu.top/gthuaqksay.html

C#:   list.Reverse();
来源：http://hz.xuetiantiany.cn/gtywhtxays.html

[D12] 查找元素下标
来源：http://hz.gaohongyu789.top/gtjvnnkdux.html

Py:   arr.index(x);  x in arr
来源：http://hz.yvedp.cn/gtmgfehkhb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shanyushiyangtech.top/gtfyeaoyqw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenjidiqi.icu/gtruzxzghx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yonumen.top/gthmnguwdc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.smart0.xyz/gteqhtmapk.html

Go:   slices.Index(arr, x)
来源：http://hz.shuidangran.top/gtkmhtxhcx.html

Ruby: arr.index(x)
来源：http://hz.yj202588.top/gtuiwphpuq.html

C#:   list.IndexOf(x);
来源：http://hz.chenzaomai.com/gtyfhkeyrl.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tian-w.cn/gtdzfcxfnq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ehwqpu.com/gtxjoktoeu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sweek.top/gtboncsryv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtbihjkagb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.kuanghao11.cn/gtlowxtjcv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.aizwys.cn/gtlkvjybyw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xylfe.cn/gtmnzwdplp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jianghu66.top/gtkcybybcw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.snrcjt.cn/gtagdmfmee.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shangyingyoupin.top/gtkicaihps.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jiagoushi.top/gtadwamcpq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.svipenyu.cn/gtolerfgus.html

JS:   arr.map(x => x * 2)
来源：http://hz.yuanzhike.top/gtfymdxmyz.html

TS:   arr.map(x => x * 2)
来源：http://hz.jyoumei.cn/gtypysfenw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.daria6918.cn/gtdhdhrobg.html

Go:   // 手写循环
来源：http://hz.svipenyu.cn/gtazzykfrq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.kuanghao11.cn/gtkyijrcsm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.sysykeji.top/gtionalmnq.html

[D15] 去重
来源：http://hz.yuanzhike.top/gtifzxcbpc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.vqdsnc.cn/gtjnoiksvj.html

PHP:  array_unique($arr);
来源：http://hz.hongshengwenyu.top/gtwbfwwigr.html

JS:   [...new Set(arr)]
来源：http://hz.sufxvd.cn/gtxricnnjn.html

TS:   [...new Set(arr)]
来源：http://hz.kuanghao11.cn/gtrwpjlwid.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinqigufen.top/gtahpfyjtf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pengpengdd.cyou/gtuziqpmzi.html

Ruby: arr.uniq
来源：http://hz.ybcxt.top/gtcvjiglop.html

C#:   list.Distinct().ToList()
来源：http://hz.dianchejie.cn/gtldbuscke.html

[D16] 求和与平均值
来源：http://hz.kuanghao11.cn/gteffazdni.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ivvv.top/gtxcxicizt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.daria6918.cn/gtyeodlqim.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhaomingkeji.xyz/gtyyztpswj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgfzy.top/gtigjbdefc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.haohaochexian.top/gtxrhpzrwe.html

Go:   // 手写循环累加
来源：http://hz.dashuyun.cn/gtbwjxnwav.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shangyingyoupin.top/gtnixabjmq.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenlongwang.top/gtalyqkhun.html

[D17] 最大值与最小值
来源：http://hz.redwolf501.top/gtalkxpxcs.html

Py:   max(arr);  min(arr)
来源：http://hz.shuidangran.top/gtynukhyhf.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258888.top/gtubgivzrb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.daxiang520.top/gtackayyhx.html

TS:   Math.max(...arr);
来源：http://hz.gogol.net.cn/gtzrczxfhq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhixingplan.top/gtilztxtpe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.fzhhl.top/gtjgfyxpry.html

Ruby: arr.max;  arr.min
来源：http://hz.quarkkingdee.top/gtxxalcfpb.html

C#:   list.Max();  list.Min()
来源：http://hz.gogol.net.cn/gttijbzrru.html

[D18] 扁平化嵌套数组
来源：http://hz.tanke756.top/gtqvzcrwzd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zdqjudy.top/gttnscvnee.html

PHP:  array_merge(...$nested);
来源：http://hz.andypj.xyz/gtystezmhq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cheryme.top/gtbovwnsgm.html

TS:   nested.flat();
来源：http://hz.kuanghao11.cn/gtuqdqaeth.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj202588.top/gtfoosgjfq.html

Go:   // 手写双层循环
来源：http://hz.wangdashe.top/gtnbunggja.html

Ruby: nested.flatten
来源：http://hz.zdqjudy.top/gtqypgqwjg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jqgfzy.top/gtzysjaofd.html

[D19] 按字段分组
来源：http://hz.svipenyu.cn/gtadfpsyya.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.9152youxi.cn/gtzsacsivg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258.top/gthctebwqs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hongshengwenyu.top/gtbuelhbzo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.havefunace.top/gtsyiuejtr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenlongwang.top/gtpqpmdkvz.html

Go:   // 手写 map[string][]T
来源：http://hz.zhoulong.xyz/gthbxnxyhj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.redwolf501.top/gtqslcztxy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.tian-w.cn/gtoxjnvuzt.html

[D20] 统计每个元素出现次数
来源：http://hz.zycfv.cn/gtunxvpqpj.html

Py:   Counter(arr)
来源：http://hz.jinqigfzy.top/gtajgxdcha.html

PHP:  array_count_values($arr);
来源：http://hz.jinyuanbaomall.cn/gtloyrhfot.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.andypj.xyz/gtdojhhyzg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guowangkeji.top/gtsusxvjmt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cdnleiting.top/gtgnezazru.html

Go:   // 手写 map[T]int
来源：http://hz.feifeiyinyue.top/gththjggzx.html

Ruby: arr.tally
来源：http://hz.dianchejie.cn/gtfsjpqafx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.kuanghao11.cn/gtvknzoeza.html

[D21] 判断是否包含某元素
来源：http://hz.cqqwz.cn/gtgpgomxcp.html

Py:   x in arr
来源：http://hz.316326.xyz/gteqlilxeo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ydzc1.top/gtjptaxfan.html

JS:   arr.includes(x)
来源：http://hz.sweek.top/gteynqdfbi.html

TS:   arr.includes(x)
来源：http://hz.haohaochexian.top/gtrhpnjknb.html

Java: list.contains(x)
来源：http://hz.jyoumei.cn/gtcjzjeteu.html

Go:   slices.Contains(arr, x)
来源：http://hz.shzxlz.cn/gtrsaauygr.html

Ruby: arr.include?(x)
来源：http://hz.yj20258888.top/gtwbgqhkzt.html

C#:   list.Contains(x)
来源：http://hz.aibaodan.cn/gtekhzooqj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.svipenyu.cn/gtzrusehyn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xziqi.cn/gtkjzfqteu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.birdmap.top/gtsnjdjrkn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.316326.xyz/gtzcsnqpov.html

TS:   [...arr];
来源：http://hz.sysykeji.top/gtreaxkenb.html

Java: new ArrayList<>(list);
来源：http://hz.hnxiangtu.top/gtdhvrnhos.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nanxinkj.top/gtwoqiynqb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.0kj1m.cn/gtwxoymgcs.html

C#:   new List<int>(list);
来源：http://hz.dianchejie.cn/gthvlolfbc.html

[D23] reduce 累积计算
来源：http://hz.nanxinkj.top/gtxobrxdpx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jyoumei.cn/gtvkycfezt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.chenzaomai.com/gtqxdxlorj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gotoacloud.top/gtojngzdjq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cashguo.top/gtvbkmgrdj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.snrcjt.cn/gthaszirdx.html

Go:   // 手写循环
来源：http://hz.mhx1999.top/gtnicgmdlu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cdnleiting.top/gtzymgdmai.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xylfe.cn/gtpqojfhyg.html

[D24] 字典 / Map 基本操作
来源：http://hz.birdmap.top/gtsqzzphzz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhiwuduotai.top/gtayvzkqbn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yuxming.cn/gtamjloocf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.daxiang520.top/gteaqbvdzt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hfpthk.cn/gterjyoach.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.andypj.xyz/gttslzoqgs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yvedp.cn/gtgntnnwfz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.aizwys.cn/gtzpujadxg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinyuanbaomall.cn/gtkkuuoote.html

[D25] Set 集合去重与交并差
来源：http://hz.hywenlv.cn/gtshqjyggq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yueranfly.top/gtejsfaxyi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhiwuduotai.top/gtfvplkloc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hongshengwenyu.top/gtlrpyevgp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.316326.xyz/gtclkmavls.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.tian-w.cn/gtiwzifyxx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xinyue.icu/gtbhstkyig.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jianghu66.top/gtzihzzrnd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.nwbrower.top/gtuxjgnuzv.html

[D26] 数组转字符串
来源：http://hz.nwbrower.top/gtycflqmdc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xylfe.cn/gtyjdcmaky.html

PHP:  implode(", ", $arr);
来源：http://hz.sweek.top/gtvhpembyp.html

JS:   arr.join(", ")
来源：http://hz.jinyuanbaomall.cn/gtcbungyln.html

TS:   arr.join(", ")
来源：http://hz.ppjwa.cn/gtfhzzofxj.html

Java: String.join(", ", list)
来源：http://hz.hywenlv.cn/gtwqswhbej.html

Go:   strings.Join(strs, ", ")
来源：http://hz.dianchejie.cn/gtdbsjyvub.html

Ruby: arr.join(", ")
来源：http://hz.jinghuilouyu.cn/gtefscbzmd.html

C#:   string.Join(", ", list)
来源：http://hz.0kj1m.cn/gthudidatp.html

================================================================================
来源：http://hz.52xcode.cn/gtkqqtynub.html

E. 字符串处理
来源：http://hz.andypj.xyz/gtvdjvamjg.html

================================================================================
来源：http://hz.c1oappe.top/gtcrgantph.html

[E01] 拼接字符串
来源：http://hz.hongshengwenyu.top/gtvqwwuzzw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.kuanghao11.cn/gtpqsdxnqk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shanyushiyangkeji.top/gtfswwkoyp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.vqdsnc.cn/gtgzpqxaup.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fzhhl.top/gtyahvwjgh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.feifeiyinyue.top/gtoaaliyzr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zycfv.cn/gtdwwlrbhv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jlsjyb.cn/gtphsayezg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.mhx1999.top/gtsiurixiv.html

[E02] 重复字符串
来源：http://hz.gotoacloud.top/gtgtzzcqbv.html

Py:   "ab" * 3
来源：http://hz.yuanzhike.top/gtcmbzhhsa.html

PHP:  str_repeat("ab", 3);
来源：http://hz.andypj.xyz/gtbcgfkaqd.html

JS:   "ab".repeat(3)
来源：http://hz.yuanzhike.top/gthplnuymw.html

TS:   "ab".repeat(3)
来源：http://hz.zhaomingkeji.xyz/gtupzmkbbv.html

Java: "ab".repeat(3)
来源：http://hz.smart0.xyz/gtroesycmt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hywenlv.cn/gtticthlfp.html

Ruby: "ab" * 3
来源：http://hz.pycfn.com/gtixbsmyjm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenzaomai.com/gtvczfznng.html

[E03] 截取子串
来源：http://hz.yuxming.cn/gtlvmajzud.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.shanyushiyangkeji.top/gtxjcbhtam.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.guowangkeji.top/gttkfqioih.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xingfuxueyuan.xyz/gtzzwzxyfc.html

TS:   s.slice(1, 4)
来源：http://hz.shanyushiyangkeji.top/gtdrmrwvdw.html

Java: s.substring(1, 4)
来源：http://hz.nwbrower.top/gtrubvhpva.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.guowangkeji.top/gtfogqsbzm.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.bjfxy.top/gtzroysdwo.html

C#:   s.Substring(1, 3)
来源：http://hz.jinghuilouyu.cn/gtuyhappyy.html

[E04] 查找子串位置
来源：http://hz.gotoacloud.top/gtqzmrysyx.html

Py:   s.find("x");  s.index("x")
来源：http://hz.redwolf501.top/gtxmehbihq.html

PHP:  strpos($s, "x");
来源：http://hz.hywenlv.cn/gtbuxzyxnx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hywenlv.cn/gtqasbqzua.html

TS:   s.indexOf("x")
来源：http://hz.jyoumei.cn/gtxbxgxnog.html

Java: s.indexOf("x")
来源：http://hz.yj20258.top/gtcqxlocyj.html

Go:   strings.Index(s, "x")
来源：http://hz.yangfankeji.com/gtdjezqhdf.html

Ruby: s.index("x")
来源：http://hz.jlsjyb.cn/gtppndqwzb.html

C#:   s.IndexOf("x")
来源：http://hz.haohaochexian.top/gttrhnwtda.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jqgfzy.top/gtykdqsdqc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.52xcode.cn/gtrpwnregj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.cdnleiting.top/gtrfafwjnl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xinyue.icu/gtmfbxrxak.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xuanzx.com/gtdulyogdk.html


<!-- 参考信息 -->