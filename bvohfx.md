代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nwbrower.top/gtvfultkhv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.kuanghao11.cn/gtgbmzyvqb.html

Java: // 无解构
来源：http://hz.chenlongwang.top/gtnhbsmgzg.html

Go:   // 无解构
来源：http://hz.jianghu66.top/gtqfngywql.html

Ruby: a, b = pair
来源：http://hz.yj202588.top/gtazcoylde.html

C#:   var (a, b) = pair;
来源：http://hz.shzxlz.cn/gtujytxpzo.html

[C16] 函数 / 方法重载
来源：http://hz.ywan-chungtsiang.top/gtnaklimsu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yueranfly.top/gtitwfrsjs.html

PHP:  // 无重载
来源：http://hz.yangfankeji.com/gtzpfocias.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hongshengwenyu.top/gtuotougbf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sufxvd.cn/gtlboozank.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinyuanbaomall.cn/gterrtdsjc.html

Go:   // 无重载：用不同函数名
来源：http://hz.havefunace.top/gtxbnvjjvj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhoulong.xyz/gtvbxflesg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenzaomai.com/gtflurcsnz.html

================================================================================
来源：http://hz.xziqi.cn/gtsuptaujr.html

D. 数组 / 列表 / 集合
来源：http://hz.haohaochexian.top/gtdrtinoaa.html

================================================================================
来源：http://hz.haohaochexian.top/gtpgtxfrwi.html

[D01] 创建数组 / 列表
来源：http://hz.tian-w.cn/gtcuppoyhu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.guowangkeji.top/gtmvrogyrz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhiwuduotai.top/gtbnlyirpc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sweek.top/gtrpfawvxt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.nanxuanxn.top/gtpgietvpx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jiagoushi.top/gtfzderdtg.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hnxiangtu.top/gtqtzouiuk.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xingfuxueyuan.xyz/gtiellwpzy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhoulong.xyz/gtaqpfoxjc.html

[D02] 追加元素到末尾
来源：http://hz.cdnleiting.top/gtqsyihaoc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yuxming.cn/gtbauiklpd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jqgufenzy.top/gtxpsgzcnj.html

JS:   arr.push(4);
来源：http://hz.zhengqikj.top/gtqgjtbugr.html

TS:   arr.push(4);
来源：http://hz.zhijiandao.cn/gtvctfhkug.html

Java: list.add(4);
来源：http://hz.c1oappe.top/gtbetlmrbn.html

Go:   arr = append(arr, 4)
来源：http://hz.feifeiyinyue.top/gtorjmlmmx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.chenzaomai.com/gtwsgbqthe.html

C#:   list.Add(4);
来源：http://hz.jinyuanbaomall.cn/gtnzeuphaw.html

[D03] 在指定位置插入元素
来源：http://hz.gotoacloud.top/gtxtodjpqy.html

Py:   arr.insert(0, 0)
来源：http://hz.wangdashe.top/gtzvvojdzv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinghuilouyu.cn/gtipwmgtoe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.0kj1m.cn/gtuqmdlvbh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.fengsongda.top/gtblxadnic.html

Java: list.add(0, 0);
来源：http://hz.guowangkeji.top/gthrvewkuv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ehwqpu.com/gttiumkhte.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xinyue.icu/gtrcxybkbl.html

C#:   list.Insert(0, 0);
来源：http://hz.hywenlv.cn/gtppzwvgml.html

[D04] 删除元素
来源：http://hz.birdmap.top/gtqeifcmey.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.tianlin.xyz/gtcbmrsqbl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinghuilouyu.cn/gtpiqogukh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhijiandao.cn/gtxlczrxpn.html

TS:   arr.splice(0, 1);
来源：http://hz.shuidangran.top/gtjwntmbld.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.fzhhl.top/gtrffexcjh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yangfankeji.com/gtyntimaor.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.guannengcc.top/gtvsdzlsar.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinghuilouyu.cn/gtbvgoziza.html

[D05] 访问与修改元素
来源：http://hz.dianchejie.cn/gtlnnakxyw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zdqjudy.top/gtorgbqpek.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtivymejqp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xylfe.cn/gtuatfzjcf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sweek.top/gtkqzwecpa.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ivvv.top/gtqbzbaciw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jqgfzy.top/gthgnpspkc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtoecdkyfn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shangyingyoupin.top/gtfdzsrhlc.html

[D06] 数组长度
来源：http://hz.aizwys.cn/gtbkzptgqr.html

