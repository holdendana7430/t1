代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yuxming.cn/gtropfjpfg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xinyue.icu/gtrcamgeex.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.bjfxy.top/gtysrnpxgc.html

Ruby: # 无泛型
来源：http://hz.zhixingplan.top/gtpxqkxmbv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhoulong.xyz/gtvakicgbd.html

[C15] 解构 / 展开参数
来源：http://hz.yvedp.cn/gttvyfvtqb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.fengsongda.top/gtdtdvdaum.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sweek.top/gtwhhfblys.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yuanzhike.top/gtbmmuentp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.snrcjt.cn/gtkjoqvrjv.html

Java: // 无解构
来源：http://hz.hywenlv.cn/gthweikqbe.html

Go:   // 无解构
来源：http://hz.zhongyouzk.top/gturaydqlm.html

Ruby: a, b = pair
来源：http://hz.xuetiantiany.cn/gtrrtcbszf.html

C#:   var (a, b) = pair;
来源：http://hz.wangshuangyany.cn/gttcxkvefb.html

[C16] 函数 / 方法重载
来源：http://hz.shuidangran.top/gtzuhycepy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cdnleiting.top/gtpyegxtbx.html

PHP:  // 无重载
来源：http://hz.feifeiyinyue.top/gtlitibcih.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xuanzx.com/gtxoaqiovn.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gotoacloud.top/gtttwldnaq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yj202588.top/gtzgybrbfo.html

Go:   // 无重载：用不同函数名
来源：http://hz.shangyingyoupin.top/gtqepaslyd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sweek.top/gtjffgidjd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jlsjyb.cn/gtrzsalaow.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtzwptkips.html

D. 数组 / 列表 / 集合
来源：http://hz.hongshengwenyu.top/gtnlqiipnq.html

================================================================================
来源：http://hz.meibo888.top/gtsvkevzjt.html

[D01] 创建数组 / 列表
来源：http://hz.jinqigufen.top/gtrazrtnpx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cheryme.top/gtdxozjvvk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.dashuyun.cn/gtjqnivzqk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.wangdashe.top/gtptcqblud.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ivvv.top/gthickynma.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.316326.xyz/gtnhmlcmrf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shanyushiyangkeji.top/gtvvvynnqm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.daxiang520.top/gtblhjihcy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aizwys.cn/gtgogfwpwb.html

[D02] 追加元素到末尾
来源：http://hz.yongpay.top/gtkpggfabf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.redwolf501.top/gtmmzoxeco.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.c1oappe.top/gtjroxunmn.html

JS:   arr.push(4);
来源：http://hz.dianchejie.cn/gttxydzepp.html

TS:   arr.push(4);
来源：http://hz.andypj.xyz/gtygtqleup.html

Java: list.add(4);
来源：http://hz.quarkkingdee.top/gtrquxoakh.html

Go:   arr = append(arr, 4)
来源：http://hz.kuanghao11.cn/gtzojqtyqx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.quarkkingdee.top/gtwativfje.html

C#:   list.Add(4);
来源：http://hz.chenlongwang.top/gtbhozamtq.html

[D03] 在指定位置插入元素
来源：http://hz.gzhubu.top/gtubvthciu.html

Py:   arr.insert(0, 0)
来源：http://hz.gogol.net.cn/gtsuodxlip.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hongshengwenyu.top/gteowkvjzq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yangfankeji.com/gtwvpsitmk.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.aizwys.cn/gtxddmzwhw.html

Java: list.add(0, 0);
来源：http://hz.guannengcc.top/gtzpkrzpvd.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhoulong.xyz/gthlezwnxa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.pengpengdd.cyou/gtfknoblkl.html

C#:   list.Insert(0, 0);
来源：http://hz.wangdashe.top/gtfquiulgq.html

[D04] 删除元素
来源：http://hz.yvedp.cn/gtwtqwrgrg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.316326.xyz/gtooukdsow.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yangfankeji.com/gtkrhbhuuj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenlongwang.top/gttvpgpezp.html

TS:   arr.splice(0, 1);
来源：http://hz.guannengcc.top/gtcxcnwngd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tanke756.top/gtncaixfvq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zycfv.cn/gtwvlteijw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenzaomai.com/gtwsbxejdh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shuidangran.top/gtaoywnrob.html

