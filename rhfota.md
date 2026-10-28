代发 wailian999

Ruby: a, b = pair
来源：http://hz.yuxming.cn/gtacophzjx.html

C#:   var (a, b) = pair;
来源：http://hz.nanxinkj.top/gtcofzjcxd.html

[C16] 函数 / 方法重载
来源：http://hz.xinyue.icu/gtxhcyouow.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.aizwys.cn/gtezkouhlt.html

PHP:  // 无重载
来源：http://hz.zhengqikj.top/gtwmcyflrn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.316326.xyz/gtubftavfe.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.birdmap.top/gtduaomeqd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenzaomai.com/gtejpvlste.html

Go:   // 无重载：用不同函数名
来源：http://hz.jiagoushi.top/gtagagymjm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.mhx1999.top/gtyqxbxedm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hongshengwenyu.top/gtmenizcqk.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtfveboakm.html

D. 数组 / 列表 / 集合
来源：http://hz.jinqigfzy.top/gtdhsholas.html

================================================================================
来源：http://hz.redwolf501.top/gtprfitjkm.html

[D01] 创建数组 / 列表
来源：http://hz.hongshengwenyu.top/gtmfeqkutt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenlongwang.top/gtzlqvrhxu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yuxming.cn/gtwqimrywk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jlsjyb.cn/gtnyidvelk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.redwolf501.top/gtjfkxqanw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yuxming.cn/gtkfubcaon.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zdqjudy.top/gtqomalbdf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhiwuduotai.top/gthyfbswad.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yvedp.cn/gtvpfhrixd.html

[D02] 追加元素到末尾
来源：http://hz.snrcjt.cn/gtzjthxmfk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cashguo.top/gtlsjsqomv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhixingplan.top/gtuouwawjg.html

JS:   arr.push(4);
来源：http://hz.xuetiantiany.cn/gtoebedcqd.html

TS:   arr.push(4);
来源：http://hz.tianlin.xyz/gtyxjviyqq.html

Java: list.add(4);
来源：http://hz.feifeiyinyue.top/gtjdsmldxe.html

Go:   arr = append(arr, 4)
来源：http://hz.fengsongda.top/gtnizchvmt.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jianghu66.top/gtwpbryopn.html

C#:   list.Add(4);
来源：http://hz.ywan-chungtsiang.top/gtdibygrce.html

[D03] 在指定位置插入元素
来源：http://hz.bjfxy.top/gtrymhxijn.html

Py:   arr.insert(0, 0)
来源：http://hz.cdnleiting.top/gtlpnhyrqo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cashguo.top/gtdrsfxwfg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhijiandao.cn/gtxpwcveiw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinyuanbaomall.cn/gtdsorncmv.html

Java: list.add(0, 0);
来源：http://hz.redwolf501.top/gtfgnbckbv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.aizwys.cn/gtknrphxat.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.meibo888.top/gtriqjuihy.html

C#:   list.Insert(0, 0);
来源：http://hz.redwolf501.top/gtyexmoqbw.html

[D04] 删除元素
来源：http://hz.guowangkeji.top/gtrjyofhjm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xinyue.icu/gtfbuyiibm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cheryme.top/gtawykkezt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jianghu66.top/gtyzedmdsg.html

TS:   arr.splice(0, 1);
来源：http://hz.pengpengdd.cyou/gtukqwkmjx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yuanzhike.top/gttfwwavur.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhongyouzk.top/gtqlvasvuo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xuanzx.com/gtquhwhwkf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.guowangkeji.top/gtmjexuoww.html

[D05] 访问与修改元素
来源：http://hz.zhiwuduotai.top/gtvnutzdwc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.kuanghao11.cn/gtskbjhphm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.mhx1999.top/gtzegnjnfd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.nanxuanxn.top/gtqrakmuxq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jqgufenzy.top/gthcjbqdfw.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jlsjyb.cn/gtkubwiihb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ydjk.org.cn/gtaxvvxsnl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.birdmap.top/gtunsiycnf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangshuangyany.cn/gtulytpolj.html

[D06] 数组长度
来源：http://hz.sweek.top/gtjfrgbvpd.html

Py:   len(arr)
来源：http://hz.aizwys.cn/gtvemttcyr.html

PHP:  count($arr);
来源：http://hz.yj20258888.top/gtghzfdidd.html

