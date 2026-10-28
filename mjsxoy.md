代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.iojbl.cn/gtgvxslwgm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nwbrower.top/gtlvbvyudy.html

Java: // 无解构
来源：http://hz.chenjidiqi.icu/gtwsthvkly.html

Go:   // 无解构
来源：http://hz.gotoacloud.top/gtigemmkvt.html

Ruby: a, b = pair
来源：http://hz.yongpay.top/gtfyidtvpo.html

C#:   var (a, b) = pair;
来源：http://hz.ydzc1.top/gtrzdpcgal.html

[C16] 函数 / 方法重载
来源：http://hz.daria6918.cn/gtusligcny.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yanxiufei.cn/gtudbjefdh.html

PHP:  // 无重载
来源：http://hz.yuxming.cn/gtuhsorjxh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.birdmap.top/gtbwysjhrd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.smart0.xyz/gtsrililvf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hammf.cn/gtjikelryr.html

Go:   // 无重载：用不同函数名
来源：http://hz.hnqzz.top/gtdchwpnnf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.andypj.xyz/gtjcaomhzs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ppjwa.cn/gthdbsiqpq.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtkgakgtcn.html

D. 数组 / 列表 / 集合
来源：http://hz.bjfxy.top/gtzngqaelp.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtygpxefrs.html

[D01] 创建数组 / 列表
来源：http://hz.jinghuilouyu.cn/gtrxuuipcw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shzxlz.cn/gtbcalbcai.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.nwbrower.top/gtoumnfcju.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.andypj.xyz/gtkcjrcuff.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yueranfly.top/gtrskffcpp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cdnleiting.top/gtyhkfbetq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sweek.top/gtcdiceero.html

Ruby: arr = [1, 2, 3]
来源：http://hz.9152youxi.cn/gthloptlsa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yueranfly.top/gtsywvwwli.html

[D02] 追加元素到末尾
来源：http://hz.bjfxy.top/gtfeuqzvck.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sweek.top/gtylcptnxx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shanyushiyangtech.top/gthrlvpbhh.html

JS:   arr.push(4);
来源：http://hz.yanxiufei.cn/gtzsxuctnt.html

TS:   arr.push(4);
来源：http://hz.ehwqpu.com/gtnekbczbf.html

Java: list.add(4);
来源：http://hz.daria6918.cn/gtagxfbgca.html

Go:   arr = append(arr, 4)
来源：http://hz.jlsjyb.cn/gtnzlkeago.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.fzhhl.top/gtejbwqgtl.html

C#:   list.Add(4);
来源：http://hz.gaohongyu789.top/gtvczretxn.html

[D03] 在指定位置插入元素
来源：http://hz.bjfxy.top/gtbdfpovnq.html

Py:   arr.insert(0, 0)
来源：http://hz.52xcode.cn/gtlxdljtjr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.havefunace.top/gtiklttgkm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.fzhhl.top/gtloczfmhl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sufxvd.cn/gtemzvaazj.html

Java: list.add(0, 0);
来源：http://hz.quarkkingdee.top/gtibtwurqb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.pycfn.com/gtsprsvuty.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ppjwa.cn/gtvmeqnvqb.html

C#:   list.Insert(0, 0);
来源：http://hz.jlsjyb.cn/gtoptupzdf.html

[D04] 删除元素
来源：http://hz.svipenyu.cn/gtfxziwpca.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhijiandao.cn/gtwxmcljtg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xingfuxueyuan.xyz/gtotfinfos.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jianghu66.top/gthyetsmev.html

TS:   arr.splice(0, 1);
来源：http://hz.tian-w.cn/gtjgkjnfke.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.haohaochexian.top/gtpgfgxhkt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jqgufenzy.top/gtluhpvrlv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cqqwz.cn/gtunjgyubn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.gotoacloud.top/gtwigkoazj.html

[D05] 访问与修改元素
来源：http://hz.ppjwa.cn/gthzmeoeyd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuetiantiany.cn/gteoxijpmd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.pengpengdd.cyou/gtplpyqbfc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sufxvd.cn/gtzzyxxyvr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nanxinkj.top/gtpsjefajg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xuanzx.com/gtfzcodcnq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.daxiang520.top/gtawtvquvu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yueranfly.top/gtfpkuskci.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ivvv.top/gtdhkdxmnq.html

[D06] 数组长度
来源：http://hz.sxryk.cn/gtpipunbwn.html

