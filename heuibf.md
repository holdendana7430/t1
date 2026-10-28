代发 wailian999

PHP:  // 无重载
来源：http://hz.jianghu66.top/gtcuhizrfq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cheryme.top/gtghvqoout.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.0kj1m.cn/gtgculzwnz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cashguo.top/gtoftodfyx.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhijiandao.cn/gtjobhgibe.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ybcxt.top/gtilavbfzf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cucudq.cn/gtwnwpvwzw.html

================================================================================
来源：http://hz.shuidangran.top/gtykkqiils.html

D. 数组 / 列表 / 集合
来源：http://hz.cheryme.top/gtdvqiacty.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtnmtalkql.html

[D01] 创建数组 / 列表
来源：http://hz.xuanzx.com/gtvjdpzudn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.redwolf501.top/gthoybmqvf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yuanzhike.top/gtqbdsgfib.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xziqi.cn/gtubnvtzng.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zycfv.cn/gtgaxnhkxu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhaomingkeji.xyz/gtbgwiaetv.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.daria6918.cn/gtaelefqvg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhijiandao.cn/gtjurqrcjn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.daxiang520.top/gtwgpaihgh.html

[D02] 追加元素到末尾
来源：http://hz.aibaodan.cn/gtjozfxcif.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.aizwys.cn/gtetfaczlb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.aibaodan.cn/gtkusejgrl.html

JS:   arr.push(4);
来源：http://hz.zycfv.cn/gtswivqnkr.html

TS:   arr.push(4);
来源：http://hz.aibaodan.cn/gtmcpsybhg.html

Java: list.add(4);
来源：http://hz.yj20258.top/gtiueggdwl.html

Go:   arr = append(arr, 4)
来源：http://hz.yuanzhike.top/gtximuvnds.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ivvv.top/gtqgagxulq.html

C#:   list.Add(4);
来源：http://hz.hammf.cn/gtalwxgiso.html

[D03] 在指定位置插入元素
来源：http://hz.yj20258888.top/gtfjuxlrdb.html

Py:   arr.insert(0, 0)
来源：http://hz.0kj1m.cn/gtrdgoayrn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gzhubu.top/gtfearcvbm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhongyouzk.top/gtbatckyvq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.mhx1999.top/gtaxbnrfkq.html

Java: list.add(0, 0);
来源：http://hz.52xcode.cn/gtzwbvriwr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.andypj.xyz/gtiixbxxjo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydzc1.top/gtaxnpcgkb.html

C#:   list.Insert(0, 0);
来源：http://hz.vqdsnc.cn/gtezdckmyc.html

[D04] 删除元素
来源：http://hz.yangfankeji.com/gtwxtgljia.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhoulong.xyz/gtrxnzisti.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yangfankeji.com/gtgacqmhcp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.tian-w.cn/gtnnzmatsf.html

TS:   arr.splice(0, 1);
来源：http://hz.zhixingplan.top/gtkkvqavrg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jiagoushi.top/gtujkeorti.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.wangshuangyany.cn/gtnsjxdnlx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yanxiufei.cn/gtgigcrpge.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.tianlin.xyz/gtnnigynbi.html

[D05] 访问与修改元素
来源：http://hz.gogol.net.cn/gtuoseshfk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sxryk.cn/gtgegkwqgl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jianghu66.top/gtikpqxshk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhoulong.xyz/gtajmxfzrv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.birdmap.top/gtkggzaysg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.pycfn.com/gtswnrfmyt.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gteqdvcmtl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jqgufenzy.top/gtgihkkyqb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.birdmap.top/gtblbeuyvh.html

[D06] 数组长度
来源：http://hz.dianchejie.cn/gtqskebytm.html

Py:   len(arr)
来源：http://hz.kuanghao11.cn/gtirrtkvsw.html

PHP:  count($arr);
来源：http://hz.yangfankeji.com/gttmcaerqp.html

JS:   arr.length
来源：http://hz.andypj.xyz/gthkembnmt.html

TS:   arr.length
来源：http://hz.cqqwz.cn/gtayowxhnf.html

Java: list.size();
来源：http://hz.sxryk.cn/gttuyrzdka.html

Go:   len(arr)
来源：http://hz.havefunace.top/gtqswkxiso.html

