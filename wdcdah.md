代发 wailian999

Ruby: a, b = pair
来源：http://hz.chenzaomai.com/gthzgykilk.html

C#:   var (a, b) = pair;
来源：http://hz.cucudq.cn/gtawfucvbs.html

[C16] 函数 / 方法重载
来源：http://hz.hnqzz.top/gtsnujdbwe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.wangdashe.top/gtzawrutii.html

PHP:  // 无重载
来源：http://hz.aibaodan.cn/gtqzplpxno.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.smart0.xyz/gtmmkkemte.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yuanzhike.top/gttqfdjthk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shanyushiyangkeji.top/gtwosdfqxj.html

Go:   // 无重载：用不同函数名
来源：http://hz.yonumen.top/gteiuxvcdw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.fengsongda.top/gtjwxtztro.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.nanxuanxn.top/gtbtdjkngz.html

================================================================================
来源：http://hz.aizwys.cn/gtchkfejcn.html

D. 数组 / 列表 / 集合
来源：http://hz.kuanghao11.cn/gtnenlxupy.html

================================================================================
来源：http://hz.ivvv.top/gtdwzahtqm.html

[D01] 创建数组 / 列表
来源：http://hz.shzxlz.cn/gtzrnngndy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hammf.cn/gtwrsjjqxy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.smart0.xyz/gtosesuwdf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.0kj1m.cn/gtwkapmvhd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xuanzx.com/gtgvmiqmhg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ydjk.org.cn/gtxwqewubm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.birdmap.top/gtwddxzkxf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shangyingyoupin.top/gtogkrwfpc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jianghu66.top/gtjnwqzwxe.html

[D02] 追加元素到末尾
来源：http://hz.chenlongwang.top/gthrpqinik.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.havefunace.top/gtehfcsrjl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jianghu66.top/gtglzpleby.html

JS:   arr.push(4);
来源：http://hz.shanyushiyangtech.top/gtsfvxffbb.html

TS:   arr.push(4);
来源：http://hz.wangdashe.top/gtbwoduygv.html

Java: list.add(4);
来源：http://hz.yangfankeji.com/gtgnypyafg.html

Go:   arr = append(arr, 4)
来源：http://hz.cqqwz.cn/gtpiirazwh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jqgfzy.top/gtszjkguvw.html

C#:   list.Add(4);
来源：http://hz.yangfankeji.com/gtutqbcsud.html

[D03] 在指定位置插入元素
来源：http://hz.zhengqikj.top/gtspwykjcz.html

Py:   arr.insert(0, 0)
来源：http://hz.iojbl.cn/gtilebyqfp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.guowangkeji.top/gtsgpqcnve.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xingfuxueyuan.xyz/gtjpchxcgb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhijiandao.cn/gtprxilmby.html

Java: list.add(0, 0);
来源：http://hz.nwbrower.top/gtneewxhek.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.c1oappe.top/gtztlbjtdf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.nanxinkj.top/gtjlegloop.html

C#:   list.Insert(0, 0);
来源：http://hz.xingfuxueyuan.xyz/gtdzcgoxvf.html

[D04] 删除元素
来源：http://hz.zycfv.cn/gtdftomnwa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.0kj1m.cn/gtchhojumg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhengqikj.top/gtumpstoqc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.9152youxi.cn/gtwhnbbnzy.html

TS:   arr.splice(0, 1);
来源：http://hz.sxryk.cn/gtbdfbutna.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hongshengwenyu.top/gtagbkkmdl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yj20258.top/gtyqgdajtp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.pycfn.com/gtzztoufig.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jiagoushi.top/gtzumgcxyq.html

[D05] 访问与修改元素
来源：http://hz.aibaodan.cn/gtmaonxgea.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtjmyqqert.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xuetiantiany.cn/gtmiieixtg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sufxvd.cn/gtzzoosayu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nwbrower.top/gtcvrcdjeq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinqigfzy.top/gtqdztytwi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.chenjidiqi.icu/gtxetgbmob.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.feifeiyinyue.top/gtdlnltvgg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ehwqpu.com/gtirddgfli.html

[D06] 数组长度
来源：http://hz.shuidangran.top/gtverbyfhf.html

Py:   len(arr)
来源：http://hz.zdqjudy.top/gtwhwnrkux.html

PHP:  count($arr);
来源：http://hz.sxryk.cn/gtviijqjso.html

