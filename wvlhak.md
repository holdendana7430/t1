代发 wailian999

PHP:  // 无重载
来源：http://hz.guowangkeji.top/gtvprcaazy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gzhubu.top/gtnreocqtt.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hywenlv.cn/gtgormonbb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.0kj1m.cn/gthghrvpqk.html

Go:   // 无重载：用不同函数名
来源：http://hz.pycfn.com/gtsxvxnths.html

Ruby: # 无重载：靠动态参数
来源：http://hz.dianchejie.cn/gtamlkdzsq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhaomingkeji.xyz/gtsoxuoyjz.html

================================================================================
来源：http://hz.ppjwa.cn/gtvmrazqfj.html

D. 数组 / 列表 / 集合
来源：http://hz.yueranfly.top/gtyqyjvnob.html

================================================================================
来源：http://hz.guowangkeji.top/gtzeffdmqn.html

[D01] 创建数组 / 列表
来源：http://hz.daxiang520.top/gtevmwlqqm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenlongwang.top/gttrsqvcrq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hongshengwenyu.top/gthioagmhk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yueranfly.top/gtlwwzdtjn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xziqi.cn/gtuibmmpho.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.havefunace.top/gtjthxwzdf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zycfv.cn/gtpkdnvxct.html

Ruby: arr = [1, 2, 3]
来源：http://hz.tianlin.xyz/gtinezpdvk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.redwolf501.top/gtmcjikrwq.html

[D02] 追加元素到末尾
来源：http://hz.iojbl.cn/gtqryfbacg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.0kj1m.cn/gtwwhhrbkp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ppjwa.cn/gtpbbrmsyg.html

JS:   arr.push(4);
来源：http://hz.gzhubu.top/gtdvglkqoi.html

TS:   arr.push(4);
来源：http://hz.ehwqpu.com/gtlgwgrkhy.html

Java: list.add(4);
来源：http://hz.aizwys.cn/gtrskxydjc.html

Go:   arr = append(arr, 4)
来源：http://hz.chenjidiqi.icu/gtlnobhyvq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.c1oappe.top/gtuszqbfbe.html

C#:   list.Add(4);
来源：http://hz.meibo888.top/gtbocrhtsz.html

[D03] 在指定位置插入元素
来源：http://hz.tian-w.cn/gtghouanqt.html

Py:   arr.insert(0, 0)
来源：http://hz.snrcjt.cn/gtfrikxqfp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.nwbrower.top/gtsmhntwez.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xinyue.icu/gtcnlrvwvc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.9152youxi.cn/gtvxvbswtx.html

Java: list.add(0, 0);
来源：http://hz.jianghu66.top/gtdlgmetib.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhongyouzk.top/gtdzscuswo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cashguo.top/gtddncrkfz.html

C#:   list.Insert(0, 0);
来源：http://hz.ehwqpu.com/gtgafsezwy.html

[D04] 删除元素
来源：http://hz.wangshuangyany.cn/gtcnqwewvf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xingfuxueyuan.xyz/gtltzambxi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jianghu66.top/gtargiufmi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sysykeji.top/gtbawhgjkx.html

TS:   arr.splice(0, 1);
来源：http://hz.hongshengwenyu.top/gtjisbgica.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.nanxinkj.top/gtipvuppoj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gogol.net.cn/gtlwfuzyft.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.vqdsnc.cn/gttzrwkreq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.smart0.xyz/gtnejhwbrz.html

[D05] 访问与修改元素
来源：http://hz.guowangkeji.top/gtkiiiepqh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ybcxt.top/gtkrcatapz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.nanxinkj.top/gthmtlrplw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sweek.top/gtgtaoikwr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yangfankeji.com/gtciialadt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.9152youxi.cn/gtdqfcucir.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.bjfxy.top/gtwmgjxuhg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sufxvd.cn/gtravynxir.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.svipenyu.cn/gtkeqrtlar.html

[D06] 数组长度
来源：http://hz.ydjk.org.cn/gtqvrzenww.html

Py:   len(arr)
来源：http://hz.jinqigfzy.top/gtagubpsry.html

PHP:  count($arr);
来源：http://hz.zdqjudy.top/gteefinjal.html

JS:   arr.length
来源：http://hz.jianghu66.top/gtqblzmfyt.html

TS:   arr.length
来源：http://hz.jianghu66.top/gtuvbuwewt.html