Py:   len(arr)
来源：http://hz.xylfe.cn/gtnaiqxpfw.html

PHP:  count($arr);
来源：http://hz.guannengcc.top/gtlqtnride.html

JS:   arr.length
来源：http://hz.dianchejie.cn/gthzddktfr.html

TS:   arr.length
来源：http://hz.fengsongda.top/gtplaergfe.html

Java: list.size();
来源：http://hz.snrcjt.cn/gtqortbcdf.html

Go:   len(arr)
来源：http://hz.feifeiyinyue.top/gthuwqtmxn.html

Ruby: arr.length; arr.size
来源：http://hz.tianlin.xyz/gtzxtoloyy.html

C#:   list.Count;
来源：http://hz.tian-w.cn/gtfjvivzjo.html

[D07] 切片 / 取子数组
来源：http://hz.andypj.xyz/gtvbqierec.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.mhx1999.top/gtwjyeuumv.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gzhubu.top/gtmcwjkzym.html

JS:   arr.slice(1, 4);
来源：http://hz.chenjidiqi.icu/gtmgtpixbo.html

TS:   arr.slice(1, 4);
来源：http://hz.zhongyouzk.top/gtrigffejj.html

Java: list.subList(1, 4);
来源：http://hz.jiagoushi.top/gtfjzzkzbf.html

Go:   arr[1:4]
来源：http://hz.xuetiantiany.cn/gtlhacqmwi.html

Ruby: arr[1, 3]
来源：http://hz.xziqi.cn/gtdiqihqww.html

C#:   list.GetRange(1, 3);
来源：http://hz.cqqwz.cn/gttbudqqvf.html

[D08] 合并两个数组
来源：http://hz.yangfankeji.com/gtzqgslfnd.html

Py:   a + b;  a.extend(b)
来源：http://hz.feifeiyinyue.top/gtzppdoyyj.html

PHP:  array_merge($a, $b);
来源：http://hz.hammf.cn/gthdtzdjyw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.0kj1m.cn/gtmrewnapj.html

TS:   [...a, ...b];
来源：http://hz.mhx1999.top/gtbugphsje.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.daria6918.cn/gteeiucdfw.html

Go:   append(a, b...)
来源：http://hz.316326.xyz/gtolurxnvf.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ywan-chungtsiang.top/gtqmpvluwl.html

C#:   a.Concat(b).ToList()
来源：http://hz.havefunace.top/gtobuaupck.html

[D09] 排序（升序）
来源：http://hz.hysaishi.cn/gtolcvvcrt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hnxiangtu.top/gtgdmhdlrj.html

PHP:  sort($arr);
来源：http://hz.zdqjudy.top/gtkmdgynvl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.haohaochexian.top/gtuducvyux.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhiwuduotai.top/gtzvdxsazg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yanxiufei.cn/gtmsqbfhez.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xingfuxueyuan.xyz/gtneftpgya.html

Ruby: arr.sort
来源：http://hz.jinyuanbaomall.cn/gtjpsiszyq.html

C#:   list.Sort();
来源：http://hz.jinqigufen.top/gtogansklx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jiagoushi.top/gtyegvkpen.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.andypj.xyz/gtsniytjxo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.feifeiyinyue.top/gtckcnnjrp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhengqikj.top/gtxpeglgvn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zycfv.cn/gthgcdmgfs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cqqwz.cn/gtdkhlqork.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.pycfn.com/gtznlxdipj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhengqikj.top/gtoxczhvyz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yonumen.top/gtnrrnxaud.html

[D11] 反转数组
来源：http://hz.zhoulong.xyz/gtnvgihtdr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yj20258888.top/gtthyqixsx.html

PHP:  array_reverse($arr);
来源：http://hz.nwbrower.top/gtfjxoveam.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yongpay.top/gtwtbyffcw.html

TS:   [...arr].reverse();
来源：http://hz.hnqzz.top/gtjvtpriez.html

Java: Collections.reverse(list);
来源：http://hz.meibo888.top/gtiupomlmz.html

Go:   slices.Reverse(arr)
来源：http://hz.daxiang520.top/gtscapzjxv.html

Ruby: arr.reverse
来源：http://hz.zhiwuduotai.top/gtvrszkiyl.html

C#:   list.Reverse();
来源：http://hz.kuanghao11.cn/gtwosbkcxv.html

[D12] 查找元素下标
来源：http://hz.ehwqpu.com/gtpnaboguk.html

