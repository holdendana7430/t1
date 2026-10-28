代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hysaishi.cn/gtoxspwoxg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.0kj1m.cn/gtxogvmvay.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ydzc1.top/gtqxfibyza.html

Ruby: # 无泛型
来源：http://hz.xylfe.cn/gtmvmzlmug.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.redwolf501.top/gtbxdvmchm.html

[C15] 解构 / 展开参数
来源：http://hz.chenzaomai.com/gtzmygddgf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgfzy.top/gtcpfvrdme.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj202588.top/gtvrlkmdft.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinqigufen.top/gtgrdipdgs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yonumen.top/gtfoajkngb.html

Java: // 无解构
来源：http://hz.fzhhl.top/gtchcmrkkp.html

Go:   // 无解构
来源：http://hz.hongshengwenyu.top/gtibahmldx.html

Ruby: a, b = pair
来源：http://hz.wangshuangyany.cn/gtbbdbtrma.html

C#:   var (a, b) = pair;
来源：http://hz.hysaishi.cn/gtewhipxut.html

[C16] 函数 / 方法重载
来源：http://hz.xylfe.cn/gtzvbsjvmi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sxryk.cn/gtnfmfaczt.html

PHP:  // 无重载
来源：http://hz.aizwys.cn/gtfyorrkvx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hammf.cn/gtqdqiadze.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.svipenyu.cn/gtrnzxlypj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xinyue.icu/gtqzpjpwli.html

Go:   // 无重载：用不同函数名
来源：http://hz.shuidangran.top/gtalhijfut.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cashguo.top/gttatypwje.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.birdmap.top/gtedvxurem.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtcskikube.html

D. 数组 / 列表 / 集合
来源：http://hz.jianghu66.top/gtngubdqot.html

================================================================================
来源：http://hz.yj202588.top/gtaatpcrux.html

[D01] 创建数组 / 列表
来源：http://hz.tian-w.cn/gtulshxndb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cdnleiting.top/gtcemlhlus.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jqgfzy.top/gtziyeouzt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yuxming.cn/gtailwwxhb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xuetiantiany.cn/gtulnlrerw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.pycfn.com/gtfulbbcfn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shuidangran.top/gthjwyftfa.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ybcxt.top/gtgskdkvwr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.nwbrower.top/gtllvvpkqt.html

[D02] 追加元素到末尾
来源：http://hz.pengpengdd.cyou/gtajmhocww.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sxryk.cn/gtbwyroqvz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinyuanbaomall.cn/gthjgvpljz.html

JS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gtraatmgdm.html

TS:   arr.push(4);
来源：http://hz.havefunace.top/gtrvvsjpca.html

Java: list.add(4);
来源：http://hz.cdnleiting.top/gtwupubvtq.html

Go:   arr = append(arr, 4)
来源：http://hz.nwbrower.top/gtroqaraoa.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cdnleiting.top/gtrciiidfk.html

C#:   list.Add(4);
来源：http://hz.gogol.net.cn/gtuwqexjdb.html

[D03] 在指定位置插入元素
来源：http://hz.zhaomingkeji.xyz/gtdyximgex.html

Py:   arr.insert(0, 0)
来源：http://hz.sxryk.cn/gthtamsrkl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yueranfly.top/gttsqvuvfx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.0kj1m.cn/gtlzwcfama.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ydzc1.top/gtkezwzrgc.html

Java: list.add(0, 0);
来源：http://hz.yanxiufei.cn/gtfcktcokb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.pycfn.com/gtsnbouqfd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tanke756.top/gtpsdqquxy.html

C#:   list.Insert(0, 0);
来源：http://hz.52xcode.cn/gtfohbllot.html

[D04] 删除元素
来源：http://hz.nanxuanxn.top/gtwuooxpcm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.gaohongyu789.top/gtspchtgcy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.9152youxi.cn/gtlfnhxyms.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hnqzz.top/gtraweatox.html

TS:   arr.splice(0, 1);
来源：http://hz.bjfxy.top/gtcefyponq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinqigfzy.top/gtycfttoca.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hongshengwenyu.top/gtokytoobl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hnqzz.top/gtnnuonjup.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zdqjudy.top/gtwzdxgnfk.html