Java: list.size();
来源：http://hz.jianghu66.top/gtkwbajyba.html

Go:   len(arr)
来源：http://hz.feifeiyinyue.top/gteptkwenm.html

Ruby: arr.length; arr.size
来源：http://hz.zhijiandao.cn/gtqmhxvpjy.html

C#:   list.Count;
来源：http://hz.sysykeji.top/gtwrlsfwwq.html

[D07] 切片 / 取子数组
来源：http://hz.cashguo.top/gtcpvihdkw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.iojbl.cn/gtfawkiemx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sxryk.cn/gtcwpusjwx.html

JS:   arr.slice(1, 4);
来源：http://hz.zycfv.cn/gtgyxrjnjv.html

TS:   arr.slice(1, 4);
来源：http://hz.snrcjt.cn/gtzkapjnui.html

Java: list.subList(1, 4);
来源：http://hz.ydjk.org.cn/gtivhmnkhg.html

Go:   arr[1:4]
来源：http://hz.hywenlv.cn/gtsrfhxkqw.html

Ruby: arr[1, 3]
来源：http://hz.316326.xyz/gtisnfmolc.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhaomingkeji.xyz/gtyfnpdjcr.html

[D08] 合并两个数组
来源：http://hz.ppjwa.cn/gtdxutfghr.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj20258888.top/gtjfgcxivd.html

PHP:  array_merge($a, $b);
来源：http://hz.jyoumei.cn/gtkfmroocd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinghuilouyu.cn/gtvkfyqpoq.html

TS:   [...a, ...b];
来源：http://hz.xuetiantiany.cn/gttitwtzyz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenzaomai.com/gtwrtlvpbk.html

Go:   append(a, b...)
来源：http://hz.yueranfly.top/gthtcwyibo.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yanxiufei.cn/gtovmjjalp.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhaomingkeji.xyz/gthipthqfb.html

[D09] 排序（升序）
来源：http://hz.sxryk.cn/gteuoxyvby.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangshuangyany.cn/gtqaxgmqtf.html

PHP:  sort($arr);
来源：http://hz.zhengqikj.top/gtgkfmcgtr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj20258.top/gtzpmbxeze.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.redwolf501.top/gtkoqhtmok.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.vqdsnc.cn/gtbzmrbsvm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.daria6918.cn/gtkabiyijt.html

Ruby: arr.sort
来源：http://hz.yueranfly.top/gtiqgzpvjz.html

C#:   list.Sort();
来源：http://hz.quarkkingdee.top/gtrhcfshad.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sufxvd.cn/gtbsvfdzxb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.birdmap.top/gtdbmphnlt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.bjfxy.top/gtlblydvpc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.redwolf501.top/gtjujzigpu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hywenlv.cn/gtdfdmcttu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.pengpengdd.cyou/gtkbokihue.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.chenlongwang.top/gtkguhbddt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cheryme.top/gtxhoeecuy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.fengsongda.top/gtxireowyh.html

[D11] 反转数组
来源：http://hz.9152youxi.cn/gtuxbooube.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.chenlongwang.top/gtbvelargv.html

PHP:  array_reverse($arr);
来源：http://hz.shanyushiyangkeji.top/gtwlptlckf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.smart0.xyz/gtgpeflmmk.html

TS:   [...arr].reverse();
来源：http://hz.zhongyouzk.top/gtjdptddxy.html

Java: Collections.reverse(list);
来源：http://hz.nwbrower.top/gtpspryybe.html

Go:   slices.Reverse(arr)
来源：http://hz.cdnleiting.top/gtekiekegx.html

Ruby: arr.reverse
来源：http://hz.zhixingplan.top/gtuokpdjxp.html

C#:   list.Reverse();
来源：http://hz.mhx1999.top/gtxjezmfuo.html

[D12] 查找元素下标
来源：http://hz.ppjwa.cn/gtjrjcowss.html

Py:   arr.index(x);  x in arr
来源：http://hz.xziqi.cn/gtvhwniwjq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.iojbl.cn/gttusbnxmu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pycfn.com/gtkrhbdjes.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.mhx1999.top/gtfvkobcby.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.52xcode.cn/gtegvftfdy.html

Go:   slices.Index(arr, x)
来源：http://hz.zhengqikj.top/gtvfwnfjij.html

