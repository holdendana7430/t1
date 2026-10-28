代发 wailian999

Ruby: a, b = pair
来源：http://hz.zhiwuduotai.top/gtkpgrofzj.html

C#:   var (a, b) = pair;
来源：http://hz.cqqwz.cn/gtaqupcrbm.html

[C16] 函数 / 方法重载
来源：http://hz.daxiang520.top/gtxovrgzap.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hammf.cn/gtleucnqje.html

PHP:  // 无重载
来源：http://hz.yongpay.top/gtmppcqmyu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yj202588.top/gtdmnomlzt.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hywenlv.cn/gtlvsmpdbk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yj202588.top/gtyfdtzwcx.html

Go:   // 无重载：用不同函数名
来源：http://hz.cucudq.cn/gtgtpsbrsx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gogol.net.cn/gthxxvzqib.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jyoumei.cn/gtutruantc.html

================================================================================
来源：http://hz.zhoulong.xyz/gtvppvlnxy.html

D. 数组 / 列表 / 集合
来源：http://hz.dianchejie.cn/gtikuazszp.html

================================================================================
来源：http://hz.ybcxt.top/gtrzfcdqbf.html

[D01] 创建数组 / 列表
来源：http://hz.9152youxi.cn/gtweaudktw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cheryme.top/gtstbldqdi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xinyue.icu/gttgjioimi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.fengsongda.top/gtmvbdngqa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.c1oappe.top/gtvpbuqrqk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yj202588.top/gtlzsjwlyr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.tianlin.xyz/gtpjqytnbk.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cqqwz.cn/gtprojgmdy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aibaodan.cn/gtffxuscer.html

[D02] 追加元素到末尾
来源：http://hz.wangdashe.top/gtsciqtguj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.bjfxy.top/gtkomhgbze.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sxryk.cn/gtpjkcfbfs.html

JS:   arr.push(4);
来源：http://hz.gzhubu.top/gtfdrzybmu.html

TS:   arr.push(4);
来源：http://hz.tianlin.xyz/gtcvdplsln.html

Java: list.add(4);
来源：http://hz.yuxming.cn/gtzasnowxm.html

Go:   arr = append(arr, 4)
来源：http://hz.sweek.top/gtymxqlzjd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xingfuxueyuan.xyz/gtzucsdsae.html

C#:   list.Add(4);
来源：http://hz.cashguo.top/gtegrrmwbo.html

[D03] 在指定位置插入元素
来源：http://hz.meibo888.top/gtedikzdgq.html

Py:   arr.insert(0, 0)
来源：http://hz.xingfuxueyuan.xyz/gtbzgcgngc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ywan-chungtsiang.top/gtzvwtujsn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.dashuyun.cn/gtojtxvspy.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.havefunace.top/gtkdmscnvv.html

Java: list.add(0, 0);
来源：http://hz.birdmap.top/gtdymaihku.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhiwuduotai.top/gtcnclnaqf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhijiandao.cn/gtnzezulpd.html

C#:   list.Insert(0, 0);
来源：http://hz.tian-w.cn/gtjhgqrikg.html

[D04] 删除元素
来源：http://hz.sweek.top/gtmdpnruvp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.wangshuangyany.cn/gtmepcpwvj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cashguo.top/gtzcdpfbtn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hysaishi.cn/gtkpnrdzxr.html

TS:   arr.splice(0, 1);
来源：http://hz.bjfxy.top/gtzkjhvbmi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.andypj.xyz/gtjlnicawy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yanxiufei.cn/gtncmxqfvz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.52xcode.cn/gtqwabzzod.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.kuanghao11.cn/gtkkbhsgfx.html

[D05] 访问与修改元素
来源：http://hz.yj20258.top/gtgojbnlvw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gtbzoipdvp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xinyue.icu/gtfroxintd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.aizwys.cn/gtjihinmff.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.daria6918.cn/gthkjhoidf.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cdnleiting.top/gtqgjqfsds.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.dashuyun.cn/gtnkxlrrau.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daria6918.cn/gtjuurmmdw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.tian-w.cn/gtzetvacvk.html

[D06] 数组长度
来源：http://hz.zycfv.cn/gtwiuqjzwh.html

Py:   len(arr)
来源：http://hz.ybcxt.top/gtlciywuvn.html

PHP:  count($arr);
来源：http://hz.havefunace.top/gtokypmzre.html