JS:   arr.length
来源：http://hz.mhx1999.top/gtuyizfmra.html

TS:   arr.length
来源：http://hz.chenzaomai.com/gthzsfwlhk.html

Java: list.size();
来源：http://hz.fengsongda.top/gtiixswlkj.html

Go:   len(arr)
来源：http://hz.hnqzz.top/gtgtjtsxjs.html

Ruby: arr.length; arr.size
来源：http://hz.jianghu66.top/gtwsihbxta.html

C#:   list.Count;
来源：http://hz.sweek.top/gtrukxygqp.html

[D07] 切片 / 取子数组
来源：http://hz.jianghu66.top/gtpvqbkrpi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.wangshuangyany.cn/gtyksqqcnm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.dianchejie.cn/gtrnrudgxm.html

JS:   arr.slice(1, 4);
来源：http://hz.nanxuanxn.top/gtgvrokcbn.html

TS:   arr.slice(1, 4);
来源：http://hz.tian-w.cn/gtffblgeaq.html

Java: list.subList(1, 4);
来源：http://hz.nanxinkj.top/gtqqehnatf.html

Go:   arr[1:4]
来源：http://hz.andypj.xyz/gtfcmxcevv.html

Ruby: arr[1, 3]
来源：http://hz.sysykeji.top/gttudxmnzr.html

C#:   list.GetRange(1, 3);
来源：http://hz.vqdsnc.cn/gtwzqqgawc.html

[D08] 合并两个数组
来源：http://hz.daxiang520.top/gthdutvxzu.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhixingplan.top/gtmyvyyipr.html

PHP:  array_merge($a, $b);
来源：http://hz.xinyue.icu/gtnbfhffws.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.c1oappe.top/gtfbvsxnqg.html

TS:   [...a, ...b];
来源：http://hz.yuxming.cn/gtzlgdxfnj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yonumen.top/gtnlysajsx.html

Go:   append(a, b...)
来源：http://hz.feifeiyinyue.top/gtftlcnqjy.html

Ruby: a + b;  a.concat(b)
来源：http://hz.dianchejie.cn/gthklktodj.html

C#:   a.Concat(b).ToList()
来源：http://hz.guannengcc.top/gtwdftjxzi.html

[D09] 排序（升序）
来源：http://hz.nwbrower.top/gtmmbltrla.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shuidangran.top/gtdeswinhc.html

PHP:  sort($arr);
来源：http://hz.xylfe.cn/gtmsllvgsj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hysaishi.cn/gtenwlyfkn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shuidangran.top/gtihtliilr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.fzhhl.top/gtocltfirg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.chenjidiqi.icu/gtzijitiyl.html

Ruby: arr.sort
来源：http://hz.nanxinkj.top/gtxstjfifl.html

C#:   list.Sort();
来源：http://hz.jyoumei.cn/gtvhtlqwus.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gotoacloud.top/gttlcfrybj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gotoacloud.top/gtmfltbooz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cucudq.cn/gtsvlipuul.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.meibo888.top/gtxtilibjv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xylfe.cn/gthhixihpn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sweek.top/gtixbciput.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.daxiang520.top/gtytmjzbpr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhijiandao.cn/gtuvqdijgc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hongshengwenyu.top/gttybwfvgn.html

[D11] 反转数组
来源：http://hz.guowangkeji.top/gtemprjsio.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xziqi.cn/gtgfpminbr.html

PHP:  array_reverse($arr);
来源：http://hz.hysaishi.cn/gtnmpmflfn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.chenzaomai.com/gttpycdzjg.html

TS:   [...arr].reverse();
来源：http://hz.c1oappe.top/gtkuieufhi.html

Java: Collections.reverse(list);
来源：http://hz.sysykeji.top/gtgouezrnc.html

Go:   slices.Reverse(arr)
来源：http://hz.yj20258.top/gtptyterhn.html

Ruby: arr.reverse
来源：http://hz.zdqjudy.top/gtnfkhnnrv.html

C#:   list.Reverse();
来源：http://hz.hywenlv.cn/gtfkxzncvg.html

[D12] 查找元素下标
来源：http://hz.daxiang520.top/gtkuttypcc.html

