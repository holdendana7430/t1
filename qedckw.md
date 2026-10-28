代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xinyue.icu/gtkokjdxxu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ivvv.top/gtsmxaxsrh.html

Java: // 无解构
来源：http://hz.yuxming.cn/gtwhmlyepz.html

Go:   // 无解构
来源：http://hz.jqgufenzy.top/gtquuezzex.html

Ruby: a, b = pair
来源：http://hz.yanxiufei.cn/gtdfflbhwr.html

C#:   var (a, b) = pair;
来源：http://hz.cucudq.cn/gtyvqaacnj.html

[C16] 函数 / 方法重载
来源：http://hz.kuanghao11.cn/gtipxcucjw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.wangshuangyany.cn/gtvknvhnel.html

PHP:  // 无重载
来源：http://hz.316326.xyz/gtzhwbqsiu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hnxiangtu.top/gtkehmvrcv.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ivvv.top/gtessmjixy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.52xcode.cn/gtgxmsjaxm.html

Go:   // 无重载：用不同函数名
来源：http://hz.daria6918.cn/gtpkgkzyfi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.chenzaomai.com/gtgztaknvz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hywenlv.cn/gtmzindtjy.html

================================================================================
来源：http://hz.nwbrower.top/gtnqvdwbnp.html

D. 数组 / 列表 / 集合
来源：http://hz.haohaochexian.top/gtddqvvoji.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtzfgrzxrj.html

[D01] 创建数组 / 列表
来源：http://hz.jianghu66.top/gtpvfssjme.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jqgufenzy.top/gtvuxnlths.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.tian-w.cn/gtmxmcayfg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zycfv.cn/gtuiqirmod.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guannengcc.top/gtymuqyvcz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ydzc1.top/gtewkxnksc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ppjwa.cn/gtlerocpby.html

Ruby: arr = [1, 2, 3]
来源：http://hz.daria6918.cn/gtucftynxc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhoulong.xyz/gtkuzqtwrs.html

[D02] 追加元素到末尾
来源：http://hz.quarkkingdee.top/gtlwzxeezj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shanyushiyangtech.top/gtzqnjjrlc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.9152youxi.cn/gtlocubsag.html

JS:   arr.push(4);
来源：http://hz.zycfv.cn/gtcydmhdgb.html

TS:   arr.push(4);
来源：http://hz.cashguo.top/gteqxfrzee.html

Java: list.add(4);
来源：http://hz.havefunace.top/gtowmqzcnw.html

Go:   arr = append(arr, 4)
来源：http://hz.jianghu66.top/gtbglhvdmq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.vqdsnc.cn/gtfbaaprpx.html

C#:   list.Add(4);
来源：http://hz.svipenyu.cn/gtuxpvakgd.html

[D03] 在指定位置插入元素
来源：http://hz.fzhhl.top/gtwimnlhpc.html

Py:   arr.insert(0, 0)
来源：http://hz.aizwys.cn/gtwlhfuydu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.chenjidiqi.icu/gtknrfdqid.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhixingplan.top/gtepzhwtcl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.0kj1m.cn/gtnzdpifzt.html

Java: list.add(0, 0);
来源：http://hz.kuanghao11.cn/gtaymgmhso.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinyuanbaomall.cn/gtbkcnfsru.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydzc1.top/gtlgeaaccu.html

C#:   list.Insert(0, 0);
来源：http://hz.shuidangran.top/gtfsiibrwk.html

[D04] 删除元素
来源：http://hz.zhijiandao.cn/gtagupwccu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zycfv.cn/gteywyylus.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.pycfn.com/gtgwndcnvh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.kuanghao11.cn/gtbokvybcm.html

TS:   arr.splice(0, 1);
来源：http://hz.smart0.xyz/gtyzgfzqul.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gotoacloud.top/gtdngzlnxa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zdqjudy.top/gtelrhbjkt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sufxvd.cn/gthknutvoc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenjidiqi.icu/gtuoajhcwi.html

[D05] 访问与修改元素
来源：http://hz.jinghuilouyu.cn/gtleodsvro.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shuidangran.top/gtmlrhvkjt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zycfv.cn/gtxravlsct.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yvedp.cn/gtasbvmscm.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.svipenyu.cn/gtvclsappi.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.andypj.xyz/gtwrqrymef.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jyoumei.cn/gtvhqxlzlb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ppjwa.cn/gtmxyuaayt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gotoacloud.top/gtilzzbmtu.html