JS:   arr.length
来源：http://hz.xuanzx.com/gtlohgjnmk.html

TS:   arr.length
来源：http://hz.cashguo.top/gtefhpudce.html

Java: list.size();
来源：http://hz.shzxlz.cn/gtdksgtwjt.html

Go:   len(arr)
来源：http://hz.jqgufenzy.top/gtawwizvtj.html

Ruby: arr.length; arr.size
来源：http://hz.cqqwz.cn/gtkjnqiege.html

C#:   list.Count;
来源：http://hz.meibo888.top/gtookylpse.html

[D07] 切片 / 取子数组
来源：http://hz.jiagoushi.top/gtorpqnjwe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.gogol.net.cn/gtldmplown.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.iojbl.cn/gtvvhrzkkw.html

JS:   arr.slice(1, 4);
来源：http://hz.zhoulong.xyz/gtqofbxovr.html

TS:   arr.slice(1, 4);
来源：http://hz.yuanzhike.top/gthjthsvhw.html

Java: list.subList(1, 4);
来源：http://hz.zycfv.cn/gtkxrjwiib.html

Go:   arr[1:4]
来源：http://hz.c1oappe.top/gtlhwbkgdf.html

Ruby: arr[1, 3]
来源：http://hz.shzxlz.cn/gthatvxise.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangkeji.top/gtjkqoaxup.html

[D08] 合并两个数组
来源：http://hz.gotoacloud.top/gttlqkurra.html

Py:   a + b;  a.extend(b)
来源：http://hz.xingfuxueyuan.xyz/gtlpiaokob.html

PHP:  array_merge($a, $b);
来源：http://hz.ehwqpu.com/gtdggecupj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.0kj1m.cn/gtkedcrhiv.html

TS:   [...a, ...b];
来源：http://hz.zhixingplan.top/gtsuexnzvc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhoulong.xyz/gtjqmqpejm.html

Go:   append(a, b...)
来源：http://hz.xinyue.icu/gtgnwphtmp.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ehwqpu.com/gtkewfovsm.html

C#:   a.Concat(b).ToList()
来源：http://hz.nanxuanxn.top/gtqqbpvczg.html

[D09] 排序（升序）
来源：http://hz.jinghuilouyu.cn/gthiybopqt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtxbhbsjtw.html

PHP:  sort($arr);
来源：http://hz.cucudq.cn/gtxpknrsxz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.daxiang520.top/gtihylehdp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shanyushiyangkeji.top/gttggthhpq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj20258.top/gtodmijzqj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gtdctbqqjp.html

Ruby: arr.sort
来源：http://hz.smart0.xyz/gtudpjxrlt.html

C#:   list.Sort();
来源：http://hz.zhijiandao.cn/gtofipwdwj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinghuilouyu.cn/gtasonmojc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ydjk.org.cn/gtjtlhmgql.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenzaomai.com/gtucexdoeh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fengsongda.top/gtvttxyhsg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.mhx1999.top/gtmbhcpfwd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj202588.top/gtrviknlxb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xinyue.icu/gtjzjbrsdf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cheryme.top/gtqagikwiu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj20258888.top/gtzeotehty.html

[D11] 反转数组
来源：http://hz.zdqjudy.top/gtqwnekeme.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cashguo.top/gtxprxhlps.html

PHP:  array_reverse($arr);
来源：http://hz.gzhubu.top/gtcacrqbgj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yj202588.top/gtjpntbokw.html

TS:   [...arr].reverse();
来源：http://hz.jianghu66.top/gtseuuctkh.html

Java: Collections.reverse(list);
来源：http://hz.yonumen.top/gtggujpqfc.html

Go:   slices.Reverse(arr)
来源：http://hz.shzxlz.cn/gtfmysmniz.html

Ruby: arr.reverse
来源：http://hz.gotoacloud.top/gtikhzgawg.html

C#:   list.Reverse();
来源：http://hz.cdnleiting.top/gtkvydyjfw.html

[D12] 查找元素下标
来源：http://hz.yueranfly.top/gtxcbgefua.html

Py:   arr.index(x);  x in arr
来源：http://hz.nanxinkj.top/gtfyxpftjn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhaomingkeji.xyz/gtnbtqenka.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.birdmap.top/gthbbadxry.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhengqikj.top/gtlrqeoawt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hammf.cn/gtakgoglng.html