Ruby: arr.length; arr.size
来源：http://hz.shangyingyoupin.top/gtlkbefita.html

C#:   list.Count;
来源：http://hz.cqqwz.cn/gthqdqdriz.html

[D07] 切片 / 取子数组
来源：http://hz.cqqwz.cn/gtgdxajmje.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.meibo888.top/gtzqnbovxz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhaomingkeji.xyz/gtvctqfpsl.html

JS:   arr.slice(1, 4);
来源：http://hz.xinyue.icu/gtnggtwywa.html

TS:   arr.slice(1, 4);
来源：http://hz.sysykeji.top/gtwanbuxvt.html

Java: list.subList(1, 4);
来源：http://hz.fzhhl.top/gtaitnfizd.html

Go:   arr[1:4]
来源：http://hz.kuanghao11.cn/gtlvjrtolp.html

Ruby: arr[1, 3]
来源：http://hz.cucudq.cn/gtemotgqay.html

C#:   list.GetRange(1, 3);
来源：http://hz.haohaochexian.top/gthuinogcz.html

[D08] 合并两个数组
来源：http://hz.wangshuangyany.cn/gtrqzymfld.html

Py:   a + b;  a.extend(b)
来源：http://hz.ydzc1.top/gtqmlslhvb.html

PHP:  array_merge($a, $b);
来源：http://hz.gaohongyu789.top/gtcvunyzfz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yonumen.top/gtzqzkairl.html

TS:   [...a, ...b];
来源：http://hz.yj20258.top/gtwprbbleh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.daria6918.cn/gtsrkvzcnu.html

Go:   append(a, b...)
来源：http://hz.kuanghao11.cn/gtprninmhd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shuidangran.top/gtmcujjunh.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinyuanbaomall.cn/gttdsyxecd.html

[D09] 排序（升序）
来源：http://hz.birdmap.top/gtjipldoxc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtykgicwop.html

PHP:  sort($arr);
来源：http://hz.zhongyouzk.top/gtocbrwnnr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gzhubu.top/gtifqgvoth.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhoulong.xyz/gtdblwckmq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.aibaodan.cn/gtqdasamks.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhoulong.xyz/gtinrgunsg.html

Ruby: arr.sort
来源：http://hz.shanyushiyangtech.top/gtgiplaowp.html

C#:   list.Sort();
来源：http://hz.snrcjt.cn/gtxcwhwzfw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.nwbrower.top/gthvixjxme.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.daria6918.cn/gtedwwcpwo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fengsongda.top/gtupflpbkn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.9152youxi.cn/gtyzvifndf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnqzz.top/gtfpgrtpsb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhaomingkeji.xyz/gtzthkqswo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gogol.net.cn/gtbrbuccit.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cdnleiting.top/gtfbvkczkz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenjidiqi.icu/gttszuzsio.html

[D11] 反转数组
来源：http://hz.jinyuanbaomall.cn/gtmwbiosni.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ivvv.top/gtlbhvopze.html

PHP:  array_reverse($arr);
来源：http://hz.tanke756.top/gtwnktfumx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yj202588.top/gtdhgendzj.html

TS:   [...arr].reverse();
来源：http://hz.ydjk.org.cn/gtcrwcjyma.html

Java: Collections.reverse(list);
来源：http://hz.redwolf501.top/gtbyixuucf.html

Go:   slices.Reverse(arr)
来源：http://hz.dashuyun.cn/gtrawotzkb.html

Ruby: arr.reverse
来源：http://hz.jqgufenzy.top/gtahukbawn.html

C#:   list.Reverse();
来源：http://hz.kuanghao11.cn/gtqxxumuxe.html

[D12] 查找元素下标
来源：http://hz.ybcxt.top/gtgugivgqn.html

Py:   arr.index(x);  x in arr
来源：http://hz.hnqzz.top/gttojaaame.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinghuilouyu.cn/gtotvxpqsm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shzxlz.cn/gtpecioklk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhongyouzk.top/gtpqlgzcbp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.andypj.xyz/gtjhnwyfge.html

Go:   slices.Index(arr, x)
来源：http://hz.zycfv.cn/gtiwipaope.html

Ruby: arr.index(x)
来源：http://hz.dianchejie.cn/gtpnotyqrj.html