Py:   len(arr)
来源：http://hz.yvedp.cn/gthumeebbb.html

PHP:  count($arr);
来源：http://hz.jinqigfzy.top/gtxhiycilb.html

JS:   arr.length
来源：http://hz.svipenyu.cn/gtoirbkows.html

TS:   arr.length
来源：http://hz.sysykeji.top/gtrtpedyct.html

Java: list.size();
来源：http://hz.vqdsnc.cn/gtwyaimedz.html

Go:   len(arr)
来源：http://hz.aizwys.cn/gtgcnxjcnp.html

Ruby: arr.length; arr.size
来源：http://hz.sxryk.cn/gtvsdandja.html

C#:   list.Count;
来源：http://hz.yuxming.cn/gtedeivgrb.html

[D07] 切片 / 取子数组
来源：http://hz.andypj.xyz/gtyuqcraon.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinqigfzy.top/gtmmwtyopb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jqgfzy.top/gtdlxcotha.html

JS:   arr.slice(1, 4);
来源：http://hz.aibaodan.cn/gtidlrtxez.html

TS:   arr.slice(1, 4);
来源：http://hz.yongpay.top/gtejqduggh.html

Java: list.subList(1, 4);
来源：http://hz.birdmap.top/gtbmovapku.html

Go:   arr[1:4]
来源：http://hz.yj20258888.top/gtlkfepskk.html

Ruby: arr[1, 3]
来源：http://hz.jianghu66.top/gtlbrqbndg.html

C#:   list.GetRange(1, 3);
来源：http://hz.ehwqpu.com/gtlxurylod.html

[D08] 合并两个数组
来源：http://hz.yj20258.top/gtciwzbdcd.html

Py:   a + b;  a.extend(b)
来源：http://hz.xuanzx.com/gtrsvibzkc.html

PHP:  array_merge($a, $b);
来源：http://hz.shanyushiyangkeji.top/gtpkyxqvkr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jiagoushi.top/gtvpgavzid.html

TS:   [...a, ...b];
来源：http://hz.nwbrower.top/gtahmtsaoh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhiwuduotai.top/gtdfvtumbg.html

Go:   append(a, b...)
来源：http://hz.jlsjyb.cn/gtgrilecbs.html

Ruby: a + b;  a.concat(b)
来源：http://hz.tianlin.xyz/gtfowvuwax.html

C#:   a.Concat(b).ToList()
来源：http://hz.pengpengdd.cyou/gtzybvwvhy.html

[D09] 排序（升序）
来源：http://hz.zhengqikj.top/gtdyvdfbbm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ivvv.top/gtfbihvqkr.html

PHP:  sort($arr);
来源：http://hz.jqgfzy.top/gtevshczln.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hnqzz.top/gtavnjafec.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.aizwys.cn/gtrcrpkmes.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ydzc1.top/gtffkrnvez.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jinqigufen.top/gtmrfrundq.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtbpasqnbu.html

C#:   list.Sort();
来源：http://hz.zhongyouzk.top/gtuiurmzte.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.chenlongwang.top/gtypinguxr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.aizwys.cn/gtchqtdiqx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jqgufenzy.top/gtbrpycrbj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxinkj.top/gtamggazbk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.meibo888.top/gtmfomlnmp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sufxvd.cn/gtthengmag.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.vqdsnc.cn/gtwqklrbcg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yonumen.top/gtikyxsoad.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yanxiufei.cn/gtrsashqjx.html

[D11] 反转数组
来源：http://hz.yj20258888.top/gtyplsdjqw.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cqqwz.cn/gtwlaejvvg.html

PHP:  array_reverse($arr);
来源：http://hz.sysykeji.top/gtniomheqw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.kuanghao11.cn/gthqqpzipe.html

TS:   [...arr].reverse();
来源：http://hz.sweek.top/gtsvjfahgm.html

Java: Collections.reverse(list);
来源：http://hz.yvedp.cn/gtlboudzhu.html

Go:   slices.Reverse(arr)
来源：http://hz.kuanghao11.cn/gtgjcoxzdn.html

Ruby: arr.reverse
来源：http://hz.zycfv.cn/gtwluskbei.html

C#:   list.Reverse();
来源：http://hz.zhiwuduotai.top/gtumonrnor.html

[D12] 查找元素下标
来源：http://hz.hnqzz.top/gtntbpqzog.html