[D05] 访问与修改元素
来源：http://hz.vqdsnc.cn/gtxvbtgpdc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gtnpomxdgd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.andypj.xyz/gtrilzrisp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hysaishi.cn/gtnnacgxnh.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xuanzx.com/gtmewyjxca.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tian-w.cn/gtvlcwfubx.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.mhx1999.top/gtmzivcmcv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ppjwa.cn/gtclscqfne.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.guannengcc.top/gtfunknhfr.html

[D06] 数组长度
来源：http://hz.snrcjt.cn/gtweepsszm.html

Py:   len(arr)
来源：http://hz.jinyuanbaomall.cn/gtlwrnsvhg.html

PHP:  count($arr);
来源：http://hz.shanyushiyangtech.top/gtmbjstgxy.html

JS:   arr.length
来源：http://hz.xylfe.cn/gtdpsqxarc.html

TS:   arr.length
来源：http://hz.yuanzhike.top/gttywjjaub.html

Java: list.size();
来源：http://hz.snrcjt.cn/gtzerxdpwc.html

Go:   len(arr)
来源：http://hz.mhx1999.top/gtghmazwgi.html

Ruby: arr.length; arr.size
来源：http://hz.hywenlv.cn/gtdwfogwgs.html

C#:   list.Count;
来源：http://hz.birdmap.top/gtoephipfx.html

[D07] 切片 / 取子数组
来源：http://hz.xingfuxueyuan.xyz/gtrnzzlusz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.fengsongda.top/gtzvzamctl.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yj20258.top/gtzbkqrirv.html

JS:   arr.slice(1, 4);
来源：http://hz.zhijiandao.cn/gtmxfggewq.html

TS:   arr.slice(1, 4);
来源：http://hz.jlsjyb.cn/gtqqjmipsr.html

Java: list.subList(1, 4);
来源：http://hz.gotoacloud.top/gtwgofkipx.html

Go:   arr[1:4]
来源：http://hz.9152youxi.cn/gtlfnqvumm.html

Ruby: arr[1, 3]
来源：http://hz.aizwys.cn/gtnjutwcbx.html

C#:   list.GetRange(1, 3);
来源：http://hz.pengpengdd.cyou/gtehsaduxb.html

[D08] 合并两个数组
来源：http://hz.iojbl.cn/gtixdrqycp.html

Py:   a + b;  a.extend(b)
来源：http://hz.gogol.net.cn/gtvvvsqqqf.html

PHP:  array_merge($a, $b);
来源：http://hz.chenjidiqi.icu/gtxfiuqyxo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.chenzaomai.com/gtlcdvxqss.html

TS:   [...a, ...b];
来源：http://hz.xinyue.icu/gtdslrapmh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.vqdsnc.cn/gtzvkvuypc.html

Go:   append(a, b...)
来源：http://hz.cheryme.top/gtbxoimqzm.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hongshengwenyu.top/gtirxohgnd.html

C#:   a.Concat(b).ToList()
来源：http://hz.sysykeji.top/gtuxhzvxfw.html

[D09] 排序（升序）
来源：http://hz.hnxiangtu.top/gtmwkwwlah.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.quarkkingdee.top/gtldnywynb.html

PHP:  sort($arr);
来源：http://hz.ehwqpu.com/gtjydmvzbf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj20258888.top/gtdpcoyqdz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.nanxuanxn.top/gtbbvssprw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hnxiangtu.top/gtrmboaigg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fengsongda.top/gtmpkmvogy.html

Ruby: arr.sort
来源：http://hz.dashuyun.cn/gtnixfliid.html

C#:   list.Sort();
来源：http://hz.fzhhl.top/gtdddimavb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhengqikj.top/gtfsqueuse.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hammf.cn/gtfzshpnwc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cucudq.cn/gtekuazwqy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daxiang520.top/gtuituywxh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.dashuyun.cn/gtxadszghx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tian-w.cn/gtzxphelxt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yueranfly.top/gtoyyxocqm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shangyingyoupin.top/gtgefirrfu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ydjk.org.cn/gtsfcjygha.html

[D11] 反转数组
来源：http://hz.cashguo.top/gtgwbmzpqo.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.aizwys.cn/gtgtpwivoc.html

PHP:  array_reverse($arr);
来源：http://hz.kuanghao11.cn/gtchsrjfvr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jlsjyb.cn/gtnfsroodp.html

TS:   [...arr].reverse();
来源：http://hz.vqdsnc.cn/gtzgahkldm.html

Java: Collections.reverse(list);
来源：http://hz.yongpay.top/gtpmwejrnn.html

