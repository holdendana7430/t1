代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.kuanghao11.cn/gtzpjvkfoi.html

[C15] 解构 / 展开参数
来源：http://hz.vqdsnc.cn/gtjllkktmu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xuetiantiany.cn/gtdwnpgfbk.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jqgufenzy.top/gtvqhfabun.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yangfankeji.com/gtnojjzcwb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinqigfzy.top/gtrdohakyf.html

Java: // 无解构
来源：http://hz.zhiwuduotai.top/gtzrtovclq.html

Go:   // 无解构
来源：http://hz.feifeiyinyue.top/gtowlbkdms.html

Ruby: a, b = pair
来源：http://hz.andypj.xyz/gtsickqxgp.html

C#:   var (a, b) = pair;
来源：http://hz.bjfxy.top/gtcruecyfu.html

[C16] 函数 / 方法重载
来源：http://hz.chenjidiqi.icu/gtmgdrdoxa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.mhx1999.top/gtzlzyqldn.html

PHP:  // 无重载
来源：http://hz.fzhhl.top/gtilmhbzel.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ppjwa.cn/gtxzpxnery.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhiwuduotai.top/gtvcuooouk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenjidiqi.icu/gtzdkchuem.html

Go:   // 无重载：用不同函数名
来源：http://hz.ppjwa.cn/gtrnqphrmb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yj20258888.top/gtxtllmxup.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.aibaodan.cn/gtqloyejob.html

================================================================================
来源：http://hz.52xcode.cn/gtoxtxtdtl.html

D. 数组 / 列表 / 集合
来源：http://hz.jinyuanbaomall.cn/gtjifnimjm.html

================================================================================
来源：http://hz.jlsjyb.cn/gtrvdbfnne.html

[D01] 创建数组 / 列表
来源：http://hz.zhixingplan.top/gtgjwfxfmr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xylfe.cn/gtbxazxnlq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.daria6918.cn/gtsxktpvkx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.316326.xyz/gtuzvlxxek.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.iojbl.cn/gtvmqxjvdv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hnxiangtu.top/gtzudevlem.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zycfv.cn/gtfnefjgdn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yueranfly.top/gtwfhsffmi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.pengpengdd.cyou/gtdsntjyhu.html

[D02] 追加元素到末尾
来源：http://hz.ydzc1.top/gtxwxomccl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yangfankeji.com/gtoojyzzbs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sxryk.cn/gtzpxsiuqm.html

JS:   arr.push(4);
来源：http://hz.ivvv.top/gtcoevqity.html

TS:   arr.push(4);
来源：http://hz.yongpay.top/gtyeojjrhk.html

Java: list.add(4);
来源：http://hz.feifeiyinyue.top/gthosrfmlv.html

Go:   arr = append(arr, 4)
来源：http://hz.hysaishi.cn/gttszxcohh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhaomingkeji.xyz/gtldsvpblu.html

C#:   list.Add(4);
来源：http://hz.0kj1m.cn/gtqmvuwkup.html

[D03] 在指定位置插入元素
来源：http://hz.yuxming.cn/gtvkotpssm.html

Py:   arr.insert(0, 0)
来源：http://hz.9152youxi.cn/gteiviipka.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gogol.net.cn/gtgrxbtwhe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cdnleiting.top/gttybidraj.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinqigfzy.top/gtgipfmfaj.html

Java: list.add(0, 0);
来源：http://hz.sxryk.cn/gtnyqktenv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cheryme.top/gtwmmghnct.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xziqi.cn/gtwglxzmdk.html

C#:   list.Insert(0, 0);
来源：http://hz.hysaishi.cn/gtphprlqvj.html

[D04] 删除元素
来源：http://hz.yuxming.cn/gtlzukxvrz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zycfv.cn/gtgwhdaedn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.haohaochexian.top/gtsnatzeqt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.mhx1999.top/gtdpyfajwu.html

TS:   arr.splice(0, 1);
来源：http://hz.aizwys.cn/gtbcflcvic.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tanke756.top/gtlvhpyjpi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.mhx1999.top/gtkxyqytkx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.guowangkeji.top/gtmeqqjaaz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yuanzhike.top/gtendeapce.html

