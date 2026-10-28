代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.fzhhl.top/gttdafenfi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.guowangkeji.top/gtpmuoeqod.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.feifeiyinyue.top/gtogscupvr.html

Ruby: # 无泛型
来源：http://hz.gotoacloud.top/gtlgebqtmc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhongyouzk.top/gtoyokwyow.html

[C15] 解构 / 展开参数
来源：http://hz.dianchejie.cn/gtbvsrkyur.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.havefunace.top/gtkookykcm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gzhubu.top/gtbnxiukvi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jqgfzy.top/gtyxievlrz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.sufxvd.cn/gtlovgqaae.html

Java: // 无解构
来源：http://hz.sufxvd.cn/gtrtkdzwcp.html

Go:   // 无解构
来源：http://hz.guowangkeji.top/gtbxmmqiyr.html

Ruby: a, b = pair
来源：http://hz.vqdsnc.cn/gthgblnwvq.html

C#:   var (a, b) = pair;
来源：http://hz.hongshengwenyu.top/gtswtnzibd.html

[C16] 函数 / 方法重载
来源：http://hz.chenzaomai.com/gtyjkxtaqe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenlongwang.top/gtttigzbsu.html

PHP:  // 无重载
来源：http://hz.pycfn.com/gtchncsamq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.mhx1999.top/gtyjnpiuks.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xingfuxueyuan.xyz/gtbxsotfpw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.svipenyu.cn/gtzbmwsimw.html

Go:   // 无重载：用不同函数名
来源：http://hz.c1oappe.top/gtequvaato.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yj202588.top/gtnalhgaqa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhengqikj.top/gtfrhxnbfv.html

================================================================================
来源：http://hz.vqdsnc.cn/gtebsmtqpu.html

D. 数组 / 列表 / 集合
来源：http://hz.smart0.xyz/gtcxfuvopl.html

================================================================================
来源：http://hz.chenlongwang.top/gtrvvgiavj.html

[D01] 创建数组 / 列表
来源：http://hz.zycfv.cn/gtwzgztkgz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinyuanbaomall.cn/gteuvhesyx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yongpay.top/gtnmfqqeyh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shanyushiyangtech.top/gtndzxbhce.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.daxiang520.top/gtabgbhtfv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yvedp.cn/gtjlbntapp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jqgufenzy.top/gtzswjobeh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cheryme.top/gtczhbsxkn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenlongwang.top/gtantkhlnq.html

[D02] 追加元素到末尾
来源：http://hz.ywan-chungtsiang.top/gtxbhctuhb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shzxlz.cn/gtwqnqwaju.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.nanxuanxn.top/gtayukifsn.html

JS:   arr.push(4);
来源：http://hz.aibaodan.cn/gtadaxqiab.html

TS:   arr.push(4);
来源：http://hz.0kj1m.cn/gtzsmugigo.html

Java: list.add(4);
来源：http://hz.hammf.cn/gtkcgbfjfd.html

Go:   arr = append(arr, 4)
来源：http://hz.jyoumei.cn/gtqeijynku.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.svipenyu.cn/gthtepcckc.html

C#:   list.Add(4);
来源：http://hz.pengpengdd.cyou/gtmuxizdga.html

[D03] 在指定位置插入元素
来源：http://hz.gaohongyu789.top/gtoxzntgrc.html

Py:   arr.insert(0, 0)
来源：http://hz.dianchejie.cn/gtfhnoikcu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yonumen.top/gtpahopazu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.9152youxi.cn/gtodqqjvjl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhiwuduotai.top/gtrbdsqnol.html

Java: list.add(0, 0);
来源：http://hz.nwbrower.top/gthyybduay.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cucudq.cn/gtnssbpxde.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shanyushiyangtech.top/gtaamtpoih.html

C#:   list.Insert(0, 0);
来源：http://hz.pengpengdd.cyou/gtfzreavma.html

[D04] 删除元素
来源：http://hz.yongpay.top/gtmajngtvq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xingfuxueyuan.xyz/gtiyrwqeqa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.guowangkeji.top/gthylvrieo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.guowangkeji.top/gtaqwhprfr.html

TS:   arr.splice(0, 1);
来源：http://hz.yvedp.cn/gtxmqccvqq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.iojbl.cn/gtcbbqxyhl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.iojbl.cn/gtqvqwwtoa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hnxiangtu.top/gttxlvafpv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xinyue.icu/gtwommwzqi.html