Go:   slices.Index(arr, x)
来源：http://hz.zycfv.cn/gtxvkqzjyv.html

Ruby: arr.index(x)
来源：http://hz.zhiwuduotai.top/gtgqcvmicx.html

C#:   list.IndexOf(x);
来源：http://hz.jinyuanbaomall.cn/gtzogqxojf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hammf.cn/gtadivxevs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.aizwys.cn/gttqahrtjo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sxryk.cn/gtocoyjmtj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.52xcode.cn/gtzehpobwb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sysykeji.top/gtjjeseioa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.haohaochexian.top/gtauoqqiav.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.quarkkingdee.top/gtjjylnuju.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.tianlin.xyz/gteimazxxj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cdnleiting.top/gtignkwzql.html

[D14] 映射转换（每个元素变形）
来源：http://hz.0kj1m.cn/gtyddcwwef.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.kuanghao11.cn/gtqbhprtrv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.mhx1999.top/gtbuwraybs.html

JS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gtolciaakv.html

TS:   arr.map(x => x * 2)
来源：http://hz.yangfankeji.com/gtjhximirr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhengqikj.top/gtxxkfermf.html

Go:   // 手写循环
来源：http://hz.9152youxi.cn/gtdwfdplht.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.smart0.xyz/gtylsuocju.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hongshengwenyu.top/gtxkenkxnx.html

[D15] 去重
来源：http://hz.pycfn.com/gtnxfljwdk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinghuilouyu.cn/gtqotfwhao.html

PHP:  array_unique($arr);
来源：http://hz.redwolf501.top/gtraxkcgqn.html

JS:   [...new Set(arr)]
来源：http://hz.jinqigufen.top/gtfviclmye.html

TS:   [...new Set(arr)]
来源：http://hz.haohaochexian.top/gtsmskdjls.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dashuyun.cn/gtnstqpxnv.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.dashuyun.cn/gtnwwnqvko.html

Ruby: arr.uniq
来源：http://hz.zhiwuduotai.top/gtkibymlpv.html

C#:   list.Distinct().ToList()
来源：http://hz.hammf.cn/gthbywxcrp.html

[D16] 求和与平均值
来源：http://hz.xingfuxueyuan.xyz/gtmtupgsbd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yonumen.top/gtwkylaxwm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinghuilouyu.cn/gtaqfaljxk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gotoacloud.top/gtdtnubuog.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pycfn.com/gtrpnafclw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.iojbl.cn/gtkmxrvyup.html

Go:   // 手写循环累加
来源：http://hz.shanyushiyangtech.top/gtshwdajdl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhaomingkeji.xyz/gtjaqnyual.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinqigufen.top/gtopumybcy.html

[D17] 最大值与最小值
来源：http://hz.aizwys.cn/gtpagxkmwc.html

Py:   max(arr);  min(arr)
来源：http://hz.aizwys.cn/gtakwxvdoy.html

PHP:  max($arr);  min($arr);
来源：http://hz.meibo888.top/gtsjothfmq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gotoacloud.top/gtexcgpvrk.html

TS:   Math.max(...arr);
来源：http://hz.pengpengdd.cyou/gtelmjzljp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gotoacloud.top/gtfbwmhjpm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sxryk.cn/gtssjazsio.html

Ruby: arr.max;  arr.min
来源：http://hz.sxryk.cn/gtvvoyfzja.html

C#:   list.Max();  list.Min()
来源：http://hz.zycfv.cn/gtvqssgmix.html

[D18] 扁平化嵌套数组
来源：http://hz.hammf.cn/gtnsjwftua.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hnqzz.top/gtqzqyphlu.html

PHP:  array_merge(...$nested);
来源：http://hz.shanyushiyangkeji.top/gtbxltqaff.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.316326.xyz/gtunbyjcyk.html

TS:   nested.flat();
来源：http://hz.quarkkingdee.top/gtlkebffzs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cdnleiting.top/gtdmgviblb.html

Go:   // 手写双层循环
来源：http://hz.hnqzz.top/gtxipglwmi.html

Ruby: nested.flatten
来源：http://hz.zhengqikj.top/gtobnbirap.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xinyue.icu/gtyojwwxrq.html