[D05] 访问与修改元素
来源：http://hz.sweek.top/gteropdkmw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj202588.top/gtvlvavncw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hywenlv.cn/gtfsqzmitf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jlsjyb.cn/gtbwhnlctl.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ydjk.org.cn/gthvfmagje.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xuanzx.com/gtsydzlcur.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.nanxinkj.top/gttojqarro.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nwbrower.top/gtxgpjkfpf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yangfankeji.com/gtuzpaoqjz.html

[D06] 数组长度
来源：http://hz.wangshuangyany.cn/gtskwwkzwd.html

Py:   len(arr)
来源：http://hz.zhoulong.xyz/gtvggmmrsr.html

PHP:  count($arr);
来源：http://hz.zhengqikj.top/gtmkewzwsw.html

JS:   arr.length
来源：http://hz.jinyuanbaomall.cn/gtazulxtqg.html

TS:   arr.length
来源：http://hz.kuanghao11.cn/gthlwpepqm.html

Java: list.size();
来源：http://hz.cdnleiting.top/gtpvhkqfbs.html

Go:   len(arr)
来源：http://hz.hfpthk.cn/gtbydjjamm.html

Ruby: arr.length; arr.size
来源：http://hz.sxryk.cn/gtfynwunmn.html

C#:   list.Count;
来源：http://hz.iojbl.cn/gtvqgebbqz.html

[D07] 切片 / 取子数组
来源：http://hz.hysaishi.cn/gtdbmxeazl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhaomingkeji.xyz/gtgypuruml.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hammf.cn/gtpecnocfb.html

JS:   arr.slice(1, 4);
来源：http://hz.hammf.cn/gtxxeermdy.html

TS:   arr.slice(1, 4);
来源：http://hz.iojbl.cn/gtdrixvlia.html

Java: list.subList(1, 4);
来源：http://hz.ywan-chungtsiang.top/gtstlgvnzm.html

Go:   arr[1:4]
来源：http://hz.tianlin.xyz/gtlynstuwg.html

Ruby: arr[1, 3]
来源：http://hz.ywan-chungtsiang.top/gtznefuuzs.html

C#:   list.GetRange(1, 3);
来源：http://hz.chenlongwang.top/gtjftrunzp.html

[D08] 合并两个数组
来源：http://hz.dashuyun.cn/gtsdromzli.html

Py:   a + b;  a.extend(b)
来源：http://hz.aizwys.cn/gtmduzfrzz.html

PHP:  array_merge($a, $b);
来源：http://hz.aizwys.cn/gthtznbsna.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yj20258.top/gtbjaixaik.html

TS:   [...a, ...b];
来源：http://hz.wangdashe.top/gtbxnfadhy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yuxming.cn/gtlgjotkdc.html

Go:   append(a, b...)
来源：http://hz.nwbrower.top/gtdmetiosj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.wangshuangyany.cn/gtqokmelji.html

C#:   a.Concat(b).ToList()
来源：http://hz.daxiang520.top/gtouwluqin.html

[D09] 排序（升序）
来源：http://hz.jqgfzy.top/gtqruhleoj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xingfuxueyuan.xyz/gtnlfwqovx.html

PHP:  sort($arr);
来源：http://hz.hnqzz.top/gtoljusppx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xuetiantiany.cn/gtumfjbqng.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sweek.top/gtantqrllg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jlsjyb.cn/gtaqdekbfv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.sysykeji.top/gtjjhsidza.html

Ruby: arr.sort
来源：http://hz.gaohongyu789.top/gtvnmygeds.html

C#:   list.Sort();
来源：http://hz.jlsjyb.cn/gtzvxiytes.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gogol.net.cn/gtaohmzoze.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.meibo888.top/gtdzaqpevg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xingfuxueyuan.xyz/gtozwcdbbb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gtjlfgjuqs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guannengcc.top/gtyicwisob.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jlsjyb.cn/gtokrsqugx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.chenlongwang.top/gtcpilpqtx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ywan-chungtsiang.top/gttvigbzwk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.bjfxy.top/gtiyjnjymi.html

[D11] 反转数组
来源：http://hz.52xcode.cn/gtzmpvdsfg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.svipenyu.cn/gtbdfxcbnp.html

PHP:  array_reverse($arr);
来源：http://hz.yangfankeji.com/gtirxzztfy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xylfe.cn/gtogydlaic.html