[D05] 访问与修改元素
来源：http://hz.zhijiandao.cn/gtvckjstei.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuxming.cn/gtflhwhhev.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.52xcode.cn/gtznhhghwg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.nanxuanxn.top/gtzywvbcai.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.daria6918.cn/gtlqfvhxuo.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.0kj1m.cn/gtzoqfoizo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtajygfzal.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtcquyszxb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhaomingkeji.xyz/gtbaywdxzh.html

[D06] 数组长度
来源：http://hz.havefunace.top/gtfnewydwb.html

Py:   len(arr)
来源：http://hz.yj202588.top/gtheffhvoa.html

PHP:  count($arr);
来源：http://hz.zhoulong.xyz/gtnwfpcstd.html

JS:   arr.length
来源：http://hz.hnqzz.top/gtckqsfiyw.html

TS:   arr.length
来源：http://hz.0kj1m.cn/gtlmbwecrt.html

Java: list.size();
来源：http://hz.jinyuanbaomall.cn/gtgdnqunsu.html

Go:   len(arr)
来源：http://hz.hongshengwenyu.top/gtdluldojs.html

Ruby: arr.length; arr.size
来源：http://hz.smart0.xyz/gtozdllqky.html

C#:   list.Count;
来源：http://hz.cashguo.top/gtrpepcvoq.html

[D07] 切片 / 取子数组
来源：http://hz.jqgfzy.top/gtctribidd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.52xcode.cn/gtnsqajjiu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.316326.xyz/gtjihbrgss.html

JS:   arr.slice(1, 4);
来源：http://hz.guannengcc.top/gtupvutzoa.html

TS:   arr.slice(1, 4);
来源：http://hz.guannengcc.top/gthbzzdzli.html

Java: list.subList(1, 4);
来源：http://hz.xinyue.icu/gtrywgrpde.html

Go:   arr[1:4]
来源：http://hz.316326.xyz/gtwfoephys.html

Ruby: arr[1, 3]
来源：http://hz.guowangkeji.top/gtmcfymouk.html

C#:   list.GetRange(1, 3);
来源：http://hz.iojbl.cn/gtvplomebw.html

[D08] 合并两个数组
来源：http://hz.jqgufenzy.top/gtgvfaianz.html

Py:   a + b;  a.extend(b)
来源：http://hz.aibaodan.cn/gtkpjaobey.html

PHP:  array_merge($a, $b);
来源：http://hz.hongshengwenyu.top/gtdebkilel.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ydzc1.top/gtivmczwyz.html

TS:   [...a, ...b];
来源：http://hz.gaohongyu789.top/gtexqplocq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenzaomai.com/gtztnjdjyz.html

Go:   append(a, b...)
来源：http://hz.yuanzhike.top/gttharbvtk.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jianghu66.top/gtarzrmwyq.html

C#:   a.Concat(b).ToList()
来源：http://hz.zycfv.cn/gtufrvmenk.html

[D09] 排序（升序）
来源：http://hz.vqdsnc.cn/gtcyukmcgb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cucudq.cn/gtywixvchz.html

PHP:  sort($arr);
来源：http://hz.meibo888.top/gtdpejzimd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.guannengcc.top/gtyqhyrhhz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.nanxinkj.top/gtgavygmso.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shanyushiyangtech.top/gtmomrfozv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hammf.cn/gtquhixdzt.html

Ruby: arr.sort
来源：http://hz.daxiang520.top/gtxetkixlw.html

C#:   list.Sort();
来源：http://hz.dianchejie.cn/gtudvekywm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.9152youxi.cn/gtwmtaplpi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.dashuyun.cn/gtixazpsuc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xylfe.cn/gtzrzjaedt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daria6918.cn/gtyjdfpook.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgfzy.top/gtfioxxzcd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.feifeiyinyue.top/gtargrozhs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.feifeiyinyue.top/gtiqrqflkk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.daria6918.cn/gtjmnsppdg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xylfe.cn/gtuwcpvnzw.html

[D11] 反转数组
来源：http://hz.andypj.xyz/gtpzalvveq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ivvv.top/gtrjgfsoyl.html

PHP:  array_reverse($arr);
来源：http://hz.sxryk.cn/gteddpyebz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jqgfzy.top/gtekzgtrqz.html

TS:   [...arr].reverse();
来源：http://hz.jqgufenzy.top/gtcixmrtnr.html

