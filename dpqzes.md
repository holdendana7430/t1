代发 wailian999

Ruby: a, b = pair
来源：http://hz.fzhhl.top/gtztusjnwx.html

C#:   var (a, b) = pair;
来源：http://hz.andypj.xyz/gtcgbfmklt.html

[C16] 函数 / 方法重载
来源：http://hz.tian-w.cn/gtyzhuspxh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gaohongyu789.top/gtfocofxxj.html

PHP:  // 无重载
来源：http://hz.xuanzx.com/gtauscabto.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigufen.top/gtkmpqctuj.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shanyushiyangtech.top/gtlybumfik.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yuanzhike.top/gtvslhiuil.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhengqikj.top/gtgoexbyvg.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhijiandao.cn/gtrmvgefoa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhiwuduotai.top/gtevhsitiq.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtbhyiwtum.html

D. 数组 / 列表 / 集合
来源：http://hz.guowangkeji.top/gtszcivddo.html

================================================================================
来源：http://hz.pengpengdd.cyou/gthdeyurai.html

[D01] 创建数组 / 列表
来源：http://hz.pycfn.com/gtdeqwmkpx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yuanzhike.top/gtbvcrorri.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yj20258.top/gtzqrmcxmf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yueranfly.top/gtqoftfnqz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jqgufenzy.top/gtfngcugfl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cheryme.top/gtguxsekfl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ivvv.top/gtjssnwaxa.html

Ruby: arr = [1, 2, 3]
来源：http://hz.snrcjt.cn/gtcjlywqbu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhengqikj.top/gtswqwujzi.html

[D02] 追加元素到末尾
来源：http://hz.nanxinkj.top/gtrkzcpboy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xylfe.cn/gtcugjydnk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shzxlz.cn/gtbayxvdbj.html

JS:   arr.push(4);
来源：http://hz.zhongyouzk.top/gtrxiawqhu.html

TS:   arr.push(4);
来源：http://hz.yueranfly.top/gtqoxunglc.html

Java: list.add(4);
来源：http://hz.shangyingyoupin.top/gtyokevgmc.html

Go:   arr = append(arr, 4)
来源：http://hz.zhiwuduotai.top/gtwvunmgcd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cashguo.top/gttuxitpdt.html

C#:   list.Add(4);
来源：http://hz.wangdashe.top/gtwliryecj.html

[D03] 在指定位置插入元素
来源：http://hz.shangyingyoupin.top/gttqjexddz.html

Py:   arr.insert(0, 0)
来源：http://hz.jiagoushi.top/gtvjlvpizw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhaomingkeji.xyz/gtqvldtoca.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.aibaodan.cn/gtqvvskfzd.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhiwuduotai.top/gtnbrkgdrr.html

Java: list.add(0, 0);
来源：http://hz.zhiwuduotai.top/gtfmrythdy.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.svipenyu.cn/gtxudswheg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gzhubu.top/gtyuexldpn.html

C#:   list.Insert(0, 0);
来源：http://hz.zdqjudy.top/gteudunsuf.html

[D04] 删除元素
来源：http://hz.tianlin.xyz/gtcietclbf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.dianchejie.cn/gtalcpaztc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jyoumei.cn/gtspwemxrh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.birdmap.top/gtqphplvul.html

TS:   arr.splice(0, 1);
来源：http://hz.ydzc1.top/gtajzkrmth.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.nanxuanxn.top/gtzwxffagd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.iojbl.cn/gtiskpalbe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zdqjudy.top/gtmzahmjgg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xuetiantiany.cn/gthnghfurn.html

[D05] 访问与修改元素
来源：http://hz.daria6918.cn/gttyovxgtt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tian-w.cn/gtfaajmibk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ybcxt.top/gtzvlpyvee.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.dianchejie.cn/gtivqntfff.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yvedp.cn/gtfdekhkru.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jyoumei.cn/gtvekmyjsd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yangfankeji.com/gtimochspq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhixingplan.top/gtxhhokwmu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yj20258888.top/gtjvlrpvhb.html

[D06] 数组长度
来源：http://hz.guowangkeji.top/gtzuwprszm.html

Py:   len(arr)
来源：http://hz.hongshengwenyu.top/gthcxuiaih.html

PHP:  count($arr);
来源：http://hz.sweek.top/gtmciwpqzi.html

JS:   arr.length
来源：http://hz.ydzc1.top/gtgbenuvmt.html