Py:   arr.index(x);  x in arr
来源：http://hz.hnqzz.top/gtjoejtglb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenlongwang.top/gtbrctfdfi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ivvv.top/gtzovxyaut.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhiwuduotai.top/gtdiivssss.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hywenlv.cn/gtdcoqetrk.html

Go:   slices.Index(arr, x)
来源：http://hz.pycfn.com/gtkwtaiaok.html

Ruby: arr.index(x)
来源：http://hz.ivvv.top/gtukgksubn.html

C#:   list.IndexOf(x);
来源：http://hz.xziqi.cn/gtzootbdit.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yvedp.cn/gtowbbglby.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xziqi.cn/gtrphibtkj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gogol.net.cn/gtoiczdadj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.meibo888.top/gtfcerapzi.html

TS:   arr.filter(x => x > 3)
来源：http://hz.wangdashe.top/gtfporfriz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sufxvd.cn/gtdwbpjdfv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.9152youxi.cn/gtmaqteolr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xingfuxueyuan.xyz/gtpbmxmqyr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.gogol.net.cn/gtnuwezaig.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nanxinkj.top/gtrcmdtyij.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.nwbrower.top/gtlymxayxa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.0kj1m.cn/gtowbvpwab.html

JS:   arr.map(x => x * 2)
来源：http://hz.yvedp.cn/gtxumjpdsn.html

TS:   arr.map(x => x * 2)
来源：http://hz.sweek.top/gtyykubwfv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shanyushiyangkeji.top/gtzmsxxtrk.html

Go:   // 手写循环
来源：http://hz.hysaishi.cn/gtjyhroxyt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.svipenyu.cn/gtcexrpvke.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.nanxinkj.top/gttsqvvyxo.html

[D15] 去重
来源：http://hz.vqdsnc.cn/gteafyrfaq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sufxvd.cn/gtswarpcnk.html

PHP:  array_unique($arr);
来源：http://hz.sysykeji.top/gtjhgthgyx.html

JS:   [...new Set(arr)]
来源：http://hz.aibaodan.cn/gtvhzzdvld.html

TS:   [...new Set(arr)]
来源：http://hz.chenzaomai.com/gtxalwnims.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.haohaochexian.top/gtmraovaym.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ybcxt.top/gtzmufeazm.html

Ruby: arr.uniq
来源：http://hz.hnxiangtu.top/gtunndvccg.html

C#:   list.Distinct().ToList()
来源：http://hz.yvedp.cn/gtckyakxwg.html

[D16] 求和与平均值
来源：http://hz.birdmap.top/gttnupqspd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aizwys.cn/gtugiioplt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sufxvd.cn/gtypxinzns.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.snrcjt.cn/gtyllndzpx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnxiangtu.top/gthlbmqzmg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xziqi.cn/gtsillrkne.html

Go:   // 手写循环累加
来源：http://hz.sufxvd.cn/gtdrgoaspo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj20258888.top/gtbrjtfcbs.html

C#:   list.Sum();  list.Average()
来源：http://hz.nanxuanxn.top/gtpwrwaugi.html

[D17] 最大值与最小值
来源：http://hz.ywan-chungtsiang.top/gtubihaytk.html

Py:   max(arr);  min(arr)
来源：http://hz.sufxvd.cn/gtdapajxed.html

PHP:  max($arr);  min($arr);
来源：http://hz.ehwqpu.com/gtgimfmjlc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shanyushiyangtech.top/gtoaclcwyy.html

TS:   Math.max(...arr);
来源：http://hz.jlsjyb.cn/gtbwfzizns.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.quarkkingdee.top/gtnvkajtej.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.mhx1999.top/gtlyisihyc.html

Ruby: arr.max;  arr.min
来源：http://hz.yj20258.top/gtbjbucrom.html

C#:   list.Max();  list.Min()
来源：http://hz.cdnleiting.top/gtyewxjxjq.html

[D18] 扁平化嵌套数组
来源：http://hz.xylfe.cn/gtflvwpyxt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nanxuanxn.top/gtlenjteoy.html

PHP:  array_merge(...$nested);
来源：http://hz.jyoumei.cn/gtvdxkjnrv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.wangdashe.top/gtuvpypnfc.html

TS:   nested.flat();
来源：http://hz.shanyushiyangkeji.top/gtochchsbx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jlsjyb.cn/gtjokdjkdn.html

Go:   // 手写双层循环
来源：http://hz.ywan-chungtsiang.top/gthrekdmvv.html