C#:   list.IndexOf(x);
来源：http://hz.xylfe.cn/gtmdfujatn.html

[D13] 过滤（保留满足条件的）
来源：http://hz.wangshuangyany.cn/gtvvozvyfb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.daxiang520.top/gtbwlvqrkg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.wangdashe.top/gtbhsiqmhx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yvedp.cn/gtqwsnaote.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtdqtmxqae.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj20258888.top/gtecycgris.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yonumen.top/gtlrtdatgh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hnqzz.top/gtuvsnhrpp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.bjfxy.top/gtkxeitfkv.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tianlin.xyz/gtskvrdcjj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cashguo.top/gtlruirhrt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.iojbl.cn/gttyltijxo.html

JS:   arr.map(x => x * 2)
来源：http://hz.wangdashe.top/gtfwqogyrc.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhengqikj.top/gtrivvwmoy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.nwbrower.top/gtppfyofud.html

Go:   // 手写循环
来源：http://hz.ivvv.top/gtqgffjyel.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.meibo888.top/gtrhefmqmy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinyuanbaomall.cn/gtfwvkqrgn.html

[D15] 去重
来源：http://hz.fengsongda.top/gtcmtwabkc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gaohongyu789.top/gtnlsoqjny.html

PHP:  array_unique($arr);
来源：http://hz.fengsongda.top/gtgerfdbvi.html

JS:   [...new Set(arr)]
来源：http://hz.sufxvd.cn/gtewcgbmap.html

TS:   [...new Set(arr)]
来源：http://hz.gaohongyu789.top/gtuxljhwut.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hywenlv.cn/gtarcmgvlf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cashguo.top/gtzgtnwzzt.html

Ruby: arr.uniq
来源：http://hz.sufxvd.cn/gtgxxyrtul.html

C#:   list.Distinct().ToList()
来源：http://hz.yongpay.top/gtewoqgfrq.html

[D16] 求和与平均值
来源：http://hz.shzxlz.cn/gtixhsidjn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhixingplan.top/gteflbtibo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.haohaochexian.top/gtnwnxdxtb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtssyhulty.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daria6918.cn/gtarsqsqkh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hysaishi.cn/gtgfoyoqay.html

Go:   // 手写循环累加
来源：http://hz.nwbrower.top/gtzqbtyraj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.chenlongwang.top/gtiizmxtmn.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhixingplan.top/gthhifmyxv.html

[D17] 最大值与最小值
来源：http://hz.fzhhl.top/gtgzzrtmrp.html

Py:   max(arr);  min(arr)
来源：http://hz.aibaodan.cn/gtjyqyuvns.html

PHP:  max($arr);  min($arr);
来源：http://hz.ehwqpu.com/gtfesuvwnz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ydzc1.top/gtfeecqnuy.html

TS:   Math.max(...arr);
来源：http://hz.shangyingyoupin.top/gtmbhusgoz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.fzhhl.top/gtomkkpmey.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.daxiang520.top/gtqfapznvf.html

Ruby: arr.max;  arr.min
来源：http://hz.quarkkingdee.top/gtmpszenlo.html

C#:   list.Max();  list.Min()
来源：http://hz.havefunace.top/gtlqswddmc.html

[D18] 扁平化嵌套数组
来源：http://hz.jqgfzy.top/gtnckzqghz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ydjk.org.cn/gtkgbhpusi.html

PHP:  array_merge(...$nested);
来源：http://hz.haohaochexian.top/gtqgjzutgm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xingfuxueyuan.xyz/gthjidvozu.html

TS:   nested.flat();
来源：http://hz.cucudq.cn/gtqfldtixg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhoulong.xyz/gtmzhhbaqx.html

Go:   // 手写双层循环
来源：http://hz.zhengqikj.top/gtsghxizqz.html

Ruby: nested.flatten
来源：http://hz.iojbl.cn/gtiodrobhl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.0kj1m.cn/gtoperehyr.html

[D19] 按字段分组
来源：http://hz.hnqzz.top/gtdrktibbg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.feifeiyinyue.top/gtcypyilmd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhixingplan.top/gtiebrhfvm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jqgfzy.top/gtfawjeaez.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hongshengwenyu.top/gtqtaezbpg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shanyushiyangkeji.top/gtonuwgdwt.html