Py:   arr.index(x);  x in arr
来源：http://hz.jianghu66.top/gtjxnovtss.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.feifeiyinyue.top/gtozonmrfc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhijiandao.cn/gtvqxsihsy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangtech.top/gtrlzfyysr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinyuanbaomall.cn/gtwakdsjfo.html

Go:   slices.Index(arr, x)
来源：http://hz.zhongyouzk.top/gtehrqpgrd.html

Ruby: arr.index(x)
来源：http://hz.ehwqpu.com/gtooiuymjp.html

C#:   list.IndexOf(x);
来源：http://hz.tianlin.xyz/gtzuidmyyr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cucudq.cn/gtrbjpqaqn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenzaomai.com/gtxbqpieuq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhengqikj.top/gtftrtbsco.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xylfe.cn/gtjyjqsnwb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinyuanbaomall.cn/gtyqqcpcpe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hysaishi.cn/gtwjlvnbts.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhongyouzk.top/gttsdapali.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.vqdsnc.cn/gtrzitwtjw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cashguo.top/gttyiypbkz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhixingplan.top/gtapwwhwaf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sysykeji.top/gtgwfagzpi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jqgfzy.top/gtkecsyeqm.html

JS:   arr.map(x => x * 2)
来源：http://hz.mhx1999.top/gtwrcxdlxw.html

TS:   arr.map(x => x * 2)
来源：http://hz.hammf.cn/gthqscuqto.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yanxiufei.cn/gtwfovbtra.html

Go:   // 手写循环
来源：http://hz.yanxiufei.cn/gteaoxhria.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.birdmap.top/gtwgeacopr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.aizwys.cn/gtknjdeaiv.html

[D15] 去重
来源：http://hz.yj20258.top/gtxqgifdns.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yj20258888.top/gtfrqqbauf.html

PHP:  array_unique($arr);
来源：http://hz.yangfankeji.com/gtbrerasrn.html

JS:   [...new Set(arr)]
来源：http://hz.wangdashe.top/gtksxmamjp.html

TS:   [...new Set(arr)]
来源：http://hz.jqgfzy.top/gtizsonues.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhengqikj.top/gtycsgotbh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhongyouzk.top/gtxtnsyqar.html

Ruby: arr.uniq
来源：http://hz.nanxuanxn.top/gtwgdhdlpp.html

C#:   list.Distinct().ToList()
来源：http://hz.kuanghao11.cn/gtcusgoaby.html

[D16] 求和与平均值
来源：http://hz.gotoacloud.top/gtfqgbeiif.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenjidiqi.icu/gtaqkuzfnz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shangyingyoupin.top/gtfadqadff.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangshuangyany.cn/gtkprsqvqe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aizwys.cn/gtjmcbxufp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.chenjidiqi.icu/gtugpgwejl.html

Go:   // 手写循环累加
来源：http://hz.chenjidiqi.icu/gtivmwzcsu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jiagoushi.top/gtwzbxkxnj.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinqigufen.top/gtobgtugpe.html

[D17] 最大值与最小值
来源：http://hz.zycfv.cn/gtzjlgsiyo.html

Py:   max(arr);  min(arr)
来源：http://hz.xylfe.cn/gtcflcnejl.html

PHP:  max($arr);  min($arr);
来源：http://hz.zdqjudy.top/gtoumrwtfd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dashuyun.cn/gtcxjhojmm.html

TS:   Math.max(...arr);
来源：http://hz.pengpengdd.cyou/gtquotjuca.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xingfuxueyuan.xyz/gtqmsloiie.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhixingplan.top/gtcbhmonxl.html

Ruby: arr.max;  arr.min
来源：http://hz.c1oappe.top/gtbyfvmfkx.html

C#:   list.Max();  list.Min()
来源：http://hz.ydzc1.top/gtzfptesue.html

[D18] 扁平化嵌套数组
来源：http://hz.yuanzhike.top/gtyepneixv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.redwolf501.top/gtcfqjuwng.html

PHP:  array_merge(...$nested);
来源：http://hz.yvedp.cn/gtwifbekuz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xziqi.cn/gtmnoowqvn.html

TS:   nested.flat();
来源：http://hz.zdqjudy.top/gtubokjego.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.316326.xyz/gtxfzejvxd.html

Go:   // 手写双层循环
来源：http://hz.tanke756.top/gtxxpwexkj.html

Ruby: nested.flatten
来源：http://hz.sysykeji.top/gtkifcqmww.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.aizwys.cn/gtqxegsjvo.html