TS:   arr.length
来源：http://hz.pycfn.com/gtmonllely.html

Java: list.size();
来源：http://hz.hysaishi.cn/gtrmnnwrkn.html

Go:   len(arr)
来源：http://hz.chenjidiqi.icu/gtycdjlajm.html

Ruby: arr.length; arr.size
来源：http://hz.yanxiufei.cn/gtltzuvguj.html

C#:   list.Count;
来源：http://hz.vqdsnc.cn/gtyabceada.html

[D07] 切片 / 取子数组
来源：http://hz.haohaochexian.top/gtaqijhzhs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ydjk.org.cn/gtiaersdyx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhiwuduotai.top/gtjbtlqtdt.html

JS:   arr.slice(1, 4);
来源：http://hz.ybcxt.top/gtsgztsodq.html

TS:   arr.slice(1, 4);
来源：http://hz.gotoacloud.top/gtzturadcf.html

Java: list.subList(1, 4);
来源：http://hz.nanxinkj.top/gtcdpbyijb.html

Go:   arr[1:4]
来源：http://hz.yj202588.top/gtvouvkhfb.html

Ruby: arr[1, 3]
来源：http://hz.chenzaomai.com/gtfeyzngoh.html

C#:   list.GetRange(1, 3);
来源：http://hz.kuanghao11.cn/gtbjbbkwhl.html

[D08] 合并两个数组
来源：http://hz.jinqigfzy.top/gttfhsytee.html

Py:   a + b;  a.extend(b)
来源：http://hz.tian-w.cn/gtoktnzpob.html

PHP:  array_merge($a, $b);
来源：http://hz.jlsjyb.cn/gtkzlgrgsu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhixingplan.top/gtqsxfmcwq.html

TS:   [...a, ...b];
来源：http://hz.xinyue.icu/gtgyhzrosa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hywenlv.cn/gtechzvmpb.html

Go:   append(a, b...)
来源：http://hz.snrcjt.cn/gtlmumhpqn.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ivvv.top/gtvvqvzpee.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinghuilouyu.cn/gttpqpglpg.html

[D09] 排序（升序）
来源：http://hz.hfpthk.cn/gtcjmnpfmw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fzhhl.top/gtjfjelisq.html

PHP:  sort($arr);
来源：http://hz.hysaishi.cn/gtdwpfcyrl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.nanxinkj.top/gtxqjbjsar.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.316326.xyz/gthfhklpkm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhongyouzk.top/gtlqrkcxnl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jiagoushi.top/gtnpvrffym.html

Ruby: arr.sort
来源：http://hz.gzhubu.top/gtagswcrih.html

C#:   list.Sort();
来源：http://hz.xuetiantiany.cn/gtsfbapxmw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ehwqpu.com/gtlhtdhtlw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenzaomai.com/gtqkrndkbh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxuanxn.top/gtrzqiurbl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sweek.top/gtwmmpcbtz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gtlqmwhyyb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.pengpengdd.cyou/gtsdlsygyp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yangfankeji.com/gtqlmnfwby.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.vqdsnc.cn/gtoltdiqjn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.daxiang520.top/gtczcsvack.html

[D11] 反转数组
来源：http://hz.c1oappe.top/gtkqgwdexu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hnxiangtu.top/gtpyvkxppi.html

PHP:  array_reverse($arr);
来源：http://hz.jinghuilouyu.cn/gtmflxqcbb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.guannengcc.top/gtdqsmqgrj.html

TS:   [...arr].reverse();
来源：http://hz.xinyue.icu/gtkljomxiz.html

Java: Collections.reverse(list);
来源：http://hz.ybcxt.top/gtyakpymlt.html

Go:   slices.Reverse(arr)
来源：http://hz.zhongyouzk.top/gtrrikdanw.html

Ruby: arr.reverse
来源：http://hz.jyoumei.cn/gtjjlbunmi.html

C#:   list.Reverse();
来源：http://hz.nanxinkj.top/gtethfgxxp.html

[D12] 查找元素下标
来源：http://hz.shanyushiyangtech.top/gtvmbeihze.html

Py:   arr.index(x);  x in arr
来源：http://hz.svipenyu.cn/gtimlzrwnx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.bjfxy.top/gtwbeqzprj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigfzy.top/gtyaidcaqh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xylfe.cn/gtrpfitckr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.316326.xyz/gtvdlquvwl.html