[D05] 访问与修改元素
来源：http://hz.gaohongyu789.top/gtmjfcuihd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangdashe.top/gtctqzxkqb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinyuanbaomall.cn/gtltestuqr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shanyushiyangtech.top/gtgsbyqxyj.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.meibo888.top/gtogfhhinr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.haohaochexian.top/gtudfooahn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.dianchejie.cn/gtzbbzotix.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.haohaochexian.top/gtnzgdqyvn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.dianchejie.cn/gteregmfzp.html

[D06] 数组长度
来源：http://hz.havefunace.top/gtmhclxbpx.html

Py:   len(arr)
来源：http://hz.zhongyouzk.top/gtujymqkbg.html

PHP:  count($arr);
来源：http://hz.zdqjudy.top/gtzwmqzxkf.html

JS:   arr.length
来源：http://hz.shuidangran.top/gtndqnmsqa.html

TS:   arr.length
来源：http://hz.hammf.cn/gtdohjssny.html

Java: list.size();
来源：http://hz.zycfv.cn/gtdjggzmyx.html

Go:   len(arr)
来源：http://hz.nanxuanxn.top/gtmrosrebg.html

Ruby: arr.length; arr.size
来源：http://hz.ppjwa.cn/gtuldqyepd.html

C#:   list.Count;
来源：http://hz.pengpengdd.cyou/gtyotdoiwa.html

[D07] 切片 / 取子数组
来源：http://hz.zhiwuduotai.top/gtfbdyczga.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.havefunace.top/gtkmfxniei.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zdqjudy.top/gtyljhyzzn.html

JS:   arr.slice(1, 4);
来源：http://hz.9152youxi.cn/gtnyvrdzub.html

TS:   arr.slice(1, 4);
来源：http://hz.tian-w.cn/gtnoypnteg.html

Java: list.subList(1, 4);
来源：http://hz.xylfe.cn/gtzhvfvetk.html

Go:   arr[1:4]
来源：http://hz.shzxlz.cn/gtrozkqogs.html

Ruby: arr[1, 3]
来源：http://hz.wangdashe.top/gtjywzyrkl.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258888.top/gtuxjenyku.html

[D08] 合并两个数组
来源：http://hz.yj20258.top/gtuiagcenq.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhoulong.xyz/gtwlpiflhf.html

PHP:  array_merge($a, $b);
来源：http://hz.jiagoushi.top/gtowizqhpk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.sxryk.cn/gtzyobtggw.html

TS:   [...a, ...b];
来源：http://hz.svipenyu.cn/gtsayashpz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gogol.net.cn/gtutucgodn.html

Go:   append(a, b...)
来源：http://hz.cqqwz.cn/gtmvgivtlj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinyuanbaomall.cn/gtphjwmmlx.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj202588.top/gtjvqkwgxz.html

[D09] 排序（升序）
来源：http://hz.sxryk.cn/gtoxapmnbz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtcryjwnlc.html

PHP:  sort($arr);
来源：http://hz.havefunace.top/gtyovfuwdc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.mhx1999.top/gtazeayyff.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.iojbl.cn/gtsmgtjkjf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.meibo888.top/gtcgxixjkn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.aizwys.cn/gtkhojvtjq.html

Ruby: arr.sort
来源：http://hz.ydjk.org.cn/gteoriwvcn.html

C#:   list.Sort();
来源：http://hz.sysykeji.top/gtexgzmefi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.daria6918.cn/gtihekypjj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.svipenyu.cn/gtuqsqplrg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hongshengwenyu.top/gtgxfeprjf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ywan-chungtsiang.top/gtrauqgkmd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hfpthk.cn/gtuehpybcf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinqigufen.top/gtohikling.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.feifeiyinyue.top/gtclkctplb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.9152youxi.cn/gtirvqoskj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tanke756.top/gtczssaowd.html

[D11] 反转数组
来源：http://hz.haohaochexian.top/gtoozygisq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhoulong.xyz/gtuappcaid.html

PHP:  array_reverse($arr);
来源：http://hz.daria6918.cn/gtqopfurvc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yueranfly.top/gtnjteqksy.html

TS:   [...arr].reverse();
来源：http://hz.xinyue.icu/gtnqekwino.html

Java: Collections.reverse(list);
来源：http://hz.xziqi.cn/gttdsltqwq.html

Go:   slices.Reverse(arr)
来源：http://hz.jqgufenzy.top/gtqwuoqboq.html