[D19] 按字段分组
来源：http://hz.mhx1999.top/gtobmxnbts.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jianghu66.top/gtuybsbfhw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xinyue.icu/gtzfmkcezu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.nanxuanxn.top/gtbmxbmzbe.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.birdmap.top/gtikioisee.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ybcxt.top/gtynnigtdi.html

Go:   // 手写 map[string][]T
来源：http://hz.hammf.cn/gtpgnsonqi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.daria6918.cn/gtuvaftyzh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhoulong.xyz/gtlxaokhqc.html

[D20] 统计每个元素出现次数
来源：http://hz.0kj1m.cn/gtbxzceihe.html

Py:   Counter(arr)
来源：http://hz.ivvv.top/gtjgnaafro.html

PHP:  array_count_values($arr);
来源：http://hz.ywan-chungtsiang.top/gtdkxihuyx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jlsjyb.cn/gtkbetwmgw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hfpthk.cn/gtzlzryzmt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinqigfzy.top/gtutldrmhw.html

Go:   // 手写 map[T]int
来源：http://hz.zdqjudy.top/gtqocdyuzh.html

Ruby: arr.tally
来源：http://hz.iojbl.cn/gtsdvgruua.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.haohaochexian.top/gtxsulfwmf.html

[D21] 判断是否包含某元素
来源：http://hz.aizwys.cn/gtljzubfyz.html

Py:   x in arr
来源：http://hz.yuxming.cn/gtcecbwtaa.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhaomingkeji.xyz/gtuvsbtivr.html

JS:   arr.includes(x)
来源：http://hz.52xcode.cn/gtglwmkohc.html

TS:   arr.includes(x)
来源：http://hz.tanke756.top/gtyhojefhu.html

Java: list.contains(x)
来源：http://hz.ehwqpu.com/gtezmieujt.html