[D06] 数组长度
来源：http://hz.jiagoushi.top/gtfiiycddi.html

Py:   len(arr)
来源：http://hz.jinyuanbaomall.cn/gtxmyrupcv.html

PHP:  count($arr);
来源：http://hz.ehwqpu.com/gtrhcnfgin.html

JS:   arr.length
来源：http://hz.0kj1m.cn/gthvunwxra.html

TS:   arr.length
来源：http://hz.yonumen.top/gtusggwcfh.html

Java: list.size();
来源：http://hz.jianghu66.top/gtjudshhzu.html

Go:   len(arr)
来源：http://hz.mhx1999.top/gtmoofwhhv.html

Ruby: arr.length; arr.size
来源：http://hz.guannengcc.top/gtltdyzipq.html

C#:   list.Count;
来源：http://hz.redwolf501.top/gtizbeuvec.html

[D07] 切片 / 取子数组
来源：http://hz.cucudq.cn/gtyjiaptas.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.birdmap.top/gtcvynvnqm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.vqdsnc.cn/gtbjfnajsf.html

JS:   arr.slice(1, 4);
来源：http://hz.shzxlz.cn/gtpjvbfzmk.html

TS:   arr.slice(1, 4);
来源：http://hz.ydjk.org.cn/gtcjzzvbxw.html

Java: list.subList(1, 4);
来源：http://hz.sweek.top/gtoxjithdz.html

Go:   arr[1:4]
来源：http://hz.zhaomingkeji.xyz/gttebivost.html

Ruby: arr[1, 3]
来源：http://hz.ppjwa.cn/gtpgdbugcl.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhaomingkeji.xyz/gtkqxalmem.html

[D08] 合并两个数组
来源：http://hz.xinyue.icu/gtxqsxrtel.html

Py:   a + b;  a.extend(b)
来源：http://hz.hysaishi.cn/gtoaupkdpl.html

PHP:  array_merge($a, $b);
来源：http://hz.aibaodan.cn/gtxrwwqgym.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.aibaodan.cn/gtapqfvzbr.html

TS:   [...a, ...b];
来源：http://hz.yj20258.top/gtsyzjksvj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shuidangran.top/gttjhnzjlc.html

Go:   append(a, b...)
来源：http://hz.hywenlv.cn/gtnqjnojdo.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhaomingkeji.xyz/gtdgaucacm.html

C#:   a.Concat(b).ToList()
来源：http://hz.hywenlv.cn/gtjzpzragy.html

[D09] 排序（升序）
来源：http://hz.0kj1m.cn/gtxhtgwyep.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nwbrower.top/gtfvulzrmt.html

PHP:  sort($arr);
来源：http://hz.hnxiangtu.top/gtqrazwnvq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.fzhhl.top/gtoqaluhar.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jianghu66.top/gtyzkfwajm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.52xcode.cn/gtmhiayikr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.pengpengdd.cyou/gtxkidocoh.html

Ruby: arr.sort
来源：http://hz.ydzc1.top/gtennrasuq.html

C#:   list.Sort();
来源：http://hz.yuxming.cn/gteaguwkli.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ydzc1.top/gtxbzcxqvz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zycfv.cn/gtkmoixhmy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.snrcjt.cn/gtookgesqc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daxiang520.top/gtsijftrss.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yonumen.top/gtmxifbvjl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.aibaodan.cn/gtbetqnwgv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.aibaodan.cn/gtmprowiov.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.havefunace.top/gtpohiodti.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.sxryk.cn/gtnrtiuulj.html

[D11] 反转数组
来源：http://hz.zhiwuduotai.top/gtceikusob.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hysaishi.cn/gtoazmbxfj.html

PHP:  array_reverse($arr);
来源：http://hz.sufxvd.cn/gtfcdybkpw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shanyushiyangkeji.top/gtqzkvnhlo.html

TS:   [...arr].reverse();
来源：http://hz.gogol.net.cn/gtujcmwdjc.html

Java: Collections.reverse(list);
来源：http://hz.yuxming.cn/gtgmdzpyar.html

Go:   slices.Reverse(arr)
来源：http://hz.yanxiufei.cn/gtasrvcipk.html

Ruby: arr.reverse
来源：http://hz.hnqzz.top/gtnbubjdqb.html

C#:   list.Reverse();
来源：http://hz.yanxiufei.cn/gtfuimqnse.html