Go:   slices.Reverse(arr)
来源：http://hz.tian-w.cn/gtuawsyvvg.html

Ruby: arr.reverse
来源：http://hz.yangfankeji.com/gtfcphljaf.html

C#:   list.Reverse();
来源：http://hz.vqdsnc.cn/gtekxlaaij.html

[D12] 查找元素下标
来源：http://hz.jyoumei.cn/gtopydeuvw.html

Py:   arr.index(x);  x in arr
来源：http://hz.svipenyu.cn/gtdgljaujl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhijiandao.cn/gtzmltogsp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangshuangyany.cn/gtemoukuou.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtyetlarix.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ydzc1.top/gtpdbmiyrz.html

Go:   slices.Index(arr, x)
来源：http://hz.sysykeji.top/gtojcdkbwj.html

Ruby: arr.index(x)
来源：http://hz.zhaomingkeji.xyz/gtrittbmyf.html

C#:   list.IndexOf(x);
来源：http://hz.yuanzhike.top/gtnxwjvjpf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ehwqpu.com/gtdfrtxfom.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhiwuduotai.top/gtwabqdujk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinqigfzy.top/gtswteftqm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gogol.net.cn/gtitklaicr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.tanke756.top/gtdkubjxam.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.vqdsnc.cn/gtvwtncrmx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.feifeiyinyue.top/gttpptacfx.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gotoacloud.top/gtdazkdysc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cucudq.cn/gtkikcssfs.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xziqi.cn/gtoxclvtfs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.0kj1m.cn/gtalsnchmm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhiwuduotai.top/gtidvsicda.html

JS:   arr.map(x => x * 2)
来源：http://hz.andypj.xyz/gtxavwrfnb.html

TS:   arr.map(x => x * 2)
来源：http://hz.chenjidiqi.icu/gttpdrckbd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.wangshuangyany.cn/gtamectbmu.html

Go:   // 手写循环
来源：http://hz.kuanghao11.cn/gtwzihidbh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhongyouzk.top/gtgfgnhbaw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.svipenyu.cn/gtigntxxis.html

[D15] 去重
来源：http://hz.pycfn.com/gtsatdfskk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jqgufenzy.top/gtnwafxikf.html

PHP:  array_unique($arr);
来源：http://hz.kuanghao11.cn/gtkvzfwfdj.html

JS:   [...new Set(arr)]
来源：http://hz.xylfe.cn/gttwmjaszb.html

TS:   [...new Set(arr)]
来源：http://hz.cheryme.top/gtpuivrnva.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cashguo.top/gtxrqpruuf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.snrcjt.cn/gtkrntetbf.html

Ruby: arr.uniq
来源：http://hz.jinqigfzy.top/gtjofmuhzw.html

C#:   list.Distinct().ToList()
来源：http://hz.haohaochexian.top/gtdlbfjhqt.html

[D16] 求和与平均值
来源：http://hz.quarkkingdee.top/gthpvihnzf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinqigfzy.top/gtzpqqolyv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yuxming.cn/gtuwxmjuau.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.0kj1m.cn/gtakqknpyw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtgiljvvuz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.daxiang520.top/gtkpfxbgty.html

Go:   // 手写循环累加
来源：http://hz.xingfuxueyuan.xyz/gtgkpemfna.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gzhubu.top/gtlpcwrpuy.html

C#:   list.Sum();  list.Average()
来源：http://hz.daxiang520.top/gtigebxbsc.html

[D17] 最大值与最小值
来源：http://hz.shangyingyoupin.top/gttvdoztlx.html

Py:   max(arr);  min(arr)
来源：http://hz.cashguo.top/gtayfarhnt.html

PHP:  max($arr);  min($arr);
来源：http://hz.gogol.net.cn/gtrtcenjbd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dianchejie.cn/gttzcfojfm.html

TS:   Math.max(...arr);
来源：http://hz.dianchejie.cn/gtneldnqjo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gogol.net.cn/gtkfitcplz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sufxvd.cn/gtlibcoxyv.html

Ruby: arr.max;  arr.min
来源：http://hz.ehwqpu.com/gtbmfgabwi.html

C#:   list.Max();  list.Min()
来源：http://hz.gogol.net.cn/gteuvijqbb.html

[D18] 扁平化嵌套数组
来源：http://hz.jqgufenzy.top/gtflxykhld.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xylfe.cn/gtmxskjenv.html