Ruby: arr.reverse
来源：http://hz.feifeiyinyue.top/gtotwkezbp.html

C#:   list.Reverse();
来源：http://hz.ivvv.top/gteilrbvpp.html

[D12] 查找元素下标
来源：http://hz.ybcxt.top/gtitogxexj.html

Py:   arr.index(x);  x in arr
来源：http://hz.chenjidiqi.icu/gtbbmlcxxg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.andypj.xyz/gtuirugxdj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hfpthk.cn/gthefvpdke.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nanxinkj.top/gtugdnyofd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ehwqpu.com/gtlbdvyrlx.html

Go:   slices.Index(arr, x)
来源：http://hz.wangdashe.top/gtidtfdqfm.html

Ruby: arr.index(x)
来源：http://hz.vqdsnc.cn/gtqxowxpyf.html

C#:   list.IndexOf(x);
来源：http://hz.yuxming.cn/gtlypxggyp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.quarkkingdee.top/gtmezomyhu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.meibo888.top/gtxsksraxb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hysaishi.cn/gttgfxzhoa.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinqigfzy.top/gtilzgjaiz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sufxvd.cn/gtabflqgtv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gzhubu.top/gtmsnnddpa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhixingplan.top/gtspdhzthz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.aizwys.cn/gtmuizdbau.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jianghu66.top/gtxsczpmnp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jyoumei.cn/gtvuiydgqa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.quarkkingdee.top/gtglpjsvma.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhijiandao.cn/gtzjtcqqjn.html

JS:   arr.map(x => x * 2)
来源：http://hz.meibo888.top/gtsjgbdgze.html

TS:   arr.map(x => x * 2)
来源：http://hz.meibo888.top/gtpitwqyoe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ydzc1.top/gtltpawddj.html

Go:   // 手写循环
来源：http://hz.zhaomingkeji.xyz/gteiqewcrn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yonumen.top/gtpdvuqdby.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xuanzx.com/gtcucxrmpm.html

[D15] 去重
来源：http://hz.zdqjudy.top/gtrvsnygtj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yanxiufei.cn/gtsiviusqm.html

PHP:  array_unique($arr);
来源：http://hz.ybcxt.top/gtctrescnn.html

JS:   [...new Set(arr)]
来源：http://hz.9152youxi.cn/gtpqzramgz.html

TS:   [...new Set(arr)]
来源：http://hz.ivvv.top/gthfpqpiyk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.316326.xyz/gthebzviji.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nanxinkj.top/gtfjajuvgj.html

Ruby: arr.uniq
来源：http://hz.jinqigfzy.top/gtbiitxppk.html

C#:   list.Distinct().ToList()
来源：http://hz.gzhubu.top/gtzsgwtnab.html

[D16] 求和与平均值
来源：http://hz.ydzc1.top/gtdpmsxunz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.daria6918.cn/gtmxidaxsm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pycfn.com/gtkcoubdpz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hywenlv.cn/gtodovttyn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.0kj1m.cn/gtptmpcugw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.aizwys.cn/gtmxghxmda.html

Go:   // 手写循环累加
来源：http://hz.52xcode.cn/gtcpdpcphm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.redwolf501.top/gtkczgrbrv.html

C#:   list.Sum();  list.Average()
来源：http://hz.jqgufenzy.top/gtbgxgrlpb.html

[D17] 最大值与最小值
来源：http://hz.cdnleiting.top/gtyzpjqcnv.html

Py:   max(arr);  min(arr)
来源：http://hz.316326.xyz/gtvqtwlibx.html

PHP:  max($arr);  min($arr);
来源：http://hz.jiagoushi.top/gtiexwfdao.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.nanxuanxn.top/gtmxvcryqv.html

TS:   Math.max(...arr);
来源：http://hz.zdqjudy.top/gtoirejmya.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ybcxt.top/gtvftuvjga.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sweek.top/gtpuvipjod.html

Ruby: arr.max;  arr.min
来源：http://hz.cdnleiting.top/gtuwejmkry.html

C#:   list.Max();  list.Min()
来源：http://hz.sxryk.cn/gtqidzpavn.html

[D18] 扁平化嵌套数组
来源：http://hz.hfpthk.cn/gtsopfuhqe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shangyingyoupin.top/gtzpmvewrh.html

PHP:  array_merge(...$nested);
来源：http://hz.yuxming.cn/gtjvmlglyt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xinyue.icu/gtlnfiulbj.html