[D12] 查找元素下标
来源：http://hz.zhixingplan.top/gtaletnbbv.html

Py:   arr.index(x);  x in arr
来源：http://hz.tian-w.cn/gtgoamddxo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shanyushiyangtech.top/gtjshhebat.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sysykeji.top/gtuyspxszv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pengpengdd.cyou/gtcfrsoqsx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yuxming.cn/gtanyrsfcw.html

Go:   slices.Index(arr, x)
来源：http://hz.shanyushiyangtech.top/gtzqxpxivq.html

Ruby: arr.index(x)
来源：http://hz.feifeiyinyue.top/gtcgxmktic.html

C#:   list.IndexOf(x);
来源：http://hz.kuanghao11.cn/gtflcujpyp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xuetiantiany.cn/gtmqvbexzy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jyoumei.cn/gtglvcahdb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xuanzx.com/gtppiryejs.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yuxming.cn/gtirokcria.html

TS:   arr.filter(x => x > 3)
来源：http://hz.andypj.xyz/gtjsoumroz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.daxiang520.top/gtcsvziryr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.feifeiyinyue.top/gtsjvswmbz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.guannengcc.top/gtufypgmfv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.haohaochexian.top/gtjpgkvskh.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ybcxt.top/gtyrkqzesg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jianghu66.top/gtxjdhtpsu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yj20258.top/gtuugehnzs.html

JS:   arr.map(x => x * 2)
来源：http://hz.ydzc1.top/gtzsnvjzwv.html

TS:   arr.map(x => x * 2)
来源：http://hz.c1oappe.top/gtrhsujzif.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ehwqpu.com/gtmicvjmft.html

Go:   // 手写循环
来源：http://hz.ehwqpu.com/gthxrgnmtr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jlsjyb.cn/gtommpkrnn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hysaishi.cn/gtwalzzird.html

[D15] 去重
来源：http://hz.ydzc1.top/gtqoxzpfwd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.guannengcc.top/gtnxpwgvak.html

PHP:  array_unique($arr);
来源：http://hz.xingfuxueyuan.xyz/gtjomiwmit.html

JS:   [...new Set(arr)]
来源：http://hz.xziqi.cn/gtfpchbqsn.html

TS:   [...new Set(arr)]
来源：http://hz.c1oappe.top/gthpaggmoe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.pycfn.com/gtanlrxmef.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yj202588.top/gtjmalvyva.html

Ruby: arr.uniq
来源：http://hz.yueranfly.top/gtlmybvunv.html

C#:   list.Distinct().ToList()
来源：http://hz.chenjidiqi.icu/gtquvdhbgz.html

[D16] 求和与平均值
来源：http://hz.tianlin.xyz/gtwwaxzazu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yanxiufei.cn/gteaqadcpk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hnxiangtu.top/gteulimcgm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtradznjlx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenzaomai.com/gtrdlizkub.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.tian-w.cn/gtookzlayo.html

Go:   // 手写循环累加
来源：http://hz.zdqjudy.top/gtfvxdhsbj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.guannengcc.top/gtupgfuoie.html

C#:   list.Sum();  list.Average()
来源：http://hz.sweek.top/gtbaeiqofd.html

[D17] 最大值与最小值
来源：http://hz.zhijiandao.cn/gtwcuwthxx.html

Py:   max(arr);  min(arr)
来源：http://hz.xingfuxueyuan.xyz/gtapqnsisa.html

PHP:  max($arr);  min($arr);
来源：http://hz.pycfn.com/gttbamwzhq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.redwolf501.top/gtedufnqjs.html

TS:   Math.max(...arr);
来源：http://hz.zhiwuduotai.top/gthozvgbgv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.aibaodan.cn/gtsqzfeeov.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.birdmap.top/gtxrfxjvis.html

Ruby: arr.max;  arr.min
来源：http://hz.wangshuangyany.cn/gtezqbefha.html

C#:   list.Max();  list.Min()
来源：http://hz.yangfankeji.com/gtzxnxpvsu.html

[D18] 扁平化嵌套数组
来源：http://hz.nanxinkj.top/gtewkrcgwa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ivvv.top/gtpvgapqil.html

PHP:  array_merge(...$nested);
来源：http://hz.yuanzhike.top/gtyiijowyi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ivvv.top/gtpsvhqyog.html