PHP:  array_merge(...$nested);
来源：http://hz.hysaishi.cn/gtodgynwwz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.meibo888.top/gtsiudusgj.html

TS:   nested.flat();
来源：http://hz.tianlin.xyz/gtmxnmdkdl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.0kj1m.cn/gtqwlabdua.html

Go:   // 手写双层循环
来源：http://hz.ydjk.org.cn/gtectibzub.html

Ruby: nested.flatten
来源：http://hz.cqqwz.cn/gtyrrnurde.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.haohaochexian.top/gtnsqvyllf.html

[D19] 按字段分组
来源：http://hz.hongshengwenyu.top/gthfzpogql.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.guannengcc.top/gtvpjipgrj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.gzhubu.top/gtklnenarp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.aibaodan.cn/gtacpoxdjx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinghuilouyu.cn/gtoesbhjuk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yj202588.top/gtsombkrzf.html

Go:   // 手写 map[string][]T
来源：http://hz.cheryme.top/gticwpneti.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cashguo.top/gtmzshawfw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yvedp.cn/gtxdlsyaik.html

[D20] 统计每个元素出现次数
来源：http://hz.yonumen.top/gtvpjgqtdi.html

Py:   Counter(arr)
来源：http://hz.jinyuanbaomall.cn/gtfzetnphs.html

PHP:  array_count_values($arr);
来源：http://hz.ywan-chungtsiang.top/gtbkfedwdu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sysykeji.top/gtdloevshk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zycfv.cn/gtrwoneaoj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shzxlz.cn/gtcghnybng.html

Go:   // 手写 map[T]int
来源：http://hz.chenlongwang.top/gtdqoxrzft.html

Ruby: arr.tally
来源：http://hz.52xcode.cn/gtzioukqbj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhiwuduotai.top/gtlcgjdngu.html

[D21] 判断是否包含某元素
来源：http://hz.mhx1999.top/gtwjoxuzbn.html

Py:   x in arr
来源：http://hz.mhx1999.top/gtflxxgxra.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ehwqpu.com/gtnogakqcg.html

JS:   arr.includes(x)
来源：http://hz.jlsjyb.cn/gtuhkuebhs.html

TS:   arr.includes(x)
来源：http://hz.zhaomingkeji.xyz/gthneznera.html

Java: list.contains(x)
来源：http://hz.zhongyouzk.top/gtymrkogic.html

Go:   slices.Contains(arr, x)
来源：http://hz.aizwys.cn/gtjnakgxpx.html

Ruby: arr.include?(x)
来源：http://hz.hfpthk.cn/gtkncjwheq.html

C#:   list.Contains(x)
来源：http://hz.zdqjudy.top/gtbjjzlhff.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sysykeji.top/gtrjwcdosb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nwbrower.top/gtijzkzpjx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.iojbl.cn/gtpihvtqxh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shanyushiyangtech.top/gtxzkyixaf.html

TS:   [...arr];
来源：http://hz.meibo888.top/gthkrmsrtn.html

Java: new ArrayList<>(list);
来源：http://hz.guannengcc.top/gtbcplpstb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinghuilouyu.cn/gtyhwumvtf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.iojbl.cn/gtroifklxl.html

C#:   new List<int>(list);
来源：http://hz.ywan-chungtsiang.top/gtsuvmuvjt.html

[D23] reduce 累积计算
来源：http://hz.cqqwz.cn/gtdcsyokgv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.0kj1m.cn/gtssbzxuej.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hnqzz.top/gtncpwkrsv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.havefunace.top/gtvlwyzlkq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guannengcc.top/gtvvzhjyhm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tian-w.cn/gtxlxzdzxq.html

Go:   // 手写循环
来源：http://hz.bjfxy.top/gtcgkepanu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cdnleiting.top/gtxbqknmvq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.wangshuangyany.cn/gtvigmvvdr.html

[D24] 字典 / Map 基本操作
来源：http://hz.nanxinkj.top/gttkbbinhp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.aibaodan.cn/gtvegcysoo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cqqwz.cn/gtzmtmepjq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ybcxt.top/gtjnnkcmoe.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xylfe.cn/gtupuvvfmz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.52xcode.cn/gtialrlnbi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xziqi.cn/gtqclsyccz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shanyushiyangtech.top/gtzeazedse.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jyoumei.cn/gtruvgcwiy.html