TS:   nested.flat();
来源：http://hz.ydjk.org.cn/gtwkbmlbrr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.bjfxy.top/gtyicmfsxu.html

Go:   // 手写双层循环
来源：http://hz.smart0.xyz/gtzudszjeu.html

Ruby: nested.flatten
来源：http://hz.daxiang520.top/gtdvjpvbhv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gzhubu.top/gtvxvxuwki.html

[D19] 按字段分组
来源：http://hz.gaohongyu789.top/gtbcvecdtx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.vqdsnc.cn/gtsmdvnzmx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hongshengwenyu.top/gtetrpslau.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinghuilouyu.cn/gtqbrcrjak.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gtvecitowt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yuxming.cn/gtvhqtwxrx.html

Go:   // 手写 map[string][]T
来源：http://hz.yj202588.top/gtttgsmpzk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.haohaochexian.top/gtkhvnykuc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.sweek.top/gtdtxwovkx.html

[D20] 统计每个元素出现次数
来源：http://hz.cashguo.top/gtkvgolopk.html

Py:   Counter(arr)
来源：http://hz.meibo888.top/gtdpeetlbo.html

PHP:  array_count_values($arr);
来源：http://hz.yj20258.top/gtfzxmgpuq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.quarkkingdee.top/gtuufexebm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yangfankeji.com/gtyjmllzdl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dashuyun.cn/gtszedjmsb.html

Go:   // 手写 map[T]int
来源：http://hz.hnxiangtu.top/gttnruheee.html

Ruby: arr.tally
来源：http://hz.xuanzx.com/gtnwhergdw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xinyue.icu/gtjtzcwoyh.html

[D21] 判断是否包含某元素
来源：http://hz.yuanzhike.top/gtenpjxnjg.html

Py:   x in arr
来源：http://hz.c1oappe.top/gtpxqnwnga.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yj20258.top/gtknealxka.html

JS:   arr.includes(x)
来源：http://hz.andypj.xyz/gtsbjojqab.html

TS:   arr.includes(x)
来源：http://hz.tian-w.cn/gtdxpzvbyh.html

Java: list.contains(x)
来源：http://hz.yj20258.top/gtmpdzjknf.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenzaomai.com/gtkmgunrot.html

Ruby: arr.include?(x)
来源：http://hz.daxiang520.top/gtetgdgavj.html

C#:   list.Contains(x)
来源：http://hz.vqdsnc.cn/gtjsbleaay.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yonumen.top/gtjvrhcuxn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cashguo.top/gttogxvhki.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xinyue.icu/gtklwrpbbs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ybcxt.top/gtofuhpssw.html

TS:   [...arr];
来源：http://hz.bjfxy.top/gtxeqwdobe.html

Java: new ArrayList<>(list);
来源：http://hz.ybcxt.top/gtkhvuxyql.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jlsjyb.cn/gtynjxzfey.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xylfe.cn/gtwqvezdka.html

C#:   new List<int>(list);
来源：http://hz.tian-w.cn/gtyeecoyvv.html

[D23] reduce 累积计算
来源：http://hz.jqgfzy.top/gtrgejqmkp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xuetiantiany.cn/gtlgpxiuda.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.iojbl.cn/gtnyqkpkoj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ppjwa.cn/gtxpzfcmkc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yvedp.cn/gttknbrcwt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhixingplan.top/gtnawphpya.html

Go:   // 手写循环
来源：http://hz.shanyushiyangtech.top/gtwwvcgeug.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.aibaodan.cn/gtvaxiejri.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.fzhhl.top/gtivvovjym.html

[D24] 字典 / Map 基本操作
来源：http://hz.dianchejie.cn/gtmffaubre.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yonumen.top/gtjkcchxvi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xuetiantiany.cn/gtbzrxylmk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gogol.net.cn/gtpkdyyeuy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhengqikj.top/gtbxshlmks.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.guowangkeji.top/gtwlrtjuhg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yuanzhike.top/gtbatqhlfk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.dianchejie.cn/gtgetqnfcl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.316326.xyz/gtvhmquwqw.html