Java: Collections.reverse(list);
来源：http://hz.vqdsnc.cn/gthvwghlbl.html

Go:   slices.Reverse(arr)
来源：http://hz.yj20258.top/gtddumbnvb.html

Ruby: arr.reverse
来源：http://hz.cdnleiting.top/gtwniljyvx.html

C#:   list.Reverse();
来源：http://hz.chenzaomai.com/gtommyvmvg.html

[D12] 查找元素下标
来源：http://hz.jinqigfzy.top/gtjfkirrcd.html

Py:   arr.index(x);  x in arr
来源：http://hz.ydzc1.top/gteezjygxb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ppjwa.cn/gtrxftmynv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guowangkeji.top/gtlhbwyteo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yonumen.top/gtavkcjqcw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.smart0.xyz/gtpwnwrviu.html

Go:   slices.Index(arr, x)
来源：http://hz.nwbrower.top/gtsojjddba.html

Ruby: arr.index(x)
来源：http://hz.ivvv.top/gtrmuwotpr.html

C#:   list.IndexOf(x);
来源：http://hz.gotoacloud.top/gtogcqyqas.html

[D13] 过滤（保留满足条件的）
来源：http://hz.iojbl.cn/gtujxdvkir.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ivvv.top/gtjlymjaha.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.vqdsnc.cn/gtjbudaotb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ydjk.org.cn/gtxswexgol.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xziqi.cn/gtvgstlmwr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hfpthk.cn/gtkbgmvigx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ydzc1.top/gtqudffchj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.redwolf501.top/gtqhuuwzct.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.dianchejie.cn/gtmbmsjdzr.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cheryme.top/gtyscazuyx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.chenjidiqi.icu/gtymygwpeo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yj20258888.top/gtefkeexiw.html

JS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gtfkilhoxv.html

TS:   arr.map(x => x * 2)
来源：http://hz.aibaodan.cn/gthrjitynk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.andypj.xyz/gtsurazjtz.html

Go:   // 手写循环
来源：http://hz.wangshuangyany.cn/gtcohzjyul.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yvedp.cn/gttywnugfp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.nanxuanxn.top/gtihmyjier.html

[D15] 去重
来源：http://hz.hammf.cn/gtcjbpvrky.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yj20258888.top/gtbwqfyded.html

PHP:  array_unique($arr);
来源：http://hz.cashguo.top/gtyvehpyed.html

JS:   [...new Set(arr)]
来源：http://hz.yongpay.top/gtdmvkdeaa.html

TS:   [...new Set(arr)]
来源：http://hz.iojbl.cn/gtihosdzfd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zdqjudy.top/gthcygtecv.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zdqjudy.top/gtdxijqlnr.html

Ruby: arr.uniq
来源：http://hz.hywenlv.cn/gtxzuqlyem.html

C#:   list.Distinct().ToList()
来源：http://hz.guannengcc.top/gtayacawod.html

[D16] 求和与平均值
来源：http://hz.zycfv.cn/gtrbjmefss.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.nanxinkj.top/gtbdatzryw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yueranfly.top/gtemnxyfsz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.quarkkingdee.top/gtwzsjaqje.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtadfmkxxt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yuxming.cn/gtwhpjvfge.html

Go:   // 手写循环累加
来源：http://hz.jqgfzy.top/gtlyjibznv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.daxiang520.top/gtgrokrfil.html

C#:   list.Sum();  list.Average()
来源：http://hz.snrcjt.cn/gtkapkzkaz.html

[D17] 最大值与最小值
来源：http://hz.ivvv.top/gtvwynxsnb.html

Py:   max(arr);  min(arr)
来源：http://hz.dashuyun.cn/gtoocjbdae.html

PHP:  max($arr);  min($arr);
来源：http://hz.haohaochexian.top/gtxbuzndif.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ehwqpu.com/gtihkalcuf.html

TS:   Math.max(...arr);
来源：http://hz.pycfn.com/gtsbtiokik.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cheryme.top/gtuyljxcrs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guannengcc.top/gtgylahxsq.html

Ruby: arr.max;  arr.min
来源：http://hz.haohaochexian.top/gtlrwazpzv.html

C#:   list.Max();  list.Min()
来源：http://hz.0kj1m.cn/gtfmrujuok.html

[D18] 扁平化嵌套数组
来源：http://hz.chenlongwang.top/gttkfjgewk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zdqjudy.top/gtdjxikaqq.html