Go:   // 手写 map[string][]T
来源：http://hz.shanyushiyangtech.top/gtitnbwyyf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ywan-chungtsiang.top/gtjwvdxetv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhiwuduotai.top/gtdbheaxmw.html

[D20] 统计每个元素出现次数
来源：http://hz.snrcjt.cn/gtpcuxmaat.html

Py:   Counter(arr)
来源：http://hz.daria6918.cn/gtrkrpkijx.html

PHP:  array_count_values($arr);
来源：http://hz.jinghuilouyu.cn/gtafexncuo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xinyue.icu/gtopuvaovr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigfzy.top/gtmhnppgxv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sweek.top/gtcbtnaucl.html

Go:   // 手写 map[T]int
来源：http://hz.ivvv.top/gtuzoyuokg.html

Ruby: arr.tally
来源：http://hz.jqgfzy.top/gtkqtsidys.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.birdmap.top/gtxrjzxudq.html

[D21] 判断是否包含某元素
来源：http://hz.ivvv.top/gtuwekjmap.html

Py:   x in arr
来源：http://hz.hywenlv.cn/gtloypzbwo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gzhubu.top/gttfhagdfg.html

JS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtraqnowhk.html

TS:   arr.includes(x)
来源：http://hz.52xcode.cn/gtwyqalzkd.html

Java: list.contains(x)
来源：http://hz.hongshengwenyu.top/gtwbsvwamk.html

Go:   slices.Contains(arr, x)
来源：http://hz.xziqi.cn/gtdyaqhpwb.html

Ruby: arr.include?(x)
来源：http://hz.jiagoushi.top/gtlfxxwyks.html

C#:   list.Contains(x)
来源：http://hz.ehwqpu.com/gtxpnphyti.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gotoacloud.top/gtzqbvfrpp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hnqzz.top/gtkdmbqnoq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.vqdsnc.cn/gtyywnnipy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nanxuanxn.top/gtgluofqfm.html

TS:   [...arr];
来源：http://hz.52xcode.cn/gtacrdvyxn.html

Java: new ArrayList<>(list);
来源：http://hz.chenjidiqi.icu/gtxfrtiajq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhongyouzk.top/gtssuupzwy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.fzhhl.top/gtagvbgbno.html

C#:   new List<int>(list);
来源：http://hz.cashguo.top/gthpfzauxc.html

[D23] reduce 累积计算
来源：http://hz.kuanghao11.cn/gtmgwmddan.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.svipenyu.cn/gtlkkqxxwm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jqgufenzy.top/gtndqofuic.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zdqjudy.top/gtnazcpakf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tanke756.top/gtrodzpywe.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jyoumei.cn/gtwcspigxm.html

Go:   // 手写循环
来源：http://hz.chenlongwang.top/gtfleozpdd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.snrcjt.cn/gtygooancw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yueranfly.top/gtvpughctt.html

[D24] 字典 / Map 基本操作
来源：http://hz.shuidangran.top/gtanumuege.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yuanzhike.top/gtqzsglakc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hammf.cn/gtmmprxvhb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yanxiufei.cn/gtsrkpdkmy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xziqi.cn/gtzeiifijx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zdqjudy.top/gthzqriifb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.aibaodan.cn/gtqflbholk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.meibo888.top/gtqrkaxgtm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jiagoushi.top/gtcpetiwjd.html

[D25] Set 集合去重与交并差
来源：http://hz.daxiang520.top/gtipdyypso.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.chenlongwang.top/gtmrjciaze.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cheryme.top/gtdchqndlf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.dianchejie.cn/gtpzxnchyt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.wangdashe.top/gtemulzcrk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.fengsongda.top/gtauzgucui.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.guowangkeji.top/gtjsfeejfz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hongshengwenyu.top/gtwitqmzht.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.daria6918.cn/gtgsfnebcm.html

[D26] 数组转字符串
来源：http://hz.ppjwa.cn/gtaxspjjfa.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yj20258888.top/gtztzfqlvs.html

PHP:  implode(", ", $arr);
来源：http://hz.chenlongwang.top/gtlbvpsxmq.html

JS:   arr.join(", ")
来源：http://hz.wangdashe.top/gtjsvmwruf.html