JS:   arr.length
来源：http://hz.zycfv.cn/gtisuwjovi.html

TS:   arr.length
来源：http://hz.hysaishi.cn/gtpmdsyeca.html

Java: list.size();
来源：http://hz.daxiang520.top/gttoqarunj.html

Go:   len(arr)
来源：http://hz.ywan-chungtsiang.top/gtsmtxwfgt.html

Ruby: arr.length; arr.size
来源：http://hz.zhaomingkeji.xyz/gtwpusqxlx.html

C#:   list.Count;
来源：http://hz.jianghu66.top/gtzjnkzpll.html

[D07] 切片 / 取子数组
来源：http://hz.feifeiyinyue.top/gtgjcdkkei.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xziqi.cn/gtdhebmhom.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yj20258888.top/gtqkqkeajm.html

JS:   arr.slice(1, 4);
来源：http://hz.havefunace.top/gthsxvzqyi.html

TS:   arr.slice(1, 4);
来源：http://hz.hnqzz.top/gtpuibkixa.html

Java: list.subList(1, 4);
来源：http://hz.jqgufenzy.top/gtajwwbobl.html

Go:   arr[1:4]
来源：http://hz.ywan-chungtsiang.top/gtchwrxlbu.html

Ruby: arr[1, 3]
来源：http://hz.hfpthk.cn/gtwmhrmflu.html

C#:   list.GetRange(1, 3);
来源：http://hz.sufxvd.cn/gtkuibmldl.html

[D08] 合并两个数组
来源：http://hz.feifeiyinyue.top/gtpumvkgtb.html

Py:   a + b;  a.extend(b)
来源：http://hz.0kj1m.cn/gtyyowfxef.html

PHP:  array_merge($a, $b);
来源：http://hz.ydzc1.top/gtyumgnofu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhixingplan.top/gtzkvjlowd.html

TS:   [...a, ...b];
来源：http://hz.chenlongwang.top/gtyzpjdvmp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhoulong.xyz/gtypaslpno.html

Go:   append(a, b...)
来源：http://hz.snrcjt.cn/gtnlcdwhcl.html

Ruby: a + b;  a.concat(b)
来源：http://hz.wangdashe.top/gtmcatkejn.html

C#:   a.Concat(b).ToList()
来源：http://hz.smart0.xyz/gtdysthooe.html

[D09] 排序（升序）
来源：http://hz.jqgfzy.top/gtnubamwsu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.iojbl.cn/gtrlsqaqje.html

PHP:  sort($arr);
来源：http://hz.haohaochexian.top/gtlikeyskb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.kuanghao11.cn/gtraxntxhd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.fengsongda.top/gtjmufzfwg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.daria6918.cn/gtwdmgwmce.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.pengpengdd.cyou/gtfxsixbrl.html

Ruby: arr.sort
来源：http://hz.cdnleiting.top/gtzjboyjkj.html

C#:   list.Sort();
来源：http://hz.shanyushiyangtech.top/gtropfmjzp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jlsjyb.cn/gtlylljpeo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.quarkkingdee.top/gtyygmbwqb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258.top/gtlubdkaia.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.redwolf501.top/gtfkjzjuiu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.c1oappe.top/gtgcpokrnn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xziqi.cn/gtpnjtlwpq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jqgfzy.top/gtwwyybjxn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xziqi.cn/gtzbbiyqnc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jqgufenzy.top/gtnduhvxrz.html

[D11] 反转数组
来源：http://hz.jqgfzy.top/gthppgpcei.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jianghu66.top/gtqpoxhvoi.html

PHP:  array_reverse($arr);
来源：http://hz.bjfxy.top/gtbnkwevim.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.fengsongda.top/gtycyvdvye.html

TS:   [...arr].reverse();
来源：http://hz.chenlongwang.top/gtcdkfwhtd.html

Java: Collections.reverse(list);
来源：http://hz.jinghuilouyu.cn/gtuulqcapn.html

Go:   slices.Reverse(arr)
来源：http://hz.yangfankeji.com/gtjwkxacro.html

Ruby: arr.reverse
来源：http://hz.nanxinkj.top/gtarstlkoz.html

C#:   list.Reverse();
来源：http://hz.ydzc1.top/gtbyuktxra.html

[D12] 查找元素下标
来源：http://hz.0kj1m.cn/gtzwkvuihb.html