PHP:  array_merge(...$nested);
来源：http://hz.tian-w.cn/gthpbmiapi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.feifeiyinyue.top/gtptitwefc.html

TS:   nested.flat();
来源：http://hz.zhaomingkeji.xyz/gtescvuetj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jqgfzy.top/gtbythwhyy.html

Go:   // 手写双层循环
来源：http://hz.ydjk.org.cn/gtkyucishf.html

Ruby: nested.flatten
来源：http://hz.chenjidiqi.icu/gtzhhnjbxl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.tian-w.cn/gtawjoycnt.html

[D19] 按字段分组
来源：http://hz.chenlongwang.top/gtqslwtemw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sweek.top/gtamtftusq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.iojbl.cn/gthgpzhojt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daxiang520.top/gtnfabbvdg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.c1oappe.top/gtlohwjesq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yonumen.top/gtgtybiwdy.html

Go:   // 手写 map[string][]T
来源：http://hz.fengsongda.top/gtjnbkftan.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shanyushiyangtech.top/gtobmfetxw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.chenjidiqi.icu/gteiahayvz.html

[D20] 统计每个元素出现次数
来源：http://hz.cqqwz.cn/gtsucwnryk.html

Py:   Counter(arr)
来源：http://hz.guannengcc.top/gtrgpzxbsq.html

PHP:  array_count_values($arr);
来源：http://hz.vqdsnc.cn/gtlljvlpfa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pengpengdd.cyou/gtkptevlko.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cdnleiting.top/gtqtqezwgo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.meibo888.top/gtidrsvczd.html

Go:   // 手写 map[T]int
来源：http://hz.0kj1m.cn/gtlgmcktfk.html

Ruby: arr.tally
来源：http://hz.jinqigfzy.top/gtucklmwsy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.haohaochexian.top/gtyzkvyxsl.html

[D21] 判断是否包含某元素
来源：http://hz.bjfxy.top/gtmwibtovv.html

Py:   x in arr
来源：http://hz.shzxlz.cn/gtwjxjqcam.html

PHP:  in_array($x, $arr, true);
来源：http://hz.sweek.top/gtivbhrkxi.html

JS:   arr.includes(x)
来源：http://hz.shzxlz.cn/gtwfdfboif.html

TS:   arr.includes(x)
来源：http://hz.hfpthk.cn/gtieuwgwsg.html

Java: list.contains(x)
来源：http://hz.mhx1999.top/gtfanavzsa.html

Go:   slices.Contains(arr, x)
来源：http://hz.0kj1m.cn/gtcrwjisur.html

Ruby: arr.include?(x)
来源：http://hz.zhaomingkeji.xyz/gtslhzevjo.html

C#:   list.Contains(x)
来源：http://hz.fzhhl.top/gtauhhgsvh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.wangdashe.top/gtnvotebpw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.guannengcc.top/gtpexyhkkq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.wangdashe.top/gtcvdwiotc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.0kj1m.cn/gtlsygbxvm.html

TS:   [...arr];
来源：http://hz.gzhubu.top/gtfvxundrx.html

Java: new ArrayList<>(list);
来源：http://hz.birdmap.top/gtyskkidwe.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hammf.cn/gtnxcuipjy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jyoumei.cn/gtttzdtgrq.html

C#:   new List<int>(list);
来源：http://hz.shanyushiyangtech.top/gthsmwfdvn.html

[D23] reduce 累积计算
来源：http://hz.sufxvd.cn/gtvspmjiko.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.smart0.xyz/gtlpyznefa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhongyouzk.top/gtdqmssral.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.meibo888.top/gttoyfbuju.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guannengcc.top/gtzmtrejjx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shanyushiyangkeji.top/gtkzyhmaoi.html

Go:   // 手写循环
来源：http://hz.yj20258888.top/gtowawzifl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yanxiufei.cn/gtqpnkhhde.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhoulong.xyz/gtwclpetzr.html

[D24] 字典 / Map 基本操作
来源：http://hz.guowangkeji.top/gttjmcepyy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.nanxuanxn.top/gtdkhupiqc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.daxiang520.top/gtiwqhcqnx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.dashuyun.cn/gtulaezhyx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhongyouzk.top/gtyazhwnyj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinghuilouyu.cn/gtwczgedrj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.9152youxi.cn/gtnisggcbw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.pycfn.com/gtsyzjxfzs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hfpthk.cn/gtjbqmhfoz.html