[D19] 按字段分组
来源：http://hz.shanyushiyangkeji.top/gtnvspixcc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.feifeiyinyue.top/gtjcnwustm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nanxuanxn.top/gtrazngyyk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shangyingyoupin.top/gtywtkdtcj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jyoumei.cn/gtzezacwrk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yanxiufei.cn/gtwfhjbigi.html

Go:   // 手写 map[string][]T
来源：http://hz.zhiwuduotai.top/gtrejjugji.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.chenlongwang.top/gtuotwylll.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jlsjyb.cn/gtrgtmjlza.html

[D20] 统计每个元素出现次数
来源：http://hz.hysaishi.cn/gtwgxgsfvt.html

Py:   Counter(arr)
来源：http://hz.yvedp.cn/gtrhyiwadz.html

PHP:  array_count_values($arr);
来源：http://hz.dianchejie.cn/gtjmkopqwv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtkjoerqop.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zycfv.cn/gtcsbiivrf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hywenlv.cn/gtbwuqkiyo.html

Go:   // 手写 map[T]int
来源：http://hz.daxiang520.top/gtmpbnksns.html

Ruby: arr.tally
来源：http://hz.ivvv.top/gthrouwipw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinqigufen.top/gtfvwpktxl.html

[D21] 判断是否包含某元素
来源：http://hz.shanyushiyangtech.top/gtcoozsfjz.html

Py:   x in arr
来源：http://hz.chenjidiqi.icu/gtdqcpveum.html

PHP:  in_array($x, $arr, true);
来源：http://hz.kuanghao11.cn/gtoldzmrpk.html

JS:   arr.includes(x)
来源：http://hz.cucudq.cn/gtphjbumkb.html

TS:   arr.includes(x)
来源：http://hz.9152youxi.cn/gtgrdiknzt.html

Java: list.contains(x)
来源：http://hz.sweek.top/gthuqlmfxv.html

Go:   slices.Contains(arr, x)
来源：http://hz.sufxvd.cn/gtujtjikff.html

Ruby: arr.include?(x)
来源：http://hz.ywan-chungtsiang.top/gtytfqtauv.html

C#:   list.Contains(x)
来源：http://hz.xinyue.icu/gthwiooqdl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinqigufen.top/gtshocttdg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yangfankeji.com/gtyahnkkhv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tian-w.cn/gtsxlpnwoh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ydzc1.top/gtvzbnnthr.html

TS:   [...arr];
来源：http://hz.yangfankeji.com/gtmtlabrod.html

Java: new ArrayList<>(list);
来源：http://hz.fengsongda.top/gtvguqipcv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hysaishi.cn/gtndfjukek.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sxryk.cn/gttveckfck.html

C#:   new List<int>(list);
来源：http://hz.shuidangran.top/gtzvfsznaw.html

[D23] reduce 累积计算
来源：http://hz.yj202588.top/gtiklscojg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj20258888.top/gtihezqcmu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.dashuyun.cn/gtaxumzksd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jianghu66.top/gteiqqnohm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuanzhike.top/gtnqowathu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.chenzaomai.com/gtdfsfnrie.html

Go:   // 手写循环
来源：http://hz.guannengcc.top/gtprumywvu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.guowangkeji.top/gtzwykxosb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinqigufen.top/gtgwvsgtue.html

[D24] 字典 / Map 基本操作
来源：http://hz.sysykeji.top/gtteshqeok.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.nwbrower.top/gtdenkxdpm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jyoumei.cn/gtlhedhodh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gogol.net.cn/gtmawjdanf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.pengpengdd.cyou/gtpaiuzqza.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.dashuyun.cn/gtxzzzsyag.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xuetiantiany.cn/gtzrkaigba.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.52xcode.cn/gtkvgxgqrg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xuanzx.com/gtekveleso.html

[D25] Set 集合去重与交并差
来源：http://hz.quarkkingdee.top/gtkycftwtc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.smart0.xyz/gtbyomotmm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.daxiang520.top/gtxvhfesru.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhijiandao.cn/gttgmybmsr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhiwuduotai.top/gtrxpefaky.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gaohongyu789.top/gtfqrksfya.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xuanzx.com/gtcgyladfm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhongyouzk.top/gtqpespkls.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xingfuxueyuan.xyz/gteappogst.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangkeji.top/gtksarpsag.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shuidangran.top/gtpqvcnjnw.html

PHP:  implode(", ", $arr);
来源：http://hz.fengsongda.top/gtzcjlmwem.html