Py:   arr.index(x);  x in arr
来源：http://hz.c1oappe.top/gtnomskkhr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sysykeji.top/gtksozthnn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnqzz.top/gtvwmrungf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tianlin.xyz/gtxejdodqz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hywenlv.cn/gtzyghaavj.html

Go:   slices.Index(arr, x)
来源：http://hz.c1oappe.top/gtjxejyfee.html

Ruby: arr.index(x)
来源：http://hz.daria6918.cn/gtoaufhetb.html

C#:   list.IndexOf(x);
来源：http://hz.fengsongda.top/gtuklsoibt.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xylfe.cn/gtxpmrqbrj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.snrcjt.cn/gtwzzyrjxp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cqqwz.cn/gtuadopxsi.html

JS:   arr.filter(x => x > 3)
来源：http://hz.tian-w.cn/gtrdgzmdnf.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yj202588.top/gtfvievngg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.fzhhl.top/gtdwzcdfmw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.0kj1m.cn/gtpmndmrkr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shanyushiyangtech.top/gtkklzgagn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenlongwang.top/gtxsjaigty.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dianchejie.cn/gtdewcghdx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ybcxt.top/gtcplpkork.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cashguo.top/gtdwmaixdv.html

JS:   arr.map(x => x * 2)
来源：http://hz.sufxvd.cn/gtjdjjlhhd.html

TS:   arr.map(x => x * 2)
来源：http://hz.chenzaomai.com/gtcwevgjvt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.vqdsnc.cn/gtnftrxtpe.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtpddbbsmt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sysykeji.top/gtrzcvryfj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ydzc1.top/gtpacznsij.html

[D15] 去重
来源：http://hz.kuanghao11.cn/gtrkavvjyr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.9152youxi.cn/gthslezhsm.html

PHP:  array_unique($arr);
来源：http://hz.dashuyun.cn/gtvdhxhcwz.html

JS:   [...new Set(arr)]
来源：http://hz.cheryme.top/gthojxgtas.html

TS:   [...new Set(arr)]
来源：http://hz.birdmap.top/gtahzejfqf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hammf.cn/gtmlpnycxk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.redwolf501.top/gtbzzsbeja.html

Ruby: arr.uniq
来源：http://hz.cqqwz.cn/gtnpvwtuxt.html

C#:   list.Distinct().ToList()
来源：http://hz.sufxvd.cn/gtfgzampgy.html

[D16] 求和与平均值
来源：http://hz.chenjidiqi.icu/gtdzfigali.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jiagoushi.top/gtsqayrkvm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hammf.cn/gtpkkooowl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sysykeji.top/gtzarmxped.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dashuyun.cn/gtqkyuufju.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ehwqpu.com/gtolbgscxc.html

Go:   // 手写循环累加
来源：http://hz.dashuyun.cn/gtwamdecvi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sweek.top/gtjqtbxdqa.html

C#:   list.Sum();  list.Average()
来源：http://hz.cdnleiting.top/gttmvuiaap.html

[D17] 最大值与最小值
来源：http://hz.jyoumei.cn/gtwjewmuqe.html

Py:   max(arr);  min(arr)
来源：http://hz.feifeiyinyue.top/gtiulskedx.html

PHP:  max($arr);  min($arr);
来源：http://hz.sufxvd.cn/gtabwzekdi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.svipenyu.cn/gtrmlzywhr.html

TS:   Math.max(...arr);
来源：http://hz.hongshengwenyu.top/gtomeayvwr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.guowangkeji.top/gtoxnijwua.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shanyushiyangkeji.top/gtrjbaglvw.html

Ruby: arr.max;  arr.min
来源：http://hz.xylfe.cn/gtfdvbrkcx.html

C#:   list.Max();  list.Min()
来源：http://hz.316326.xyz/gtnzccofin.html

[D18] 扁平化嵌套数组
来源：http://hz.ywan-chungtsiang.top/gtmjoftqpi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.havefunace.top/gtjoqtmgon.html

PHP:  array_merge(...$nested);
来源：http://hz.gzhubu.top/gtssfmxhah.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xingfuxueyuan.xyz/gtmpiotaxo.html

TS:   nested.flat();
来源：http://hz.aizwys.cn/gtonakhmqg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xuetiantiany.cn/gtaebwzshr.html