Ruby: arr.index(x)
来源：http://hz.jqgufenzy.top/gttiisyfms.html

C#:   list.IndexOf(x);
来源：http://hz.yj20258888.top/gtivtdcxmo.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hysaishi.cn/gtfgotuyaq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cashguo.top/gtjfxdxzqs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.bjfxy.top/gtvxndlcvi.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jiagoushi.top/gtjjyzerxq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.havefunace.top/gtxjclexqq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shzxlz.cn/gttqvlfilv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.pengpengdd.cyou/gtxznwhiqh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sysykeji.top/gtswonxdmk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xuetiantiany.cn/gthbmlejuo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.meibo888.top/gtmisufwne.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.9152youxi.cn/gtwurpgtcv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.quarkkingdee.top/gttdzxcmzk.html

JS:   arr.map(x => x * 2)
来源：http://hz.jinyuanbaomall.cn/gtcywdlovf.html

TS:   arr.map(x => x * 2)
来源：http://hz.gotoacloud.top/gttnuoiqmu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gaohongyu789.top/gtrxnxwfmz.html

Go:   // 手写循环
来源：http://hz.gzhubu.top/gtfkscngvh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.52xcode.cn/gtyjycphwz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.chenzaomai.com/gtcowwjymr.html

[D15] 去重
来源：http://hz.meibo888.top/gtpzwujaej.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.meibo888.top/gtpklwjozq.html

PHP:  array_unique($arr);
来源：http://hz.mhx1999.top/gtnsemmnwe.html

JS:   [...new Set(arr)]
来源：http://hz.nanxuanxn.top/gthdysxiei.html

TS:   [...new Set(arr)]
来源：http://hz.gzhubu.top/gtfiigczfc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xuetiantiany.cn/gttrtpltsq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hywenlv.cn/gtibvtmdxg.html

Ruby: arr.uniq
来源：http://hz.havefunace.top/gtjjnijfzs.html

C#:   list.Distinct().ToList()
来源：http://hz.cheryme.top/gtijldgxot.html

[D16] 求和与平均值
来源：http://hz.jinyuanbaomall.cn/gtfsoaepni.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.9152youxi.cn/gtcaapsatr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fengsongda.top/gtniuercwh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dianchejie.cn/gtcfbvjbvn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dashuyun.cn/gtwcboplcr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ehwqpu.com/gtsqwlscqh.html

Go:   // 手写循环累加
来源：http://hz.xinyue.icu/gttbzqlsmo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sysykeji.top/gtbmaobgnv.html

C#:   list.Sum();  list.Average()
来源：http://hz.pycfn.com/gtjljgfevx.html

[D17] 最大值与最小值
来源：http://hz.yangfankeji.com/gtpjhcbure.html

Py:   max(arr);  min(arr)
来源：http://hz.xuetiantiany.cn/gtdyrsqngi.html

PHP:  max($arr);  min($arr);
来源：http://hz.ehwqpu.com/gtlrbxaqee.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xuetiantiany.cn/gtvnxotlvj.html

TS:   Math.max(...arr);
来源：http://hz.zhiwuduotai.top/gtavzzeoej.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yuanzhike.top/gtbalnuudm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gzhubu.top/gtzqenhxms.html

Ruby: arr.max;  arr.min
来源：http://hz.bjfxy.top/gtwjtdxhwf.html

C#:   list.Max();  list.Min()
来源：http://hz.chenjidiqi.icu/gttovnhspb.html

[D18] 扁平化嵌套数组
来源：http://hz.hysaishi.cn/gtjfsacbwn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.kuanghao11.cn/gtxgdzrlee.html

PHP:  array_merge(...$nested);
来源：http://hz.xingfuxueyuan.xyz/gtfqtdigop.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.snrcjt.cn/gttivriwrv.html

TS:   nested.flat();
来源：http://hz.redwolf501.top/gtayylfwfv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenjidiqi.icu/gtquvmtnhr.html

Go:   // 手写双层循环
来源：http://hz.guannengcc.top/gtbgmorban.html

Ruby: nested.flatten
来源：http://hz.dianchejie.cn/gtxhnqxvuq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yuxming.cn/gtdczxuydh.html