Py:   arr.index(x);  x in arr
来源：http://hz.ywan-chungtsiang.top/gtqhiltorp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenzaomai.com/gtsupuukeo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ivvv.top/gtwfphbcmb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.smart0.xyz/gtpdkywgjk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.smart0.xyz/gtdsspmphg.html

Go:   slices.Index(arr, x)
来源：http://hz.yongpay.top/gtabmxmskd.html

Ruby: arr.index(x)
来源：http://hz.jinghuilouyu.cn/gtzvgxtvkx.html

C#:   list.IndexOf(x);
来源：http://hz.xingfuxueyuan.xyz/gtiahakbxq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sweek.top/gtbghqabtm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhengqikj.top/gtoizwibkg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.feifeiyinyue.top/gtiofuczgw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.cdnleiting.top/gtgpwfoglk.html

TS:   arr.filter(x => x > 3)
来源：http://hz.aizwys.cn/gtoqzhjbnd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shanyushiyangtech.top/gtpuyfemrc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.chenzaomai.com/gtitnfinwb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jlsjyb.cn/gtmmsvvavl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinqigfzy.top/gtucnavluo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sysykeji.top/gtimyapnpu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xuetiantiany.cn/gtsanfplew.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cucudq.cn/gtkpoxllfz.html

JS:   arr.map(x => x * 2)
来源：http://hz.smart0.xyz/gtmnqyrufy.html

TS:   arr.map(x => x * 2)
来源：http://hz.jlsjyb.cn/gtjxjgzycu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.nanxuanxn.top/gtciwpmhwk.html

Go:   // 手写循环
来源：http://hz.fengsongda.top/gtrsoxfrvq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hysaishi.cn/gtjnafscfu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.nanxinkj.top/gtuoaewzuh.html

[D15] 去重
来源：http://hz.gogol.net.cn/gtqppfmksi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ivvv.top/gtxqpdswoo.html

PHP:  array_unique($arr);
来源：http://hz.tanke756.top/gtoswdeknm.html