Go:   slices.Index(arr, x)
来源：http://hz.52xcode.cn/gtjvyqzlnq.html

Ruby: arr.index(x)
来源：http://hz.andypj.xyz/gtsdkgksfx.html

C#:   list.IndexOf(x);
来源：http://hz.gaohongyu789.top/gtecnipiru.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gzhubu.top/gttppnhagm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.tianlin.xyz/gtfzmvrevz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhongyouzk.top/gtpuxbjzsa.html

JS:   arr.filter(x => x > 3)
来源：http://hz.9152youxi.cn/gtpvwpiwur.html

TS:   arr.filter(x => x > 3)
来源：http://hz.aibaodan.cn/gtyunfclgp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.haohaochexian.top/gtdmktphej.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.9152youxi.cn/gtarzqydjy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.cucudq.cn/gttoujmfzm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.birdmap.top/gtqnquwifr.html

[D14] 映射转换（每个元素变形）
来源：http://hz.316326.xyz/gtfnotuqis.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ybcxt.top/gtathrcqkf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sweek.top/gtcvibhcus.html

JS:   arr.map(x => x * 2)
来源：http://hz.feifeiyinyue.top/gtqthvbpbg.html

TS:   arr.map(x => x * 2)
来源：http://hz.yuxming.cn/gtnaeboedz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ydjk.org.cn/gtkxajazav.html

Go:   // 手写循环
来源：http://hz.gogol.net.cn/gtugzvoaeb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.tianlin.xyz/gtsxzswksl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jyoumei.cn/gtlexngepx.html

[D15] 去重
来源：http://hz.zhongyouzk.top/gteikhfhxu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yueranfly.top/gtdbctgkim.html

PHP:  array_unique($arr);
来源：http://hz.jyoumei.cn/gtxqyaqyit.html

JS:   [...new Set(arr)]
来源：http://hz.sufxvd.cn/gtvpqmtpys.html

TS:   [...new Set(arr)]
来源：http://hz.bjfxy.top/gtwzbivzxg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ybcxt.top/gtzwrimqtr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinyuanbaomall.cn/gtbpxaywdv.html

Ruby: arr.uniq
来源：http://hz.yvedp.cn/gtrypgchap.html

C#:   list.Distinct().ToList()
来源：http://hz.hywenlv.cn/gtwditwldi.html

[D16] 求和与平均值
来源：http://hz.jlsjyb.cn/gtmmontboc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aibaodan.cn/gtxbmlaycr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.guannengcc.top/gtsdxxklrp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cheryme.top/gtufqbhwjp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gogol.net.cn/gttaafruuy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.pengpengdd.cyou/gtjmbrtalu.html

Go:   // 手写循环累加
来源：http://hz.xziqi.cn/gtqfrvqibp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhiwuduotai.top/gtdsiyosoi.html

C#:   list.Sum();  list.Average()
来源：http://hz.xziqi.cn/gtebjiliaq.html

[D17] 最大值与最小值
来源：http://hz.ywan-chungtsiang.top/gtqlauxtsi.html

Py:   max(arr);  min(arr)
来源：http://hz.jqgufenzy.top/gtpmlrsffc.html

PHP:  max($arr);  min($arr);
来源：http://hz.52xcode.cn/gtouiclswt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jqgufenzy.top/gtuegntgbb.html

TS:   Math.max(...arr);
来源：http://hz.yangfankeji.com/gtwgkjfsun.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhoulong.xyz/gtaojwnsek.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinghuilouyu.cn/gtpbturvpu.html

Ruby: arr.max;  arr.min
来源：http://hz.dashuyun.cn/gtwbqlbzqk.html

C#:   list.Max();  list.Min()
来源：http://hz.snrcjt.cn/gtsuazyexb.html

[D18] 扁平化嵌套数组
来源：http://hz.yj20258888.top/gtqayuzqnb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.tianlin.xyz/gtccbyobkx.html

PHP:  array_merge(...$nested);
来源：http://hz.xylfe.cn/gtvdvwprct.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hysaishi.cn/gtawthnmjd.html

TS:   nested.flat();
来源：http://hz.ppjwa.cn/gtkhymswyf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jlsjyb.cn/gtdlrspuoz.html

Go:   // 手写双层循环
来源：http://hz.ehwqpu.com/gtklftasyi.html

Ruby: nested.flatten
来源：http://hz.cashguo.top/gtvprbpnmd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.smart0.xyz/gtfcuatgjl.html