Go:   // 手写双层循环
来源：http://hz.yanxiufei.cn/gtmhkqvsui.html

Ruby: nested.flatten
来源：http://hz.ydjk.org.cn/gthyewoevs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hnqzz.top/gtelioacxj.html

[D19] 按字段分组
来源：http://hz.haohaochexian.top/gtkylpsgak.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.svipenyu.cn/gtehuollvf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ydjk.org.cn/gtlbxxnvmf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.sufxvd.cn/gtmkjsioxv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.fzhhl.top/gtcckxkbfe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhixingplan.top/gtdfjpmptw.html

Go:   // 手写 map[string][]T
来源：http://hz.nwbrower.top/gtivbiuntd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sufxvd.cn/gtohatdjcs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.aizwys.cn/gtcnfybzsz.html

[D20] 统计每个元素出现次数
来源：http://hz.guannengcc.top/gtbgqulbrq.html

Py:   Counter(arr)
来源：http://hz.0kj1m.cn/gtdjvffick.html

PHP:  array_count_values($arr);
来源：http://hz.yonumen.top/gtylfdawgk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sxryk.cn/gtbtntkghh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cashguo.top/gttabzhwir.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hfpthk.cn/gtcgmvhoaw.html

Go:   // 手写 map[T]int
来源：http://hz.zhiwuduotai.top/gtghfyxecl.html

Ruby: arr.tally
来源：http://hz.daxiang520.top/gtnuluzyaa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ivvv.top/gtgidrzvdk.html

[D21] 判断是否包含某元素
来源：http://hz.tianlin.xyz/gtiiipzmlr.html

Py:   x in arr
来源：http://hz.dianchejie.cn/gtxsrwbutt.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhongyouzk.top/gtuukndmnj.html

JS:   arr.includes(x)
来源：http://hz.zhixingplan.top/gtntiyzabk.html

TS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gtizbubzcq.html

Java: list.contains(x)
来源：http://hz.ydjk.org.cn/gtjejsrljm.html

Go:   slices.Contains(arr, x)
来源：http://hz.yangfankeji.com/gtziuhujlm.html

Ruby: arr.include?(x)
来源：http://hz.shzxlz.cn/gtvbqgmdpz.html

C#:   list.Contains(x)
来源：http://hz.ywan-chungtsiang.top/gtzujezjaf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.svipenyu.cn/gtgwbnzzxr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yj20258.top/gtbofvaoaq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hongshengwenyu.top/gtwickmycm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhaomingkeji.xyz/gtcoamyzsq.html

TS:   [...arr];
来源：http://hz.nwbrower.top/gtgmthatnm.html

Java: new ArrayList<>(list);
来源：http://hz.aizwys.cn/gtlpvcwfke.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xuetiantiany.cn/gtqbhermpf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhongyouzk.top/gtwdopdlvj.html

C#:   new List<int>(list);
来源：http://hz.jinghuilouyu.cn/gtvrumtovz.html

[D23] reduce 累积计算
来源：http://hz.chenlongwang.top/gtcflcmakp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.mhx1999.top/gtsvmwzqzk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ivvv.top/gtxeilcbqt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.0kj1m.cn/gtvsmzpzfb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.iojbl.cn/gtitdrbrzn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj20258888.top/gtirikqded.html

Go:   // 手写循环
来源：http://hz.yanxiufei.cn/gtbutuquzt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangdashe.top/gthxbtmbft.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jianghu66.top/gtbjiznpzu.html

[D24] 字典 / Map 基本操作
来源：http://hz.mhx1999.top/gtsstwufjx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.fzhhl.top/gtbpmsvxjp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ybcxt.top/gtxamhqbnb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.tanke756.top/gtqiuplqoa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yanxiufei.cn/gtbxvmdntw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.dashuyun.cn/gtqldngzxs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zycfv.cn/gtfpqlfbdv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.fzhhl.top/gtubmoxjuw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gogol.net.cn/gtnidaqeux.html

[D25] Set 集合去重与交并差
来源：http://hz.jianghu66.top/gtdezhdyqu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.0kj1m.cn/gtdzgrdkwj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gaohongyu789.top/gtgiaulncs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.guowangkeji.top/gtxmbmurpr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.pengpengdd.cyou/gtdcbwepdk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.tianlin.xyz/gtlectlmcc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yuxming.cn/gtirjuhinm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hongshengwenyu.top/gtbmakgtyp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cucudq.cn/gtgxprgaro.html