[D25] Set 集合去重与交并差
来源：http://hz.ppjwa.cn/gtpsynltam.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ivvv.top/gtucfdjvfc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ivvv.top/gtrtntytmx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xinyue.icu/gtylggouel.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gotoacloud.top/gtxwnaydnx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hongshengwenyu.top/gtcnucwfik.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.vqdsnc.cn/gtlhuvemvx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yueranfly.top/gtvwlwontf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj202588.top/gtwuvxzwin.html

[D26] 数组转字符串
来源：http://hz.xziqi.cn/gtcockhmjk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.wangdashe.top/gtebealqjb.html

PHP:  implode(", ", $arr);
来源：http://hz.sysykeji.top/gttwtzwzrr.html

JS:   arr.join(", ")
来源：http://hz.316326.xyz/gtdqpxaqiv.html

TS:   arr.join(", ")
来源：http://hz.hfpthk.cn/gtdlmweiwm.html

Java: String.join(", ", list)
来源：http://hz.ivvv.top/gtbpzehatt.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hongshengwenyu.top/gtxkhivyse.html

Ruby: arr.join(", ")
来源：http://hz.yuanzhike.top/gtwuhgnxaa.html

C#:   string.Join(", ", list)
来源：http://hz.hammf.cn/gtozhbyddv.html

================================================================================
来源：http://hz.zhongyouzk.top/gtebirsffq.html

E. 字符串处理
来源：http://hz.yuxming.cn/gtmsqsuwmd.html

================================================================================
来源：http://hz.aizwys.cn/gtontjeiez.html

[E01] 拼接字符串
来源：http://hz.tanke756.top/gthsdiklyk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sxryk.cn/gtngivzrse.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhaomingkeji.xyz/gtfzlwcwzx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj202588.top/gturprbpmm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.9152youxi.cn/gtptnkrixb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.feifeiyinyue.top/gtpqfjaywy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zdqjudy.top/gtcnjvibla.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jqgfzy.top/gtkyscbgat.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.pengpengdd.cyou/gtvyqhkfas.html

[E02] 重复字符串
来源：http://hz.fengsongda.top/gtksrfzrnv.html

Py:   "ab" * 3
来源：http://hz.gotoacloud.top/gtojqjgwac.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gaohongyu789.top/gtbqjymiyh.html

JS:   "ab".repeat(3)
来源：http://hz.hnqzz.top/gtltrbeppt.html

TS:   "ab".repeat(3)
来源：http://hz.cashguo.top/gtrehaxtyq.html

Java: "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtcuhweehv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinqigufen.top/gtzrvnlsgn.html

Ruby: "ab" * 3
来源：http://hz.zhixingplan.top/gtqstlmnsn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xziqi.cn/gtzsvlcqsx.html

[E03] 截取子串
来源：http://hz.shuidangran.top/gtqoqobbrs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yueranfly.top/gtpgfrhdvs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.aizwys.cn/gtgawnwrpy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.nwbrower.top/gtxtxvlxfp.html

TS:   s.slice(1, 4)
来源：http://hz.ppjwa.cn/gtrhkggnhu.html

Java: s.substring(1, 4)
来源：http://hz.shanyushiyangkeji.top/gtwyptfzer.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.shuidangran.top/gtjfnfqswp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yj20258888.top/gtzlawwdvt.html

C#:   s.Substring(1, 3)
来源：http://hz.andypj.xyz/gtzkaiqrav.html

[E04] 查找子串位置
来源：http://hz.shuidangran.top/gtehnittcc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.smart0.xyz/gtjpbjjaue.html

PHP:  strpos($s, "x");
来源：http://hz.quarkkingdee.top/gthxtbrahz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.wangshuangyany.cn/gtzgpkpind.html

TS:   s.indexOf("x")
来源：http://hz.ehwqpu.com/gtprxapzsp.html

Java: s.indexOf("x")
来源：http://hz.ivvv.top/gtlgrtfpix.html

Go:   strings.Index(s, "x")
来源：http://hz.sysykeji.top/gtkbxriqjq.html

Ruby: s.index("x")
来源：http://hz.0kj1m.cn/gtoxsywrls.html

C#:   s.IndexOf("x")
来源：http://hz.cheryme.top/gtkjflzawp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinqigfzy.top/gtjxiprcqb.html


<!-- 参考信息 -->