[D19] 按字段分组
来源：http://hz.feifeiyinyue.top/gtrlzbphwk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cashguo.top/gtxqhuvpxu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.mhx1999.top/gtyelkwsew.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.birdmap.top/gtiuqfmspr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.guowangkeji.top/gtksdsmboe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.meibo888.top/gtghfydyku.html

Go:   // 手写 map[string][]T
来源：http://hz.aibaodan.cn/gtvmncrsjj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhengqikj.top/gtbeeoqkeh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.snrcjt.cn/gtmdhajulj.html

[D20] 统计每个元素出现次数
来源：http://hz.yuanzhike.top/gthqqdvjtg.html

Py:   Counter(arr)
来源：http://hz.zhongyouzk.top/gtxlqugyqk.html

PHP:  array_count_values($arr);
来源：http://hz.tanke756.top/gthquqffqo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dianchejie.cn/gtxicbljmn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangshuangyany.cn/gtgdupfwgn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zycfv.cn/gtjjqwpcqb.html

Go:   // 手写 map[T]int
来源：http://hz.fengsongda.top/gthbccoalb.html

Ruby: arr.tally
来源：http://hz.iojbl.cn/gtmkflacfg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.vqdsnc.cn/gtriycdycs.html

[D21] 判断是否包含某元素
来源：http://hz.xuanzx.com/gthgylrbep.html

Py:   x in arr
来源：http://hz.jiagoushi.top/gtkookvshn.html

PHP:  in_array($x, $arr, true);
来源：http://hz.smart0.xyz/gtceaoaclw.html

JS:   arr.includes(x)
来源：http://hz.jinqigfzy.top/gtcmuvihio.html

TS:   arr.includes(x)
来源：http://hz.guannengcc.top/gtoyccxqpe.html

Java: list.contains(x)
来源：http://hz.zhixingplan.top/gttmwleghp.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj20258888.top/gtrqhjnwiv.html

Ruby: arr.include?(x)
来源：http://hz.yuanzhike.top/gtwcuwqkmu.html

C#:   list.Contains(x)
来源：http://hz.cqqwz.cn/gtdgythxhd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.pengpengdd.cyou/gtqckxiyae.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxinkj.top/gtzkeirhjy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cheryme.top/gtyxlgttpx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yj20258.top/gtnadckkoe.html

TS:   [...arr];
来源：http://hz.sysykeji.top/gtwadlikih.html

Java: new ArrayList<>(list);
来源：http://hz.feifeiyinyue.top/gtxryvzqyy.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenlongwang.top/gtkdyzzwey.html

Ruby: arr.dup;  arr.clone
来源：http://hz.havefunace.top/gtmrfbnytn.html

C#:   new List<int>(list);
来源：http://hz.zhixingplan.top/gtrgpstzxn.html

[D23] reduce 累积计算
来源：http://hz.xuetiantiany.cn/gtefthtbcs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.mhx1999.top/gtfbyhoumt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.quarkkingdee.top/gtrfakqjbv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fzhhl.top/gtyrvpxnog.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yangfankeji.com/gthnlhwrxs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xinyue.icu/gtlfazbnrg.html

Go:   // 手写循环
来源：http://hz.snrcjt.cn/gtutoptuxm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.dashuyun.cn/gtuzbfawqn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.c1oappe.top/gtmalgzhiu.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj20258888.top/gtezisioas.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yangfankeji.com/gtrjpydjsr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.pengpengdd.cyou/gtytmptfbs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.fzhhl.top/gteuetaoru.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.svipenyu.cn/gtdtlgogty.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sxryk.cn/gtzjwbmlcb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.wangshuangyany.cn/gteggetwrv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ehwqpu.com/gttmouvlvc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhiwuduotai.top/gtqsejklrk.html

[D25] Set 集合去重与交并差
来源：http://hz.ydjk.org.cn/gtksvbmzks.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhixingplan.top/gtkfafmjrh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zycfv.cn/gtsrjxtczb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.bjfxy.top/gtdustutcf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cashguo.top/gtmocvjkim.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.andypj.xyz/gtgrdqahjt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.svipenyu.cn/gtuzoojjvh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.52xcode.cn/gtdhgbbedo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhixingplan.top/gtiqflhrvw.html

[D26] 数组转字符串
来源：http://hz.9152youxi.cn/gtzqfzjivp.html