[D26] 数组转字符串
来源：http://hz.nwbrower.top/gtijhdqtbk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.9152youxi.cn/gtqwyflaed.html

PHP:  implode(", ", $arr);
来源：http://hz.svipenyu.cn/gtsqozldwf.html

JS:   arr.join(", ")
来源：http://hz.shanyushiyangtech.top/gtfsynsehb.html

TS:   arr.join(", ")
来源：http://hz.pycfn.com/gtyhdwjngm.html

Java: String.join(", ", list)
来源：http://hz.chenlongwang.top/gthuuiarrd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hywenlv.cn/gtzmmosjoj.html

Ruby: arr.join(", ")
来源：http://hz.shuidangran.top/gtycelwlaj.html

C#:   string.Join(", ", list)
来源：http://hz.jinghuilouyu.cn/gtdjaaewje.html

================================================================================
来源：http://hz.zycfv.cn/gtxwlxqrue.html

E. 字符串处理
来源：http://hz.shangyingyoupin.top/gtjdnmqghe.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtmxvelmmu.html

[E01] 拼接字符串
来源：http://hz.gogol.net.cn/gtglafhsfj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hfpthk.cn/gtwauxluyz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xylfe.cn/gtcrjngdyq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gtpazwbytf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhixingplan.top/gtnualopmw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.aizwys.cn/gtzwdtbxnk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hywenlv.cn/gtavskwxwt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ybcxt.top/gttfecplgv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.kuanghao11.cn/gtymmgseas.html

[E02] 重复字符串
来源：http://hz.ehwqpu.com/gtbawsfsde.html

Py:   "ab" * 3
来源：http://hz.yueranfly.top/gtvejkyevy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fengsongda.top/gtfsdieglt.html

JS:   "ab".repeat(3)
来源：http://hz.cheryme.top/gtsibvebfx.html

TS:   "ab".repeat(3)
来源：http://hz.wangdashe.top/gtgndrflgg.html

Java: "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtbslrehrx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.aizwys.cn/gtlylnkzyl.html

Ruby: "ab" * 3
来源：http://hz.ywan-chungtsiang.top/gtstsvdmeg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gogol.net.cn/gtziddvcyn.html

[E03] 截取子串
来源：http://hz.yj202588.top/gtuwosifwt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sweek.top/gtgxyhfudb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhixingplan.top/gtplypxqru.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj20258888.top/gtjcmwbqpu.html

TS:   s.slice(1, 4)
来源：http://hz.316326.xyz/gtkurispwp.html

Java: s.substring(1, 4)
来源：http://hz.guowangkeji.top/gteqiksacv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.gotoacloud.top/gtqejddxmg.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.nanxuanxn.top/gtlekqoqyt.html

C#:   s.Substring(1, 3)
来源：http://hz.sweek.top/gtsbdeeccq.html

[E04] 查找子串位置
来源：http://hz.ydzc1.top/gtenzdulfk.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xinyue.icu/gtdxdsutvf.html

PHP:  strpos($s, "x");
来源：http://hz.cqqwz.cn/gthftcyhcv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhaomingkeji.xyz/gthgmelqzl.html

TS:   s.indexOf("x")
来源：http://hz.zhengqikj.top/gtvftwtdio.html

Java: s.indexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtagfjqxhb.html

Go:   strings.Index(s, "x")
来源：http://hz.jianghu66.top/gtuljsepuk.html

Ruby: s.index("x")
来源：http://hz.kuanghao11.cn/gtyrvzklyi.html

C#:   s.IndexOf("x")
来源：http://hz.birdmap.top/gtlzvmmocu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinqigfzy.top/gtjodgyrxt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.gaohongyu789.top/gtmqchnrnv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.pengpengdd.cyou/gtydxqwwrb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ydzc1.top/gtqqbhrmbq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yj20258.top/gtqzbggkdk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnxiangtu.top/gtclefggbh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.guannengcc.top/gtpclxhwuf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ywan-chungtsiang.top/gtlfvedfsr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hammf.cn/gtkzcjtdlr.html

[E06] 替换子串
来源：http://hz.snrcjt.cn/gtybemyxse.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sweek.top/gtdsmnlcdt.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhengqikj.top/gtjuredyht.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtibgtveqe.html


<!-- 参考信息 -->