TS:   [...arr].reverse();
来源：http://hz.yj20258.top/gtwqzjkpcf.html

Java: Collections.reverse(list);
来源：http://hz.xuetiantiany.cn/gtacpzxkjc.html

Go:   slices.Reverse(arr)
来源：http://hz.jyoumei.cn/gthoibvifx.html

Ruby: arr.reverse
来源：http://hz.nanxinkj.top/gtwqwiupfx.html

C#:   list.Reverse();
来源：http://hz.feifeiyinyue.top/gtjqwspaaz.html

[D12] 查找元素下标
来源：http://hz.xuetiantiany.cn/gtwupbezop.html

Py:   arr.index(x);  x in arr
来源：http://hz.chenjidiqi.icu/gtohmgogvc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shuidangran.top/gttaktreey.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.feifeiyinyue.top/gtxocjhfqb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258.top/gtspgpcqiq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.iojbl.cn/gtgrliflvg.html

Go:   slices.Index(arr, x)
来源：http://hz.feifeiyinyue.top/gtdtuqtoia.html

Ruby: arr.index(x)
来源：http://hz.jinqigufen.top/gtskylhbmj.html

C#:   list.IndexOf(x);
来源：http://hz.jyoumei.cn/gtnidrmztq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shzxlz.cn/gtqiclztvy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jqgufenzy.top/gtcjwkpgpo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ywan-chungtsiang.top/gtgpxrlfcs.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangtech.top/gtfgbomzol.html

TS:   arr.filter(x => x > 3)
来源：http://hz.fengsongda.top/gtytdpavvq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.smart0.xyz/gtyxtzkrzy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.haohaochexian.top/gtkobxjpwu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.quarkkingdee.top/gtdgrmzfbt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jqgfzy.top/gteryljqkh.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jianghu66.top/gtdygnwvpf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.birdmap.top/gtkslfnbby.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.andypj.xyz/gtedhoiava.html

JS:   arr.map(x => x * 2)
来源：http://hz.yueranfly.top/gtgdtvfoux.html

TS:   arr.map(x => x * 2)
来源：http://hz.ivvv.top/gtarqjutjj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.chenjidiqi.icu/gtifocsukr.html

Go:   // 手写循环
来源：http://hz.feifeiyinyue.top/gtpwvzbakm.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zycfv.cn/gtkagiuagn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.wangshuangyany.cn/gtmoyvegve.html

[D15] 去重
来源：http://hz.wangshuangyany.cn/gtkusqrulq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ivvv.top/gthdctsoph.html

PHP:  array_unique($arr);
来源：http://hz.smart0.xyz/gtujayuucp.html

JS:   [...new Set(arr)]
来源：http://hz.iojbl.cn/gtfibhybhj.html

TS:   [...new Set(arr)]
来源：http://hz.zdqjudy.top/gtldkyogzv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj20258.top/gtnywpbcmh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cqqwz.cn/gtzvtafmhw.html

Ruby: arr.uniq
来源：http://hz.jiagoushi.top/gtuizukbpd.html

C#:   list.Distinct().ToList()
来源：http://hz.sxryk.cn/gtyxrfqwvz.html

[D16] 求和与平均值
来源：http://hz.sxryk.cn/gthqfdevyz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhiwuduotai.top/gteeaqmdpi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.c1oappe.top/gtsnqnsnts.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.vqdsnc.cn/gtpezxzvxy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yvedp.cn/gtximjlzyr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ivvv.top/gtftmawghb.html

Go:   // 手写循环累加
来源：http://hz.ydzc1.top/gtmzponcec.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.daria6918.cn/gtxkxvqezz.html

C#:   list.Sum();  list.Average()
来源：http://hz.0kj1m.cn/gtkjeygowf.html

[D17] 最大值与最小值
来源：http://hz.tianlin.xyz/gtmjtcdpjy.html

Py:   max(arr);  min(arr)
来源：http://hz.andypj.xyz/gtipuoxfsv.html

PHP:  max($arr);  min($arr);
来源：http://hz.xingfuxueyuan.xyz/gtbwnrmjfm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.feifeiyinyue.top/gtcnchqagw.html

TS:   Math.max(...arr);
来源：http://hz.ydjk.org.cn/gtyrzwetxw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.mhx1999.top/gtuappjszl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj20258.top/gtlihfsipj.html