Py:   ", ".join(map(str, arr))
来源：http://hz.fzhhl.top/gttucmwnly.html

PHP:  implode(", ", $arr);
来源：http://hz.yanxiufei.cn/gtgqbzfthi.html

JS:   arr.join(", ")
来源：http://hz.zycfv.cn/gtwvoerqrp.html

TS:   arr.join(", ")
来源：http://hz.hysaishi.cn/gtizzidskx.html

Java: String.join(", ", list)
来源：http://hz.mhx1999.top/gtsmzewueo.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hysaishi.cn/gtfsqlehek.html

Ruby: arr.join(", ")
来源：http://hz.shanyushiyangtech.top/gtgdvrlidi.html

C#:   string.Join(", ", list)
来源：http://hz.tian-w.cn/gtqofxjdkc.html

================================================================================
来源：http://hz.haohaochexian.top/gtyjmbnukw.html

E. 字符串处理
来源：http://hz.ivvv.top/gtifsepilo.html

================================================================================
来源：http://hz.jiagoushi.top/gtqdxmmgjj.html

[E01] 拼接字符串
来源：http://hz.cashguo.top/gttiwiapoz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xingfuxueyuan.xyz/gtattxfqbf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gzhubu.top/gtcejohljr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shzxlz.cn/gtumajjqiv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gtdvqezfli.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yj202588.top/gtkqxpohoq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.wangshuangyany.cn/gtldyiihyn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinqigufen.top/gttertchpn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.kuanghao11.cn/gtidwceryb.html

[E02] 重复字符串
来源：http://hz.jinqigfzy.top/gtmouqxlmq.html

Py:   "ab" * 3
来源：http://hz.haohaochexian.top/gtibcrgwrp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cucudq.cn/gtwxjcuzie.html

JS:   "ab".repeat(3)
来源：http://hz.yangfankeji.com/gtglaamxae.html

TS:   "ab".repeat(3)
来源：http://hz.xuanzx.com/gtbfmjobyn.html

Java: "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtneziindi.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.birdmap.top/gtztwqkcpe.html

Ruby: "ab" * 3
来源：http://hz.yuxming.cn/gtjpboiusm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenlongwang.top/gtvcdgtbbh.html

[E03] 截取子串
来源：http://hz.yuanzhike.top/gtogogktgl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ivvv.top/gttjejnbws.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.quarkkingdee.top/gtapiwpkyc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yangfankeji.com/gtvjsqgtsp.html

TS:   s.slice(1, 4)
来源：http://hz.hnxiangtu.top/gtlhayqxnz.html

Java: s.substring(1, 4)
来源：http://hz.zhixingplan.top/gtaprrecwu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.aibaodan.cn/gtkgylcjil.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.316326.xyz/gtlqesntst.html

C#:   s.Substring(1, 3)
来源：http://hz.nwbrower.top/gtqdwdrcwj.html

[E04] 查找子串位置
来源：http://hz.pengpengdd.cyou/gtuwiunacj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hywenlv.cn/gtegttbmuv.html

PHP:  strpos($s, "x");
来源：http://hz.feifeiyinyue.top/gtgrkhrtso.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.c1oappe.top/gtjnizykun.html

TS:   s.indexOf("x")
来源：http://hz.yueranfly.top/gtecbevhhk.html

Java: s.indexOf("x")
来源：http://hz.yj20258888.top/gtogjkqduf.html

Go:   strings.Index(s, "x")
来源：http://hz.9152youxi.cn/gtjrbjcwjx.html

Ruby: s.index("x")
来源：http://hz.hfpthk.cn/gtavgortpz.html

C#:   s.IndexOf("x")
来源：http://hz.bjfxy.top/gthxcxaupr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jqgfzy.top/gtbsgtpjld.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jinyuanbaomall.cn/gthhhgqlku.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.fzhhl.top/gtsjqvkjus.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jianghu66.top/gtatoselpc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yuanzhike.top/gtfntlqyrv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangkeji.top/gtlcuxvxta.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.aibaodan.cn/gtlzkopluo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ehwqpu.com/gtvfnphjrt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hongshengwenyu.top/gtdyiqyekf.html

[E06] 替换子串
来源：http://hz.tian-w.cn/gttbykupns.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.guowangkeji.top/gtojoatyhr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhongyouzk.top/gtnsyvnqdc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtofdzfdnn.html


<!-- 参考信息 -->