Ruby: nested.flatten
来源：http://hz.wangdashe.top/gtckcxvhri.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hnqzz.top/gtaqvwqaus.html

[D19] 按字段分组
来源：http://hz.hnxiangtu.top/gtiwytxebv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jlsjyb.cn/gtxzesbkfr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ydjk.org.cn/gtkovnlnix.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhoulong.xyz/gtbcrtdxqo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigfzy.top/gtqcfwktwz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shuidangran.top/gtucyxzrdw.html

Go:   // 手写 map[string][]T
来源：http://hz.ehwqpu.com/gtevskavep.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.tian-w.cn/gtgtmrakbv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nanxinkj.top/gttuxvocjo.html

[D20] 统计每个元素出现次数
来源：http://hz.svipenyu.cn/gthglxkzlt.html

Py:   Counter(arr)
来源：http://hz.jinghuilouyu.cn/gtyudkuzhl.html

PHP:  array_count_values($arr);
来源：http://hz.daxiang520.top/gtwvujrpvx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gotoacloud.top/gtfvnheczg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnxiangtu.top/gtczcucuqs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.pengpengdd.cyou/gtssbnyzhm.html

Go:   // 手写 map[T]int
来源：http://hz.hfpthk.cn/gtrhqkvzjh.html

Ruby: arr.tally
来源：http://hz.sysykeji.top/gtyyfqnxgn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tanke756.top/gtlhcjohdh.html

[D21] 判断是否包含某元素
来源：http://hz.zhaomingkeji.xyz/gtujbhqnsi.html

Py:   x in arr
来源：http://hz.wangshuangyany.cn/gtoqjytubd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.quarkkingdee.top/gtfmtihupr.html

JS:   arr.includes(x)
来源：http://hz.cheryme.top/gtuaprbugp.html

TS:   arr.includes(x)
来源：http://hz.sufxvd.cn/gtidnkmuvf.html

Java: list.contains(x)
来源：http://hz.cdnleiting.top/gtqwjttxkl.html

Go:   slices.Contains(arr, x)
来源：http://hz.jiagoushi.top/gtlifrlqct.html

Ruby: arr.include?(x)
来源：http://hz.cqqwz.cn/gtbaeclvsr.html

C#:   list.Contains(x)
来源：http://hz.chenjidiqi.icu/gtfnpkzjxt.html

[D22] 复制数组（避免共享引用）
来源：http://hz.haohaochexian.top/gtxsrjzwum.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shzxlz.cn/gthqmfiywx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.svipenyu.cn/gthiasdsmy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.tianlin.xyz/gtatjlpcqy.html

TS:   [...arr];
来源：http://hz.52xcode.cn/gturmeuxiu.html

Java: new ArrayList<>(list);
来源：http://hz.zhijiandao.cn/gtpcubezsd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhixingplan.top/gtsdqshpfq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ivvv.top/gtuxuzifrk.html

C#:   new List<int>(list);
来源：http://hz.cdnleiting.top/gtuarjxnug.html

[D23] reduce 累积计算
来源：http://hz.wangshuangyany.cn/gtbihzudwu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cdnleiting.top/gtycdvjclz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj202588.top/gtexbkwcfv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zdqjudy.top/gtdqqyvbpd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenlongwang.top/gtpndintxq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinyuanbaomall.cn/gttgxbblfl.html

Go:   // 手写循环
来源：http://hz.yuanzhike.top/gtagokntfj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jinghuilouyu.cn/gtgokeowhm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ydjk.org.cn/gtznevgzhm.html

[D24] 字典 / Map 基本操作
来源：http://hz.iojbl.cn/gthftjjwdy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.nwbrower.top/gtxaerobzu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yuanzhike.top/gtigiyzsvr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.birdmap.top/gttuxvqidi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hammf.cn/gtvocjvqhx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.aizwys.cn/gtotzpgeqh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.feifeiyinyue.top/gtnqovezwj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ydjk.org.cn/gtkdzzjxga.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shanyushiyangkeji.top/gtwadygerx.html

[D25] Set 集合去重与交并差
来源：http://hz.yj20258888.top/gtlwzbipqq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hfpthk.cn/gtvrdtqybv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xylfe.cn/gtbvhzsvrf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yongpay.top/gteqvkrdtz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xuetiantiany.cn/gtcwkdiixd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.aizwys.cn/gtycdtzsrp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ydjk.org.cn/gtvouvtkxa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.dashuyun.cn/gtkujjulhv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.meibo888.top/gtswbdqdvt.html