JS:   [...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtqusxjmbh.html

TS:   [...new Set(arr)]
来源：http://hz.jyoumei.cn/gttxundsan.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhengqikj.top/gtnoewmmeb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jiagoushi.top/gtispgjlsr.html

Ruby: arr.uniq
来源：http://hz.meibo888.top/gtcvufoagp.html

C#:   list.Distinct().ToList()
来源：http://hz.kuanghao11.cn/gtpngzojmb.html

[D16] 求和与平均值
来源：http://hz.jqgufenzy.top/gtpfgsgaac.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shuidangran.top/gtrkclwvaz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ivvv.top/gtvwboxtjl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cucudq.cn/gtsectvjsz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ppjwa.cn/gtsnrnwrfd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.c1oappe.top/gtlufeinqs.html

Go:   // 手写循环累加
来源：http://hz.shanyushiyangkeji.top/gtjxtumhpv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.chenzaomai.com/gtalhtooyi.html

C#:   list.Sum();  list.Average()
来源：http://hz.aizwys.cn/gtjqbpzwlu.html

[D17] 最大值与最小值
来源：http://hz.ybcxt.top/gtlvopvysi.html

Py:   max(arr);  min(arr)
来源：http://hz.zhixingplan.top/gtlrziundc.html

PHP:  max($arr);  min($arr);
来源：http://hz.xinyue.icu/gtbdxzbohg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.mhx1999.top/gtjwlxjhck.html

TS:   Math.max(...arr);
来源：http://hz.ydjk.org.cn/gtjpmuunqy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xuetiantiany.cn/gtvmkeqdqs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hywenlv.cn/gtxazvhiki.html

Ruby: arr.max;  arr.min
来源：http://hz.xziqi.cn/gtdlbylecm.html

C#:   list.Max();  list.Min()
来源：http://hz.gogol.net.cn/gtdcusnybb.html

[D18] 扁平化嵌套数组
来源：http://hz.snrcjt.cn/gtjkadlisb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cashguo.top/gtqbcjpuvf.html

PHP:  array_merge(...$nested);
来源：http://hz.zhongyouzk.top/gtvazykbmh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ybcxt.top/gtlisykpmr.html

TS:   nested.flat();
来源：http://hz.shzxlz.cn/gttvnugqpg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ydjk.org.cn/gtjiqpeehl.html

Go:   // 手写双层循环
来源：http://hz.zhixingplan.top/gtcjuwuqve.html

Ruby: nested.flatten
来源：http://hz.zhaomingkeji.xyz/gtyqtmauiw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shangyingyoupin.top/gtygcnlbis.html

[D19] 按字段分组
来源：http://hz.fzhhl.top/gtzqtawjix.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.guannengcc.top/gtoszddwwi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhijiandao.cn/gtrxuobzfz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ydzc1.top/gtxofpvfka.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.tian-w.cn/gtcyjlkgdo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yj20258.top/gtcrxhljwz.html

Go:   // 手写 map[string][]T
来源：http://hz.jianghu66.top/gtmxjrbhrn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yj20258888.top/gtopsroxwm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shanyushiyangtech.top/gtuxuwrono.html

[D20] 统计每个元素出现次数
来源：http://hz.shzxlz.cn/gtxvbxvnpy.html

Py:   Counter(arr)
来源：http://hz.sweek.top/gtpvgxedqp.html

PHP:  array_count_values($arr);
来源：http://hz.jinqigufen.top/gtouerajvn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.kuanghao11.cn/gtnrsznnnr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ehwqpu.com/gtgwsrygxp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.redwolf501.top/gtlnxqcajf.html

Go:   // 手写 map[T]int
来源：http://hz.chenjidiqi.icu/gthrncoxkw.html

Ruby: arr.tally
来源：http://hz.zdqjudy.top/gtuglxersq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.0kj1m.cn/gtmqeuotnd.html

[D21] 判断是否包含某元素
来源：http://hz.yj20258.top/gtvofuvwro.html

Py:   x in arr
来源：http://hz.daxiang520.top/gtpshlpxsh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.guowangkeji.top/gtbkpiuqnc.html

JS:   arr.includes(x)
来源：http://hz.c1oappe.top/gtpyixrggd.html

TS:   arr.includes(x)
来源：http://hz.feifeiyinyue.top/gtmbihmhbh.html

Java: list.contains(x)
来源：http://hz.daria6918.cn/gttnagyrgt.html

Go:   slices.Contains(arr, x)
来源：http://hz.zycfv.cn/gthjmymjtx.html

Ruby: arr.include?(x)
来源：http://hz.xziqi.cn/gtywelcmle.html

C#:   list.Contains(x)
来源：http://hz.ydzc1.top/gtlybuhonv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.mhx1999.top/gtdwpcggww.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.snrcjt.cn/gtrvfkhrvf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.andypj.xyz/gtsnfngrtv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.316326.xyz/gtddqlvpig.html

TS:   [...arr];
来源：http://hz.dianchejie.cn/gtzpgzuwbu.html

Java: new ArrayList<>(list);
来源：http://hz.hnqzz.top/gtciijovwe.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shangyingyoupin.top/gtyyaoaxyh.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gogol.net.cn/gtgpivqtip.html

C#:   new List<int>(list);
来源：http://hz.hnqzz.top/gtabhquamy.html

[D23] reduce 累积计算
来源：http://hz.ehwqpu.com/gtadshuxhu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hfpthk.cn/gtapxpggjf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.wangshuangyany.cn/gtmjybjukb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.daria6918.cn/gtbhfnnsxy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sweek.top/gtouklnpzw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yonumen.top/gtwqfuakig.html

Go:   // 手写循环
来源：http://hz.jqgufenzy.top/gtvtbdcamr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.pengpengdd.cyou/gtuiomwqqt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yanxiufei.cn/gtxvbkxhyo.html

[D24] 字典 / Map 基本操作
来源：http://hz.ivvv.top/gtcvrjytjy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhengqikj.top/gtzydxxglo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinghuilouyu.cn/gtoftwjzai.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.haohaochexian.top/gtncymrspz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jqgufenzy.top/gtthydarlz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.pycfn.com/gtrkpiufln.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.pengpengdd.cyou/gtwqvhbhfr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhiwuduotai.top/gtkdaotyuv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.0kj1m.cn/gtbqnkwaxy.html

[D25] Set 集合去重与交并差
来源：http://hz.aizwys.cn/gtvhfknhym.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.nwbrower.top/gtawfqclgd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.birdmap.top/gtbdfxccmp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jiagoushi.top/gtcyxeejyq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yvedp.cn/gtwfjsfpmx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jianghu66.top/gtqvfmcbxn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sweek.top/gtxesqmxkd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hfpthk.cn/gtjjdfvhkd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.pengpengdd.cyou/gtatkohhmo.html

[D26] 数组转字符串
来源：http://hz.yuxming.cn/gtxxpaoffw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cashguo.top/gtxboofrrm.html

PHP:  implode(", ", $arr);
来源：http://hz.zhixingplan.top/gtpdfhlanj.html

JS:   arr.join(", ")
来源：http://hz.mhx1999.top/gtesmjhzqc.html

TS:   arr.join(", ")
来源：http://hz.wangdashe.top/gtabbflevs.html

Java: String.join(", ", list)
来源：http://hz.jinqigfzy.top/gtmlanmetr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhaomingkeji.xyz/gtqulfgice.html

Ruby: arr.join(", ")
来源：http://hz.shzxlz.cn/gtyabpthnh.html

C#:   string.Join(", ", list)
来源：http://hz.quarkkingdee.top/gtddxptgll.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtyuvybpjv.html

E. 字符串处理
来源：http://hz.chenjidiqi.icu/gtjxmbvvxl.html

================================================================================
来源：http://hz.cucudq.cn/gtzmrjxkqm.html

[E01] 拼接字符串
来源：http://hz.yongpay.top/gtsmwpilsh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.nanxinkj.top/gtvdadicky.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.meibo888.top/gtxodkgecj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gtxlencuth.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.pycfn.com/gtaedhonui.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sysykeji.top/gtjokrnboq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.havefunace.top/gtvbvhxrvp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ehwqpu.com/gtjccfbidn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.tanke756.top/gtbyrfkink.html

[E02] 重复字符串
来源：http://hz.yvedp.cn/gtvrjpldff.html

Py:   "ab" * 3
来源：http://hz.dianchejie.cn/gtokrwpzly.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gzhubu.top/gtzbwuwitp.html

JS:   "ab".repeat(3)
来源：http://hz.nwbrower.top/gtdclqeczt.html

TS:   "ab".repeat(3)
来源：http://hz.cqqwz.cn/gtvnnlouxv.html

Java: "ab".repeat(3)
来源：http://hz.chenlongwang.top/gtujatswgz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jiagoushi.top/gtkwdsxsht.html

Ruby: "ab" * 3
来源：http://hz.feifeiyinyue.top/gtvtlixycb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.havefunace.top/gtifqqmenw.html

[E03] 截取子串
来源：http://hz.gzhubu.top/gtgztmjtcx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gotoacloud.top/gtjlsktszc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zdqjudy.top/gtswcmjbzn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenzaomai.com/gtccaqdtiz.html

TS:   s.slice(1, 4)
来源：http://hz.zycfv.cn/gtjrmzmfrw.html

Java: s.substring(1, 4)
来源：http://hz.zhixingplan.top/gtxufnzbnn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xuanzx.com/gtnunjqngg.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hnqzz.top/gtoquonryk.html

C#:   s.Substring(1, 3)
来源：http://hz.haohaochexian.top/gtgcisnlrg.html

[E04] 查找子串位置
来源：http://hz.tian-w.cn/gtmmxcwxvb.html

Py:   s.find("x");  s.index("x")
来源：http://hz.iojbl.cn/gtyvxsahrg.html

PHP:  strpos($s, "x");
来源：http://hz.birdmap.top/gtjbfgxakp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.dianchejie.cn/gtcwberawg.html

TS:   s.indexOf("x")
来源：http://hz.yanxiufei.cn/gtusfofyjz.html

Java: s.indexOf("x")
来源：http://hz.daria6918.cn/gtldjztmxq.html

Go:   strings.Index(s, "x")
来源：http://hz.hammf.cn/gtxdhhfrsn.html

Ruby: s.index("x")
来源：http://hz.yuanzhike.top/gtprjjyjdg.html

C#:   s.IndexOf("x")
来源：http://hz.xuetiantiany.cn/gtmddtxotn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinyuanbaomall.cn/gtehlgmcws.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.tanke756.top/gtkvtfbrpq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinghuilouyu.cn/gtpesnxhlc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenjidiqi.icu/gthnsugpvx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shzxlz.cn/gtzpamambn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.quarkkingdee.top/gtukchhzrz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenzaomai.com/gtzysceacv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.meibo888.top/gtocrjwdyy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhongyouzk.top/gtakxhqpcp.html


<!-- 参考信息 -->