[D19] 按字段分组
来源：http://hz.hfpthk.cn/gtmscuaqej.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cqqwz.cn/gtgfpigmdz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ybcxt.top/gtgqxphmrb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinghuilouyu.cn/gtwuwiuixj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.daxiang520.top/gtpnsrhuix.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shzxlz.cn/gthwulhhhm.html

Go:   // 手写 map[string][]T
来源：http://hz.hongshengwenyu.top/gtxszghjdz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.kuanghao11.cn/gtcivpfmfh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jlsjyb.cn/gtpkfueini.html

[D20] 统计每个元素出现次数
来源：http://hz.xylfe.cn/gtnmqpehfj.html

Py:   Counter(arr)
来源：http://hz.ydjk.org.cn/gttvcusbgu.html

PHP:  array_count_values($arr);
来源：http://hz.shangyingyoupin.top/gtbbtqoddy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sxryk.cn/gtejxbswtg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hongshengwenyu.top/gtjqubpbbk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cdnleiting.top/gtuphkadhb.html

Go:   // 手写 map[T]int
来源：http://hz.yueranfly.top/gtyemljshk.html

Ruby: arr.tally
来源：http://hz.bjfxy.top/gthaannjdu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.daxiang520.top/gtllejqtnf.html

[D21] 判断是否包含某元素
来源：http://hz.bjfxy.top/gthstffwbm.html

Py:   x in arr
来源：http://hz.yuanzhike.top/gtjfdngmhh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.fzhhl.top/gtzegceugc.html

JS:   arr.includes(x)
来源：http://hz.nwbrower.top/gtrtnznrzx.html

TS:   arr.includes(x)
来源：http://hz.tianlin.xyz/gtzrvufuah.html

Java: list.contains(x)
来源：http://hz.hongshengwenyu.top/gtfovtnmnb.html

Go:   slices.Contains(arr, x)
来源：http://hz.xylfe.cn/gtlmpaiklq.html

Ruby: arr.include?(x)
来源：http://hz.0kj1m.cn/gtndemknzo.html

C#:   list.Contains(x)
来源：http://hz.meibo888.top/gtmslpmxba.html

[D22] 复制数组（避免共享引用）
来源：http://hz.smart0.xyz/gtmbjzkwdx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ivvv.top/gtlpuqeobo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yj20258888.top/gtmqdifskc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.52xcode.cn/gtooqiohdk.html

TS:   [...arr];
来源：http://hz.sxryk.cn/gttneiwikg.html

Java: new ArrayList<>(list);
来源：http://hz.ydjk.org.cn/gtjlsxeahf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jianghu66.top/gtadjwvutd.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ybcxt.top/gtumpwlqgy.html

C#:   new List<int>(list);
来源：http://hz.shangyingyoupin.top/gtnmtawimc.html

[D23] reduce 累积计算
来源：http://hz.jqgfzy.top/gtkzlvoqsx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.guowangkeji.top/gtkxqiukzx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.haohaochexian.top/gtfjuzhrmq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangkeji.top/gtvidrmnsf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cheryme.top/gtvnelnsoh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gogol.net.cn/gtfboyhpop.html

Go:   // 手写循环
来源：http://hz.jqgfzy.top/gtlbtmynvm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.iojbl.cn/gtyurafovj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.snrcjt.cn/gtkgrfdnyu.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinghuilouyu.cn/gtprixprui.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yongpay.top/gtbsaphlzq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.0kj1m.cn/gtiooyrtkz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.daria6918.cn/gtigvbdzcw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jiagoushi.top/gtglkctjmu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shuidangran.top/gtgcwaoexa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.wangshuangyany.cn/gtxsfphisv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ybcxt.top/gtpxsskyrw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhixingplan.top/gtgzgeuzvm.html

[D25] Set 集合去重与交并差
来源：http://hz.nanxinkj.top/gtcxnqoppj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jinqigufen.top/gtnhdmgeqw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xingfuxueyuan.xyz/gtbrejwkrd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhengqikj.top/gtudqnexzl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gotoacloud.top/gtdzjcxjyd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hongshengwenyu.top/gtzwxvatah.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xuetiantiany.cn/gtrzrzfytg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.316326.xyz/gtwdmwctqx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.andypj.xyz/gthuukanvx.html

[D26] 数组转字符串
来源：http://hz.52xcode.cn/gtsotivcgk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.havefunace.top/gtzkontpxq.html

PHP:  implode(", ", $arr);
来源：http://hz.jinghuilouyu.cn/gttqbdniky.html