TS:   arr.join(", ")
来源：http://hz.jinqigfzy.top/gtjoyiruxl.html

Java: String.join(", ", list)
来源：http://hz.chenzaomai.com/gtfrwnsccb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yangfankeji.com/gtbeyugdap.html

Ruby: arr.join(", ")
来源：http://hz.birdmap.top/gtzpiwlwhx.html

C#:   string.Join(", ", list)
来源：http://hz.yuanzhike.top/gtkoblnqow.html

================================================================================
来源：http://hz.tanke756.top/gtoxomylpl.html

E. 字符串处理
来源：http://hz.cucudq.cn/gtvdngfnmk.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtgryopunw.html

[E01] 拼接字符串
来源：http://hz.cucudq.cn/gtcirmnkrc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.bjfxy.top/gtadchznfz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ybcxt.top/gtkfqjsvcs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shuidangran.top/gtvdralbbg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.redwolf501.top/gtfavkydhr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.tanke756.top/gtwbccbxsk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.haohaochexian.top/gtmzvtvfxi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj20258888.top/gtnjodlwfv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhixingplan.top/gtirwjhkzl.html

[E02] 重复字符串
来源：http://hz.yj20258888.top/gtsmgpkurf.html

Py:   "ab" * 3
来源：http://hz.iojbl.cn/gttxsvhgpw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.redwolf501.top/gtmagqndjd.html

JS:   "ab".repeat(3)
来源：http://hz.shzxlz.cn/gtdwxzqxfp.html

TS:   "ab".repeat(3)
来源：http://hz.ydzc1.top/gtsdxemrld.html

Java: "ab".repeat(3)
来源：http://hz.zhengqikj.top/gtwqnajvgt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.vqdsnc.cn/gtxvjvzkbo.html

Ruby: "ab" * 3
来源：http://hz.zhijiandao.cn/gttfhdyyki.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.9152youxi.cn/gtlbhzensz.html

[E03] 截取子串
来源：http://hz.redwolf501.top/gtlmkvczgu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.wangdashe.top/gtfnidxvkm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hysaishi.cn/gtcyxlnhfb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xylfe.cn/gtomnqxvhy.html

TS:   s.slice(1, 4)
来源：http://hz.sxryk.cn/gtbwwnqwrn.html

Java: s.substring(1, 4)
来源：http://hz.jqgufenzy.top/gtqehazfvx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.nwbrower.top/gtowmmcfsb.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.tanke756.top/gtfxykqely.html

C#:   s.Substring(1, 3)
来源：http://hz.hysaishi.cn/gtskpzbsnr.html

[E04] 查找子串位置
来源：http://hz.sysykeji.top/gthmiwoooo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gzhubu.top/gtnhgyytce.html

PHP:  strpos($s, "x");
来源：http://hz.gotoacloud.top/gtuqfnekda.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shzxlz.cn/gtqzrondbt.html

TS:   s.indexOf("x")
来源：http://hz.cucudq.cn/gtkcwgstdx.html

Java: s.indexOf("x")
来源：http://hz.snrcjt.cn/gtkvrkikql.html

Go:   strings.Index(s, "x")
来源：http://hz.zhaomingkeji.xyz/gtfbkuiujz.html

Ruby: s.index("x")
来源：http://hz.c1oappe.top/gtxedffnox.html

C#:   s.IndexOf("x")
来源：http://hz.sweek.top/gtnogulwez.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hnxiangtu.top/gtioslllid.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.vqdsnc.cn/gtsyeurpbh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.guannengcc.top/gtdidtlryo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.wangshuangyany.cn/gtpdkyouys.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jqgfzy.top/gtnrkchjyv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhiwuduotai.top/gtfygxvjms.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ydzc1.top/gtsfytsxsl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yvedp.cn/gtlfwcxjbd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhaomingkeji.xyz/gtwrvwfzom.html

[E06] 替换子串
来源：http://hz.gotoacloud.top/gtxnxrmwns.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinyuanbaomall.cn/gtvblhguds.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hfpthk.cn/gtqgifelma.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gtjlhzangx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtkmwunmwm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtnbuseild.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ivvv.top/gtkhzjyalo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jqgufenzy.top/gtennczczg.html


<!-- 参考信息 -->