JS:   arr.join(", ")
来源：http://hz.fengsongda.top/gtzcppyynz.html

TS:   arr.join(", ")
来源：http://hz.bjfxy.top/gtsrboquqa.html

Java: String.join(", ", list)
来源：http://hz.xuanzx.com/gtxmnztexa.html

Go:   strings.Join(strs, ", ")
来源：http://hz.wangshuangyany.cn/gtprwgpbws.html

Ruby: arr.join(", ")
来源：http://hz.jinyuanbaomall.cn/gttkxfjtdi.html

C#:   string.Join(", ", list)
来源：http://hz.jinqigufen.top/gtltgjjzfu.html

================================================================================
来源：http://hz.shzxlz.cn/gtmqiiwgta.html

E. 字符串处理
来源：http://hz.zhaomingkeji.xyz/gtfkvaeyao.html

================================================================================
来源：http://hz.cheryme.top/gtpawqjskc.html

[E01] 拼接字符串
来源：http://hz.guowangkeji.top/gtcvxcixhl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shangyingyoupin.top/gthzpthrnr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jiagoushi.top/gtlpuxjray.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shangyingyoupin.top/gtsyfrfdhs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yanxiufei.cn/gtzqtqidyk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yuxming.cn/gtlecyqjmn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gogol.net.cn/gtijcbiozz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jiagoushi.top/gtvduazzrs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xuetiantiany.cn/gtrwulsoqb.html

[E02] 重复字符串
来源：http://hz.kuanghao11.cn/gtgcvhrbqh.html

Py:   "ab" * 3
来源：http://hz.meibo888.top/gtwznwemot.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xylfe.cn/gtxgreawqp.html

JS:   "ab".repeat(3)
来源：http://hz.guowangkeji.top/gtiousakjj.html

TS:   "ab".repeat(3)
来源：http://hz.jlsjyb.cn/gtnihlaqcx.html

Java: "ab".repeat(3)
来源：http://hz.gotoacloud.top/gtfuxkdfah.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shzxlz.cn/gtjspcvdln.html

Ruby: "ab" * 3
来源：http://hz.xuanzx.com/gtkgpceaui.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.tianlin.xyz/gtfhjjuvtk.html

[E03] 截取子串
来源：http://hz.ydzc1.top/gtadyangmd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jiagoushi.top/gtncpwkxzr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.andypj.xyz/gtbqlrwszz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cdnleiting.top/gtktsdwtms.html

TS:   s.slice(1, 4)
来源：http://hz.yj202588.top/gtdjhpifus.html

Java: s.substring(1, 4)
来源：http://hz.jyoumei.cn/gtytltodqd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.chenzaomai.com/gtrbzechbq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.svipenyu.cn/gtlztjpmvh.html

C#:   s.Substring(1, 3)
来源：http://hz.shanyushiyangkeji.top/gtzgxuselt.html

[E04] 查找子串位置
来源：http://hz.shangyingyoupin.top/gtglijxykl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cheryme.top/gtgmgobjsg.html

PHP:  strpos($s, "x");
来源：http://hz.zycfv.cn/gtbtrxegvh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.aizwys.cn/gtxvvflbct.html

TS:   s.indexOf("x")
来源：http://hz.tianlin.xyz/gtfoftipjt.html

Java: s.indexOf("x")
来源：http://hz.havefunace.top/gtmpzwlfez.html

Go:   strings.Index(s, "x")
来源：http://hz.fzhhl.top/gtsznxnrpe.html

Ruby: s.index("x")
来源：http://hz.fzhhl.top/gtepgzhdbt.html

C#:   s.IndexOf("x")
来源：http://hz.xinyue.icu/gtykqletfc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yj202588.top/gttazbgkns.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.gogol.net.cn/gtconlbedm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.0kj1m.cn/gtjphgwckq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.aibaodan.cn/gttkbfmyih.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.pengpengdd.cyou/gtvyvlrnvw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258888.top/gtetgfatrn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yuxming.cn/gtublfydpu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jinqigfzy.top/gtggjdhzta.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sufxvd.cn/gtvikpzqgt.html

[E06] 替换子串
来源：http://hz.sxryk.cn/gtvujnalmm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cheryme.top/gtnqjnmtfk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.dashuyun.cn/gtqihzlgty.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gtibfpvhuz.html


<!-- 参考信息 -->