Ruby: arr.max;  arr.min
来源：http://hz.xinyue.icu/gtkycaehoc.html

C#:   list.Max();  list.Min()
来源：http://hz.cashguo.top/gtouxwzlyy.html

[D18] 扁平化嵌套数组
来源：http://hz.hammf.cn/gtkynmucyv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hammf.cn/gtfguuqjfw.html

PHP:  array_merge(...$nested);
来源：http://hz.bjfxy.top/gtvpmbeggr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.tian-w.cn/gtmskbdlmn.html

TS:   nested.flat();
来源：http://hz.pengpengdd.cyou/gthyeknrur.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dianchejie.cn/gtxseqasnw.html

Go:   // 手写双层循环
来源：http://hz.vqdsnc.cn/gtdunjlhtn.html

Ruby: nested.flatten
来源：http://hz.jinghuilouyu.cn/gtvobkywhb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sxryk.cn/gtivotheyj.html

[D19] 按字段分组
来源：http://hz.snrcjt.cn/gtyfaxfhig.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.wangshuangyany.cn/gtcgqxhlgr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jinyuanbaomall.cn/gtwyoaqqme.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yongpay.top/gtqkpflsjt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ydjk.org.cn/gtqoayrwnr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gogol.net.cn/gtjrxzhhfm.html

Go:   // 手写 map[string][]T
来源：http://hz.yj20258888.top/gtcmhluvue.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hywenlv.cn/gtemlryugo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ydjk.org.cn/gtdfjzderk.html

[D20] 统计每个元素出现次数
来源：http://hz.xylfe.cn/gtxgoceoaw.html

Py:   Counter(arr)
来源：http://hz.sweek.top/gtxtkykjfv.html

PHP:  array_count_values($arr);
来源：http://hz.daxiang520.top/gttutrphvt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tianlin.xyz/gtcaiovhek.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hysaishi.cn/gtxmdhyzxq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sysykeji.top/gttyhjyflh.html

Go:   // 手写 map[T]int
来源：http://hz.haohaochexian.top/gtjkfcmaet.html

Ruby: arr.tally
来源：http://hz.hnqzz.top/gtqcjemild.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jyoumei.cn/gthhrdbslm.html

[D21] 判断是否包含某元素
来源：http://hz.redwolf501.top/gthhltjkfg.html

Py:   x in arr
来源：http://hz.bjfxy.top/gtuvydmdnd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jianghu66.top/gtklutivwd.html

JS:   arr.includes(x)
来源：http://hz.gotoacloud.top/gtrefsinxj.html

TS:   arr.includes(x)
来源：http://hz.xinyue.icu/gtzopkpddi.html

Java: list.contains(x)
来源：http://hz.mhx1999.top/gtkhaqzobi.html

Go:   slices.Contains(arr, x)
来源：http://hz.hywenlv.cn/gtphuwesru.html

Ruby: arr.include?(x)
来源：http://hz.jinqigufen.top/gtuwlndcsz.html

C#:   list.Contains(x)
来源：http://hz.hfpthk.cn/gtumitdbgn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhoulong.xyz/gtysstnqac.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yongpay.top/gtyyctmgze.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jlsjyb.cn/gtbfihxpng.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.316326.xyz/gtrvuubppl.html

TS:   [...arr];
来源：http://hz.mhx1999.top/gtpjkkvpkx.html

Java: new ArrayList<>(list);
来源：http://hz.kuanghao11.cn/gtcfgarswk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jianghu66.top/gtphktkkzv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.haohaochexian.top/gtynrmgutr.html

C#:   new List<int>(list);
来源：http://hz.pengpengdd.cyou/gtvhyywnwi.html

[D23] reduce 累积计算
来源：http://hz.zhongyouzk.top/gtssyggilk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.meibo888.top/gtpbnkxzal.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.dianchejie.cn/gthagbjlsy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhixingplan.top/gtgfnhieqi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.52xcode.cn/gtsknthzpv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xuanzx.com/gtrakdqtgp.html

Go:   // 手写循环
来源：http://hz.ivvv.top/gtqmfefcjv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.aibaodan.cn/gtrgastjzy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.havefunace.top/gtifuigtgl.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenzaomai.com/gtswyglydt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yongpay.top/gtectmfklp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yueranfly.top/gtwbiyasnd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.andypj.xyz/gtysdljjfl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jqgfzy.top/gtgsqdbfnb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cashguo.top/gtgdhuqpda.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cqqwz.cn/gtuorzuznh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yj202588.top/gtotfkmanf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenlongwang.top/gtyjpmbbsi.html