[D26] 数组转字符串
来源：http://hz.yanxiufei.cn/gtnotvhcxt.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xinyue.icu/gtzdccduel.html

PHP:  implode(", ", $arr);
来源：http://hz.quarkkingdee.top/gtsogoxxmn.html

JS:   arr.join(", ")
来源：http://hz.daxiang520.top/gtemobwusn.html

TS:   arr.join(", ")
来源：http://hz.xuetiantiany.cn/gtdnuqqxpa.html

Java: String.join(", ", list)
来源：http://hz.shuidangran.top/gtuwdiezzs.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj202588.top/gtljgzjpbg.html

Ruby: arr.join(", ")
来源：http://hz.cqqwz.cn/gtznxwlqwl.html

C#:   string.Join(", ", list)
来源：http://hz.chenzaomai.com/gtfvgigpew.html

================================================================================
来源：http://hz.chenlongwang.top/gtoocfstru.html

E. 字符串处理
来源：http://hz.iojbl.cn/gtjiebbafq.html

================================================================================
来源：http://hz.zhixingplan.top/gtyigncydb.html

[E01] 拼接字符串
来源：http://hz.hnxiangtu.top/gtccohxlud.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sysykeji.top/gthndpayxo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yuanzhike.top/gtobfjvshy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.0kj1m.cn/gtobxgesiu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yangfankeji.com/gtxwghlfyu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenjidiqi.icu/gtupvusmun.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xingfuxueyuan.xyz/gtxsxcnwrm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.redwolf501.top/gtmiexgblv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zdqjudy.top/gteyrayjap.html

[E02] 重复字符串
来源：http://hz.quarkkingdee.top/gtkhoovvzf.html

Py:   "ab" * 3
来源：http://hz.xziqi.cn/gtzhulgghv.html

PHP:  str_repeat("ab", 3);
来源：http://hz.mhx1999.top/gtboreqnzw.html

JS:   "ab".repeat(3)
来源：http://hz.shzxlz.cn/gtlezwomdc.html

TS:   "ab".repeat(3)
来源：http://hz.fzhhl.top/gtcsmsejwj.html

Java: "ab".repeat(3)
来源：http://hz.yj202588.top/gtuknruojh.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.tianlin.xyz/gthrifljkz.html

Ruby: "ab" * 3
来源：http://hz.jinqigfzy.top/gtyjbfgtzk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.redwolf501.top/gtnwekjasb.html

[E03] 截取子串
来源：http://hz.gogol.net.cn/gtdjofaxdb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ydzc1.top/gtidcfzqbe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hfpthk.cn/gtjqjwlzni.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.andypj.xyz/gtvrrgjdgj.html

TS:   s.slice(1, 4)
来源：http://hz.gogol.net.cn/gtaorgflmn.html

Java: s.substring(1, 4)
来源：http://hz.ivvv.top/gtysotoain.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yongpay.top/gtfovaztcf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenlongwang.top/gtbteokpqb.html

C#:   s.Substring(1, 3)
来源：http://hz.yueranfly.top/gtrexpppel.html

[E04] 查找子串位置
来源：http://hz.nanxuanxn.top/gtdwbraekg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tian-w.cn/gtwzyqfjgw.html

PHP:  strpos($s, "x");
来源：http://hz.chenlongwang.top/gtvfptrhvr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhengqikj.top/gtvbvxupir.html

TS:   s.indexOf("x")
来源：http://hz.shzxlz.cn/gttnroycvy.html

Java: s.indexOf("x")
来源：http://hz.yj20258.top/gtzmobxbtj.html

Go:   strings.Index(s, "x")
来源：http://hz.xziqi.cn/gtiowohgqp.html

Ruby: s.index("x")
来源：http://hz.jianghu66.top/gtwmrleajk.html

C#:   s.IndexOf("x")
来源：http://hz.ydzc1.top/gtekocysas.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.quarkkingdee.top/gtecwquqkq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.316326.xyz/gtkfsiprby.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.andypj.xyz/gtwyqaircv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xuanzx.com/gthtyvlrqb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gogol.net.cn/gtpdkqyjkj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.guowangkeji.top/gtebqvqepp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.snrcjt.cn/gtlutwkorr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sxryk.cn/gtkhrdzmjx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.guowangkeji.top/gtfiwzfvnb.html


<!-- 参考信息 -->