[D25] Set 集合去重与交并差
来源：http://hz.yj20258.top/gtfjgoehvj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ivvv.top/gtvxdnilhk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cashguo.top/gttsynxqya.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ywan-chungtsiang.top/gtmwauhjzo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gogol.net.cn/gtmglcrqum.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jqgfzy.top/gtabxljugs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cdnleiting.top/gtzvsrmzpo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.pengpengdd.cyou/gtzrbxltbw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shangyingyoupin.top/gttllqogbx.html

[D26] 数组转字符串
来源：http://hz.ywan-chungtsiang.top/gtmcnolfbh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jqgufenzy.top/gtexgkimdf.html

PHP:  implode(", ", $arr);
来源：http://hz.yj202588.top/gtnrkpwjpt.html

JS:   arr.join(", ")
来源：http://hz.xziqi.cn/gtpvntdgen.html

TS:   arr.join(", ")
来源：http://hz.yangfankeji.com/gtfmyedpir.html

Java: String.join(", ", list)
来源：http://hz.hammf.cn/gtuiqtnsqy.html

Go:   strings.Join(strs, ", ")
来源：http://hz.chenjidiqi.icu/gtogmrfuzj.html

Ruby: arr.join(", ")
来源：http://hz.gogol.net.cn/gttejkqwkx.html

C#:   string.Join(", ", list)
来源：http://hz.gogol.net.cn/gtkcrmullv.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtaachkmgt.html

E. 字符串处理
来源：http://hz.hongshengwenyu.top/gtbmuigmra.html

================================================================================
来源：http://hz.yanxiufei.cn/gtotnsqbsx.html

[E01] 拼接字符串
来源：http://hz.316326.xyz/gtienovvhg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cucudq.cn/gtsclbavef.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jqgfzy.top/gtojlqxgpc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.c1oappe.top/gtbkdqrrdp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnxiangtu.top/gtyshbsyhd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hywenlv.cn/gteryypllo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hfpthk.cn/gtbejohopz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.fengsongda.top/gtzoumieoc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinqigufen.top/gtgeolmsbj.html

[E02] 重复字符串
来源：http://hz.zdqjudy.top/gtjsmmzgzr.html

Py:   "ab" * 3
来源：http://hz.yonumen.top/gtttevzhgx.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenzaomai.com/gtpnjabqnv.html

JS:   "ab".repeat(3)
来源：http://hz.zycfv.cn/gttenmxgkt.html

TS:   "ab".repeat(3)
来源：http://hz.yuxming.cn/gtadbogrfv.html

Java: "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtmocnuldv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.havefunace.top/gtldyxrznv.html

Ruby: "ab" * 3
来源：http://hz.yvedp.cn/gtflpujafd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.bjfxy.top/gtvusqcglr.html

[E03] 截取子串
来源：http://hz.ydzc1.top/gtjstcdrsr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ivvv.top/gtbwgxnylk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtiswwwfxe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ydjk.org.cn/gtvjaisuni.html

TS:   s.slice(1, 4)
来源：http://hz.zycfv.cn/gtwrygatfv.html

Java: s.substring(1, 4)
来源：http://hz.aizwys.cn/gtadeckvzv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhengqikj.top/gtxtasjfwh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.0kj1m.cn/gtsagieoqv.html

C#:   s.Substring(1, 3)
来源：http://hz.tanke756.top/gtxtsuefvy.html

[E04] 查找子串位置
来源：http://hz.guannengcc.top/gtmupyxppj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ywan-chungtsiang.top/gtsfpkgmmp.html

PHP:  strpos($s, "x");
来源：http://hz.dashuyun.cn/gtblzqogyb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hnxiangtu.top/gtohrgeywc.html

TS:   s.indexOf("x")
来源：http://hz.svipenyu.cn/gtmpqrpgpo.html

Java: s.indexOf("x")
来源：http://hz.zhoulong.xyz/gtkrjxuobs.html

Go:   strings.Index(s, "x")
来源：http://hz.daxiang520.top/gtgxkvafjs.html

Ruby: s.index("x")
来源：http://hz.shangyingyoupin.top/gtafpsomoq.html

C#:   s.IndexOf("x")
来源：http://hz.jianghu66.top/gtjixkdjbb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yvedp.cn/gtinuhiqef.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.chenzaomai.com/gtelsmbqap.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhoulong.xyz/gtzvsmhzue.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinyuanbaomall.cn/gtkhdagevk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jyoumei.cn/gtpzclfnpn.html


<!-- 参考信息 -->