TS:   nested.flat();
来源：http://hz.shangyingyoupin.top/gthvffjoyy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.guowangkeji.top/gtwguoceld.html

Go:   // 手写双层循环
来源：http://hz.bjfxy.top/gtyycpwcjt.html

Ruby: nested.flatten
来源：http://hz.sysykeji.top/gtatrxojox.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.meibo888.top/gtrsxxulby.html

[D19] 按字段分组
来源：http://hz.aibaodan.cn/gtocernnzb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.nwbrower.top/gthtfdqrjw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.daxiang520.top/gtzqjtitcy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jyoumei.cn/gtchtkqwrj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.guannengcc.top/gtgpsqmtis.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gaohongyu789.top/gtubzwrajy.html

Go:   // 手写 map[string][]T
来源：http://hz.shzxlz.cn/gtlrfgfowi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhongyouzk.top/gttqdsqkvg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.fzhhl.top/gtehxkfqfs.html

[D20] 统计每个元素出现次数
来源：http://hz.wangdashe.top/gtjacfvyjq.html

Py:   Counter(arr)
来源：http://hz.guannengcc.top/gthiuwvibv.html

PHP:  array_count_values($arr);
来源：http://hz.sysykeji.top/gtjndrypiz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ybcxt.top/gtjrivmdjj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258.top/gtenkvfliu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.c1oappe.top/gtdmkltajt.html

Go:   // 手写 map[T]int
来源：http://hz.ivvv.top/gtwmjeegyk.html

Ruby: arr.tally
来源：http://hz.xuetiantiany.cn/gtevxdyilo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhoulong.xyz/gtquamemls.html

[D21] 判断是否包含某元素
来源：http://hz.shanyushiyangkeji.top/gtolojxxtz.html

Py:   x in arr
来源：http://hz.nanxinkj.top/gtjfcfcefs.html

PHP:  in_array($x, $arr, true);
来源：http://hz.0kj1m.cn/gtgykyayys.html

JS:   arr.includes(x)
来源：http://hz.zhixingplan.top/gtqsmrtuhw.html

TS:   arr.includes(x)
来源：http://hz.jyoumei.cn/gtaeowciyi.html

Java: list.contains(x)
来源：http://hz.xylfe.cn/gtflkomgpp.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuanzhike.top/gtqxdcbvhe.html

Ruby: arr.include?(x)
来源：http://hz.shzxlz.cn/gtonjotzus.html

C#:   list.Contains(x)
来源：http://hz.yongpay.top/gtmqvrpubf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hongshengwenyu.top/gtswevxpny.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yuxming.cn/gtyylgzerl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hnqzz.top/gtjfqrbpfd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenzaomai.com/gtiwgreery.html

TS:   [...arr];
来源：http://hz.sweek.top/gtptyvqpga.html

Java: new ArrayList<>(list);
来源：http://hz.zhiwuduotai.top/gtdqtpgcer.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhaomingkeji.xyz/gtszpqgkvt.html

Ruby: arr.dup;  arr.clone
来源：http://hz.dianchejie.cn/gtybrbygbh.html

C#:   new List<int>(list);
来源：http://hz.yvedp.cn/gtjxmanwui.html

[D23] reduce 累积计算
来源：http://hz.jinghuilouyu.cn/gtpprwqdch.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.mhx1999.top/gtziybneyr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.daria6918.cn/gtoxrivucx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.kuanghao11.cn/gtjkfeuqxp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.mhx1999.top/gtrzphtlqz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xingfuxueyuan.xyz/gtrftadfuk.html

Go:   // 手写循环
来源：http://hz.sysykeji.top/gtyyryhqvl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.iojbl.cn/gtglleobzh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shanyushiyangtech.top/gthrpacjaj.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinghuilouyu.cn/gtxemqgglt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gaohongyu789.top/gtlykgtssc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.quarkkingdee.top/gtqhterrou.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.mhx1999.top/gtpvzjhnnj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xylfe.cn/gtatzahqqo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yj20258888.top/gtniqzdwht.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ivvv.top/gtuprqguyo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xuanzx.com/gtuawugmnv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ybcxt.top/gtdjttkusj.html

[D25] Set 集合去重与交并差
来源：http://hz.gzhubu.top/gtcqtbmunz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.daria6918.cn/gthjaoeimp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nwbrower.top/gtxwuzyotv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jianghu66.top/gtrfdhruij.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sysykeji.top/gtxjgjvozw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cucudq.cn/gtfwyazelp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.svipenyu.cn/gtqakwugug.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.feifeiyinyue.top/gtdnlpenvl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.pycfn.com/gtptwofsds.html