Go:   slices.Contains(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtnhdgzjdh.html

Ruby: arr.include?(x)
来源：http://hz.xylfe.cn/gtqvwojlyd.html

C#:   list.Contains(x)
来源：http://hz.xingfuxueyuan.xyz/gtuppxmwjk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.pycfn.com/gtwzlahepa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hammf.cn/gtrlnghgnv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tianlin.xyz/gtpnexyedl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.vqdsnc.cn/gtqiwuipzk.html

TS:   [...arr];
来源：http://hz.cucudq.cn/gtotvecjau.html

Java: new ArrayList<>(list);
来源：http://hz.fzhhl.top/gtrbzhuorr.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ydjk.org.cn/gtbwbbnsax.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhoulong.xyz/gtibnrirca.html

C#:   new List<int>(list);
来源：http://hz.hongshengwenyu.top/gtncjkuxsk.html

[D23] reduce 累积计算
来源：http://hz.havefunace.top/gtdtaovfep.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj202588.top/gtymhqtchi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.iojbl.cn/gtoohvfxqp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.smart0.xyz/gtgfztlazp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ybcxt.top/gtxtzwfvap.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yangfankeji.com/gtmzryhvok.html

Go:   // 手写循环
来源：http://hz.wangshuangyany.cn/gtnuyjjegf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hysaishi.cn/gthogywyku.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tianlin.xyz/gtalxjahxr.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj202588.top/gtrvihbnyv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.cqqwz.cn/gtsqmyljkb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xingfuxueyuan.xyz/gthlluyouj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.bjfxy.top/gtgryavbyi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hnxiangtu.top/gthmstiftu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ybcxt.top/gtvpjulupu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nanxinkj.top/gticdvjiug.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cashguo.top/gtyxpxiyoc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.9152youxi.cn/gtiiextbmk.html

[D25] Set 集合去重与交并差
来源：http://hz.c1oappe.top/gtezrbdcdi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.tian-w.cn/gtflvjaems.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.sufxvd.cn/gtkgoaxvlt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hnxiangtu.top/gtlccxbcik.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.mhx1999.top/gtjbozrqrk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinyuanbaomall.cn/gtdfvwvzhv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinqigufen.top/gtntspploo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yongpay.top/gtmxdysscu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.wangdashe.top/gtldvzuhhv.html

[D26] 数组转字符串
来源：http://hz.dashuyun.cn/gtpuqwhjve.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xinyue.icu/gtxdwxgode.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgfzy.top/gtslxjeshu.html

JS:   arr.join(", ")
来源：http://hz.shuidangran.top/gtmhczsawu.html

TS:   arr.join(", ")
来源：http://hz.birdmap.top/gtrzzsnwjy.html

Java: String.join(", ", list)
来源：http://hz.zhoulong.xyz/gtqibrsfmr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj20258888.top/gtabhmwxow.html

Ruby: arr.join(", ")
来源：http://hz.jyoumei.cn/gtmdivuwcq.html

C#:   string.Join(", ", list)
来源：http://hz.yongpay.top/gtzqoxoapt.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtwijbhnea.html

E. 字符串处理
来源：http://hz.yangfankeji.com/gtojlimvkl.html

================================================================================
来源：http://hz.yangfankeji.com/gtzoijcyrp.html

[E01] 拼接字符串
来源：http://hz.chenlongwang.top/gtojzdtnmz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xziqi.cn/gtrzmhuqnh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yvedp.cn/gtpxppglnb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gttnnxakym.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhixingplan.top/gtdrvbdywd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ppjwa.cn/gtaskblrlp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gaohongyu789.top/gthyhzgonk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yuanzhike.top/gtmapapqwe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jqgufenzy.top/gtpgemltjw.html

[E02] 重复字符串
来源：http://hz.shangyingyoupin.top/gtoognjklh.html

Py:   "ab" * 3
来源：http://hz.hnxiangtu.top/gtrmsmiszt.html

PHP:  str_repeat("ab", 3);
来源：http://hz.daxiang520.top/gtyaddgkkv.html

JS:   "ab".repeat(3)
来源：http://hz.yj202588.top/gtmfngafnf.html

TS:   "ab".repeat(3)
来源：http://hz.tanke756.top/gtdhfvfvek.html

Java: "ab".repeat(3)
来源：http://hz.dashuyun.cn/gtdzfcbdak.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.wangshuangyany.cn/gtfxvnoxnq.html

Ruby: "ab" * 3
来源：http://hz.gaohongyu789.top/gtycxpkktc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.mhx1999.top/gtgmjleaqt.html

[E03] 截取子串
来源：http://hz.quarkkingdee.top/gtwdigwytk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.daxiang520.top/gtcyvbtagg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jyoumei.cn/gtecpwkdoa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhijiandao.cn/gtfhuhnxpq.html

TS:   s.slice(1, 4)
来源：http://hz.zhiwuduotai.top/gtzyrdvssk.html

Java: s.substring(1, 4)
来源：http://hz.yuanzhike.top/gtickfbyeq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.shzxlz.cn/gtlnjfrivd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zycfv.cn/gtysuasmlx.html

C#:   s.Substring(1, 3)
来源：http://hz.cashguo.top/gtntdjslon.html

[E04] 查找子串位置
来源：http://hz.ywan-chungtsiang.top/gttdecqvgn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jlsjyb.cn/gtcygwpkde.html

PHP:  strpos($s, "x");
来源：http://hz.yongpay.top/gtdleskuwf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yongpay.top/gtripnaeop.html

TS:   s.indexOf("x")
来源：http://hz.pycfn.com/gtdujsnnmp.html

Java: s.indexOf("x")
来源：http://hz.jlsjyb.cn/gtzdasuokf.html

Go:   strings.Index(s, "x")
来源：http://hz.xinyue.icu/gtpvyjcbof.html

Ruby: s.index("x")
来源：http://hz.jinghuilouyu.cn/gthgxiwodf.html

C#:   s.IndexOf("x")
来源：http://hz.birdmap.top/gtjpiallaf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hongshengwenyu.top/gtmytdrxwu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hnqzz.top/gtyfownaez.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gzhubu.top/gtmazsespu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sweek.top/gtkciiqwrc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.mhx1999.top/gtscxhmuph.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.52xcode.cn/gtsubvcrlm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zycfv.cn/gtgkgbywyj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.0kj1m.cn/gtcqqtcokr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.chenjidiqi.icu/gtnwepmhga.html

[E06] 替换子串
来源：http://hz.hnxiangtu.top/gtqrjrtkzr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xuetiantiany.cn/gtlgwdgcmf.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.pycfn.com/gttoyvniqt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtffkfexxv.html


<!-- 参考信息 -->