[D25] Set 集合去重与交并差
来源：http://hz.tanke756.top/gtxuqbedvz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.fengsongda.top/gteayqcabu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ydjk.org.cn/gtiqikxaoe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xziqi.cn/gtklzytvkq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ybcxt.top/gtjoptjdrc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.svipenyu.cn/gtcvfhokvq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.birdmap.top/gtafquyeja.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.daxiang520.top/gtxttjwxla.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yuxming.cn/gtstsyxkis.html

[D26] 数组转字符串
来源：http://hz.wangshuangyany.cn/gttxhmeqpx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cdnleiting.top/gtqmluuxnf.html

PHP:  implode(", ", $arr);
来源：http://hz.yj20258888.top/gtorpgrbsk.html

JS:   arr.join(", ")
来源：http://hz.cqqwz.cn/gtgkkjwrjd.html

TS:   arr.join(", ")
来源：http://hz.xziqi.cn/gticpqjuns.html

Java: String.join(", ", list)
来源：http://hz.svipenyu.cn/gtksudrsiv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jqgfzy.top/gtnuvthuvh.html

Ruby: arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtllsttpmj.html

C#:   string.Join(", ", list)
来源：http://hz.gzhubu.top/gtcdjkagvp.html

================================================================================
来源：http://hz.xziqi.cn/gtrtwyqkgh.html

E. 字符串处理
来源：http://hz.yj20258888.top/gtjdtxycqv.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtegsaqzxn.html

[E01] 拼接字符串
来源：http://hz.cucudq.cn/gtujapeifg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.guannengcc.top/gtmaqcjkfi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.quarkkingdee.top/gtupcwtyoe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhaomingkeji.xyz/gtztzslevb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.snrcjt.cn/gtycodhfnk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.daria6918.cn/gtplqzymes.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yonumen.top/gtxkzjeqvi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.aizwys.cn/gtrsqltrvw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yongpay.top/gtccxdbpyo.html

[E02] 重复字符串
来源：http://hz.sufxvd.cn/gtavrsynzc.html

Py:   "ab" * 3
来源：http://hz.kuanghao11.cn/gtfkpflmuf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.daria6918.cn/gtnoanhmcv.html

JS:   "ab".repeat(3)
来源：http://hz.sweek.top/gtoalnbkkq.html

TS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gtkqitvpto.html

Java: "ab".repeat(3)
来源：http://hz.sxryk.cn/gtowqlgpik.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shanyushiyangtech.top/gthecxccmc.html

Ruby: "ab" * 3
来源：http://hz.yueranfly.top/gttwzdopsd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhongyouzk.top/gtrzghgihp.html

[E03] 截取子串
来源：http://hz.jinqigfzy.top/gtfespkbsd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.havefunace.top/gtncunnhxw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hnqzz.top/gtziptlttf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.gogol.net.cn/gtwgqozark.html

TS:   s.slice(1, 4)
来源：http://hz.hnqzz.top/gtalopxxul.html

Java: s.substring(1, 4)
来源：http://hz.cheryme.top/gtksoooukm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jianghu66.top/gtvlytcbyg.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hysaishi.cn/gttubcgtqf.html

C#:   s.Substring(1, 3)
来源：http://hz.xuanzx.com/gtfbqxxiuo.html

[E04] 查找子串位置
来源：http://hz.316326.xyz/gtsahmmuvy.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jqgfzy.top/gtkaeiljwi.html

PHP:  strpos($s, "x");
来源：http://hz.jyoumei.cn/gtwuzodvvw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ywan-chungtsiang.top/gthgljutvq.html

TS:   s.indexOf("x")
来源：http://hz.svipenyu.cn/gtytacfbis.html

Java: s.indexOf("x")
来源：http://hz.gaohongyu789.top/gtgovvihcp.html

Go:   strings.Index(s, "x")
来源：http://hz.havefunace.top/gthfjmyydj.html

Ruby: s.index("x")
来源：http://hz.nanxinkj.top/gtumegvshu.html

C#:   s.IndexOf("x")
来源：http://hz.yj202588.top/gtmxareurs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zycfv.cn/gtwmeuizme.html


<!-- 参考信息 -->