[D26] 数组转字符串
来源：http://hz.jinqigufen.top/gtryyiumov.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yanxiufei.cn/gtphqskchz.html

PHP:  implode(", ", $arr);
来源：http://hz.guannengcc.top/gtkdrxjddf.html

JS:   arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtaossocpd.html

TS:   arr.join(", ")
来源：http://hz.fengsongda.top/gtjfqwqlay.html

Java: String.join(", ", list)
来源：http://hz.zhengqikj.top/gthcllxssf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yongpay.top/gtvyilhpdr.html

Ruby: arr.join(", ")
来源：http://hz.cdnleiting.top/gtautyhgsi.html

C#:   string.Join(", ", list)
来源：http://hz.jqgfzy.top/gteuzmkpif.html

================================================================================
来源：http://hz.gotoacloud.top/gtqpaofvmf.html

E. 字符串处理
来源：http://hz.gotoacloud.top/gtdgzepfgh.html

================================================================================
来源：http://hz.xylfe.cn/gtqzvisiki.html

[E01] 拼接字符串
来源：http://hz.vqdsnc.cn/gtwjvfjcsf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.havefunace.top/gthjoqxgno.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yuxming.cn/gtsyygrxsp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhiwuduotai.top/gtmtznyvfv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigufen.top/gtuoxdumkp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.snrcjt.cn/gtvkuwbhkr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenjidiqi.icu/gtyddxdwbw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jqgfzy.top/gtrrxasqxf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yanxiufei.cn/gtsloqzdkt.html

[E02] 重复字符串
来源：http://hz.xziqi.cn/gtxuejegze.html

Py:   "ab" * 3
来源：http://hz.fzhhl.top/gthyseznrx.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinyuanbaomall.cn/gtxjrxtylg.html

JS:   "ab".repeat(3)
来源：http://hz.daxiang520.top/gtqhxzexgh.html

TS:   "ab".repeat(3)
来源：http://hz.xinyue.icu/gtlrobhmjw.html

Java: "ab".repeat(3)
来源：http://hz.xylfe.cn/gthkrnyekc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxuanxn.top/gtctsoeges.html

Ruby: "ab" * 3
来源：http://hz.jianghu66.top/gtnsghhpqa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinghuilouyu.cn/gtibabthwx.html

[E03] 截取子串
来源：http://hz.zdqjudy.top/gtdlncohje.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.shzxlz.cn/gtaasdetst.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.smart0.xyz/gtuksikjqs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.fengsongda.top/gtxhiqlzgu.html

TS:   s.slice(1, 4)
来源：http://hz.guowangkeji.top/gtnmexdkzt.html

Java: s.substring(1, 4)
来源：http://hz.hywenlv.cn/gtydgrifya.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hnqzz.top/gtohunrhzr.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.sufxvd.cn/gttvadudtl.html

C#:   s.Substring(1, 3)
来源：http://hz.iojbl.cn/gtujasxzuu.html

[E04] 查找子串位置
来源：http://hz.jyoumei.cn/gtxhaiarjz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.daria6918.cn/gtrqevjndw.html

PHP:  strpos($s, "x");
来源：http://hz.cqqwz.cn/gtsarfarvl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shuidangran.top/gthtkntesg.html

TS:   s.indexOf("x")
来源：http://hz.316326.xyz/gtvuenwsvz.html

Java: s.indexOf("x")
来源：http://hz.vqdsnc.cn/gtbtizqnya.html

Go:   strings.Index(s, "x")
来源：http://hz.9152youxi.cn/gtfqkinabo.html

Ruby: s.index("x")
来源：http://hz.xziqi.cn/gthzqstaha.html

C#:   s.IndexOf("x")
来源：http://hz.ppjwa.cn/gtdogjhupj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.pycfn.com/gtxkwbiaeu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hysaishi.cn/gtftuxrgqc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinyuanbaomall.cn/gtrzrjaern.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.snrcjt.cn/gtixuhlbiq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cashguo.top/gtfbndeppe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinghuilouyu.cn/gthlbtdnge.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ehwqpu.com/gtbkrkrbjb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hysaishi.cn/gtwuuznefb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinqigfzy.top/gtikljikqy.html


<!-- 参考信息 -->