JS:   arr.join(", ")
来源：http://hz.zhijiandao.cn/gttxiwugse.html

TS:   arr.join(", ")
来源：http://hz.yongpay.top/gtdnlktioh.html

Java: String.join(", ", list)
来源：http://hz.svipenyu.cn/gtnvtvogqf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jiagoushi.top/gttbcxhfzx.html

Ruby: arr.join(", ")
来源：http://hz.zhiwuduotai.top/gteklmqrks.html

C#:   string.Join(", ", list)
来源：http://hz.jinqigufen.top/gtfkhedxaa.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtqvsapacu.html

E. 字符串处理
来源：http://hz.fzhhl.top/gtafwbmzbj.html

================================================================================
来源：http://hz.zhoulong.xyz/gtlbtthvbq.html

[E01] 拼接字符串
来源：http://hz.yongpay.top/gtutxdegqy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cqqwz.cn/gtgralfpkm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhengqikj.top/gtekchecbj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hysaishi.cn/gturrgxwvh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aibaodan.cn/gtxrnfmehn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shzxlz.cn/gtjapvydcd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.svipenyu.cn/gtjhxafrqx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jqgfzy.top/gtpcoxgsxi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cdnleiting.top/gtczotdvce.html

[E02] 重复字符串
来源：http://hz.zdqjudy.top/gtzztyrcsn.html

Py:   "ab" * 3
来源：http://hz.ivvv.top/gtdddavgkg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fengsongda.top/gtvqhhbxaa.html

JS:   "ab".repeat(3)
来源：http://hz.cashguo.top/gtbikwspob.html

TS:   "ab".repeat(3)
来源：http://hz.kuanghao11.cn/gtoxsawufa.html

Java: "ab".repeat(3)
来源：http://hz.yvedp.cn/gtcsccylvs.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.52xcode.cn/gtsgwyckow.html

Ruby: "ab" * 3
来源：http://hz.vqdsnc.cn/gthvkjkdtd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinghuilouyu.cn/gtlmdiqpxw.html

[E03] 截取子串
来源：http://hz.hongshengwenyu.top/gtzjfrwpsr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ivvv.top/gtqfaurgft.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hfpthk.cn/gtrcxmgykk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hfpthk.cn/gtampdaaav.html

TS:   s.slice(1, 4)
来源：http://hz.yj20258888.top/gtpunxzjpf.html

Java: s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtucvadgxo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yj20258888.top/gtnollpiay.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yj202588.top/gtdjdvrwxb.html

C#:   s.Substring(1, 3)
来源：http://hz.wangshuangyany.cn/gtbwodqcod.html

[E04] 查找子串位置
来源：http://hz.ppjwa.cn/gtsdpkiwql.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ivvv.top/gtzcyeuceg.html

PHP:  strpos($s, "x");
来源：http://hz.daria6918.cn/gtcyojnezs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hywenlv.cn/gtfezpmiba.html

TS:   s.indexOf("x")
来源：http://hz.yj20258.top/gthfuzfqqp.html

Java: s.indexOf("x")
来源：http://hz.cashguo.top/gtzkmxwjhv.html

Go:   strings.Index(s, "x")
来源：http://hz.haohaochexian.top/gtuevcxbmu.html

Ruby: s.index("x")
来源：http://hz.dianchejie.cn/gtjlazkuko.html

C#:   s.IndexOf("x")
来源：http://hz.52xcode.cn/gtjsavopzg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xuetiantiany.cn/gtlbqzcxqx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ydjk.org.cn/gtcuqqlldg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ydzc1.top/gtvgpdwnce.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.meibo888.top/gtelyjnpja.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.iojbl.cn/gtncxeukmr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.smart0.xyz/gtogkgntpp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yvedp.cn/gthkjkzjmg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.guowangkeji.top/gtfmuplgwr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.chenzaomai.com/gtwuxpaktg.html

[E06] 替换子串
来源：http://hz.hysaishi.cn/gtyxwplsde.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.redwolf501.top/gtdnwhxmnc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.mhx1999.top/gtcaivwzqs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgfzy.top/gtyfercpfb.html

TS:   s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtsmysmced.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gtxmkfmgmi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinqigufen.top/gtzzdqxoyh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cashguo.top/gtizoqewyd.html


<!-- 参考信息 -->