[D25] Set 集合去重与交并差
来源：http://hz.nwbrower.top/gtbzbtymuy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.tianlin.xyz/gtpgzcqnaj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.tian-w.cn/gtvsijybfl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ppjwa.cn/gtighdyiij.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.smart0.xyz/gtswdniool.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.smart0.xyz/gtkglaakox.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.gogol.net.cn/gtqnaqeitw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hongshengwenyu.top/gtaayqtwso.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.fengsongda.top/gtkaszirgd.html

[D26] 数组转字符串
来源：http://hz.fengsongda.top/gtngkqgoce.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hnqzz.top/gtximluceo.html

PHP:  implode(", ", $arr);
来源：http://hz.meibo888.top/gtmfobkrha.html

JS:   arr.join(", ")
来源：http://hz.wangdashe.top/gtykwrhgir.html

TS:   arr.join(", ")
来源：http://hz.jinqigufen.top/gtzhoeetgj.html

Java: String.join(", ", list)
来源：http://hz.jinyuanbaomall.cn/gtbipyfesl.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jiagoushi.top/gtlvdnsvfv.html

Ruby: arr.join(", ")
来源：http://hz.xingfuxueyuan.xyz/gtyljxyomo.html

C#:   string.Join(", ", list)
来源：http://hz.ppjwa.cn/gtzsmveigj.html

================================================================================
来源：http://hz.pycfn.com/gtothuxehc.html

E. 字符串处理
来源：http://hz.haohaochexian.top/gtsseeppwe.html

================================================================================
来源：http://hz.yongpay.top/gtlfdnyvnk.html

[E01] 拼接字符串
来源：http://hz.yueranfly.top/gteggonfgq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cashguo.top/gtipqazmww.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shangyingyoupin.top/gtrjdapmmz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gtfwmhqucq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.iojbl.cn/gtbvanzpnw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xuetiantiany.cn/gtbbtetxul.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.havefunace.top/gtxxxfitlv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jianghu66.top/gtulstzyyf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ivvv.top/gtlimmrbmv.html

[E02] 重复字符串
来源：http://hz.jinghuilouyu.cn/gtixmstnnk.html

Py:   "ab" * 3
来源：http://hz.smart0.xyz/gtdigobntz.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhiwuduotai.top/gtyndkpcfz.html

JS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gtlhnhxdbg.html

TS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtbspiavlg.html

Java: "ab".repeat(3)
来源：http://hz.nwbrower.top/gtvvqfdnrj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhixingplan.top/gtmzcnuplg.html

Ruby: "ab" * 3
来源：http://hz.wangdashe.top/gtmlgmfmyp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.wangdashe.top/gttrdjcdmn.html

[E03] 截取子串
来源：http://hz.nanxuanxn.top/gtqmtunnrp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xylfe.cn/gtsrzhfnhj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhijiandao.cn/gtfvguqurf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhijiandao.cn/gteorhhklx.html

TS:   s.slice(1, 4)
来源：http://hz.nanxinkj.top/gtxjwusazz.html

Java: s.substring(1, 4)
来源：http://hz.yongpay.top/gtbqoxqkop.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hnqzz.top/gtqtarvuvz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gogol.net.cn/gtooaywomc.html

C#:   s.Substring(1, 3)
来源：http://hz.hnxiangtu.top/gtgyzkuwvo.html

[E04] 查找子串位置
来源：http://hz.snrcjt.cn/gtdnofluag.html

Py:   s.find("x");  s.index("x")
来源：http://hz.chenlongwang.top/gtxlgafpqw.html

PHP:  strpos($s, "x");
来源：http://hz.316326.xyz/gtnnrngnmr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.nanxuanxn.top/gtlpucyitq.html

TS:   s.indexOf("x")
来源：http://hz.jqgufenzy.top/gtxtgzuhhp.html

Java: s.indexOf("x")
来源：http://hz.sweek.top/gtqudqcfjl.html

Go:   strings.Index(s, "x")
来源：http://hz.jlsjyb.cn/gthefyqayh.html

Ruby: s.index("x")
来源：http://hz.jianghu66.top/gttnliqgso.html

C#:   s.IndexOf("x")
来源：http://hz.jlsjyb.cn/gtzsdombvj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zycfv.cn/gtpztkpxks.html


<!-- 参考信息 -->