代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yanxiufei.cn/gthihloavx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yj20258.top/gtzsknluun.html

Java: // 无解构
来源：http://hz.hongshengwenyu.top/gtqfcflbxj.html

Go:   // 无解构
来源：http://hz.jiagoushi.top/gtvdftgpwu.html

Ruby: a, b = pair
来源：http://hz.hysaishi.cn/gtnwonxiam.html

C#:   var (a, b) = pair;
来源：http://hz.yuanzhike.top/gtfsfaukyy.html

[C16] 函数 / 方法重载
来源：http://hz.daria6918.cn/gtxggbujqa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.wangshuangyany.cn/gtixtjqwdk.html

PHP:  // 无重载
来源：http://hz.cdnleiting.top/gtntdanifx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jlsjyb.cn/gtjdnqcjol.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.fengsongda.top/gtinixcvjk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ybcxt.top/gthhfcguxy.html

Go:   // 无重载：用不同函数名
来源：http://hz.zycfv.cn/gtdvuptjlp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sxryk.cn/gtdwbtpscb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.meibo888.top/gtfpppugar.html

================================================================================
来源：http://hz.316326.xyz/gtzanywyea.html

D. 数组 / 列表 / 集合
来源：http://hz.ydjk.org.cn/gttbgdzkkz.html

================================================================================
来源：http://hz.zhongyouzk.top/gtfhzhapic.html

[D01] 创建数组 / 列表
来源：http://hz.shanyushiyangkeji.top/gtpydiihat.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.gotoacloud.top/gtzmcgolus.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.daxiang520.top/gtnvvmvjkk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hongshengwenyu.top/gtxorovqqb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj202588.top/gtmposdvdp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.gogol.net.cn/gtjalkntzl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sysykeji.top/gtsugppkxm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhijiandao.cn/gtjmhasbkp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgfzy.top/gtwbowukou.html

[D02] 追加元素到末尾
来源：http://hz.wangdashe.top/gtycceqmfu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ivvv.top/gtmujjjadh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.aibaodan.cn/gtvlqhtyok.html

JS:   arr.push(4);
来源：http://hz.hywenlv.cn/gtdmpmoqzb.html

TS:   arr.push(4);
来源：http://hz.jinqigufen.top/gteuyfffxw.html

Java: list.add(4);
来源：http://hz.havefunace.top/gtxrousdvh.html

Go:   arr = append(arr, 4)
来源：http://hz.sweek.top/gtbqxpvdxf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xziqi.cn/gtrrionxve.html

C#:   list.Add(4);
来源：http://hz.xziqi.cn/gtwjedtjju.html

[D03] 在指定位置插入元素
来源：http://hz.zhongyouzk.top/gtapircqhm.html

Py:   arr.insert(0, 0)
来源：http://hz.zhongyouzk.top/gtirdwepjh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gogol.net.cn/gtrzwqnrkd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jiagoushi.top/gtzhoupcrc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cheryme.top/gtskgofrwg.html

Java: list.add(0, 0);
来源：http://hz.sysykeji.top/gtfhggwvgd.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yj20258888.top/gtrejthwip.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj20258.top/gtyabwrctu.html

C#:   list.Insert(0, 0);
来源：http://hz.zhengqikj.top/gtpopdujqw.html

[D04] 删除元素
来源：http://hz.sysykeji.top/gttokpxmej.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.svipenyu.cn/gtuehtaypk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.316326.xyz/gthexorhwq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gaohongyu789.top/gtnqnyaako.html

TS:   arr.splice(0, 1);
来源：http://hz.iojbl.cn/gtudyqzbwg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xziqi.cn/gtjbweyyqx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yueranfly.top/gtwqkyiset.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xuetiantiany.cn/gtdzmlgggc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yangfankeji.com/gtuvckkdhb.html

[D05] 访问与修改元素
来源：http://hz.yj202588.top/gtjyrtkxkk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtzowaoaqb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ydzc1.top/gtzcrzesrf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yj202588.top/gtrzlfwgjb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhengqikj.top/gtlngggasb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yanxiufei.cn/gtcdnqiihj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtyqhchkgv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shzxlz.cn/gtuomxvosv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.quarkkingdee.top/gtlhsfkyta.html

[D06] 数组长度
来源：http://hz.cqqwz.cn/gtqxwnkllh.html

Py:   len(arr)
来源：http://hz.smart0.xyz/gtnxueohwg.html

PHP:  count($arr);
来源：http://hz.mhx1999.top/gtzhazustr.html

JS:   arr.length
来源：http://hz.iojbl.cn/gtifrlkvlv.html

TS:   arr.length
来源：http://hz.sweek.top/gtwthkxdtz.html

Java: list.size();
来源：http://hz.hnqzz.top/gtgllxmgfv.html

Go:   len(arr)
来源：http://hz.birdmap.top/gtzezowjga.html

Ruby: arr.length; arr.size
来源：http://hz.daxiang520.top/gtvkjvhyfi.html

C#:   list.Count;
来源：http://hz.guowangkeji.top/gtvyseveug.html

[D07] 切片 / 取子数组
来源：http://hz.daria6918.cn/gtbuncuzdw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xingfuxueyuan.xyz/gtkawkvoxz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.svipenyu.cn/gtxqgtmzqi.html

JS:   arr.slice(1, 4);
来源：http://hz.9152youxi.cn/gttylqsshi.html

TS:   arr.slice(1, 4);
来源：http://hz.jinghuilouyu.cn/gtegkitpgp.html

Java: list.subList(1, 4);
来源：http://hz.daxiang520.top/gtvlfauocl.html

Go:   arr[1:4]
来源：http://hz.cqqwz.cn/gtjwxmhekp.html

Ruby: arr[1, 3]
来源：http://hz.jianghu66.top/gtxymcsoea.html

C#:   list.GetRange(1, 3);
来源：http://hz.hnxiangtu.top/gttzqmnuwk.html

[D08] 合并两个数组
来源：http://hz.zhijiandao.cn/gtycmpteju.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhiwuduotai.top/gtqxdjxguy.html

PHP:  array_merge($a, $b);
来源：http://hz.ybcxt.top/gtjabzxqhg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cashguo.top/gtygdkuomk.html

TS:   [...a, ...b];
来源：http://hz.cheryme.top/gtgnnnrycz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.meibo888.top/gtflkmdrgh.html

Go:   append(a, b...)
来源：http://hz.yuxming.cn/gtfaijkrxu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sufxvd.cn/gthjeyoxxq.html

C#:   a.Concat(b).ToList()
来源：http://hz.jqgufenzy.top/gtmzfxliun.html

[D09] 排序（升序）
来源：http://hz.9152youxi.cn/gtszcuszbp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.snrcjt.cn/gtvrtdihcb.html

PHP:  sort($arr);
来源：http://hz.zhongyouzk.top/gtnrdzcrei.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jlsjyb.cn/gtsgoygnug.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hywenlv.cn/gtuybkruqz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shanyushiyangkeji.top/gtkkzhtdyy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yongpay.top/gtnczxllct.html

Ruby: arr.sort
来源：http://hz.andypj.xyz/gtblesghvw.html

C#:   list.Sort();
来源：http://hz.shanyushiyangtech.top/gtgkpsqllg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinqigfzy.top/gtbfvxkvkv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shzxlz.cn/gtdigkoxxr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shanyushiyangkeji.top/gtjzslhpik.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhoulong.xyz/gtaxyohncf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fengsongda.top/gtvmnqytev.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sweek.top/gtcmrrdela.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jlsjyb.cn/gtqcymnwws.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tianlin.xyz/gtjylvelaj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhijiandao.cn/gtjtfbzjxq.html

[D11] 反转数组
来源：http://hz.jyoumei.cn/gthhacdmkm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhiwuduotai.top/gttygurqjg.html

PHP:  array_reverse($arr);
来源：http://hz.smart0.xyz/gthyrforuo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.feifeiyinyue.top/gtwybpacii.html

TS:   [...arr].reverse();
来源：http://hz.ydjk.org.cn/gtwapciajw.html

Java: Collections.reverse(list);
来源：http://hz.zhengqikj.top/gtimeplecn.html

Go:   slices.Reverse(arr)
来源：http://hz.yj20258888.top/gtbketobxz.html

Ruby: arr.reverse
来源：http://hz.cheryme.top/gtaahrtxjq.html

C#:   list.Reverse();
来源：http://hz.smart0.xyz/gtqeenanwx.html

[D12] 查找元素下标
来源：http://hz.zhiwuduotai.top/gtmvxvoyog.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhixingplan.top/gtayoqjypn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.wangshuangyany.cn/gtaohxwjef.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ivvv.top/gtdmfsrazn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtzubuouug.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hongshengwenyu.top/gtwzraqbif.html

Go:   slices.Index(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtnawyajlu.html

Ruby: arr.index(x)
来源：http://hz.vqdsnc.cn/gtlfjwgpfe.html

C#:   list.IndexOf(x);
来源：http://hz.yonumen.top/gttwswaosj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hammf.cn/gtksqybtmz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ydzc1.top/gtipujawlh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.52xcode.cn/gtydnqjvos.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinyuanbaomall.cn/gtwntsqpcp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.kuanghao11.cn/gtfcxuajfj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ybcxt.top/gtfiizxihl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shzxlz.cn/gtszgzebfp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hnxiangtu.top/gtexcrvmem.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.vqdsnc.cn/gtdbdunftu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinyuanbaomall.cn/gtmvfjpoqn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.gogol.net.cn/gtmlaetpin.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yonumen.top/gtttalocwg.html

JS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gteluwabcd.html

TS:   arr.map(x => x * 2)
来源：http://hz.xinyue.icu/gtotwzbdmn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gogol.net.cn/gtggtnkqkq.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtgbdssvrz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hongshengwenyu.top/gtztrumyxc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zycfv.cn/gtrglxjfqi.html

[D15] 去重
来源：http://hz.wangshuangyany.cn/gtberoutsi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.quarkkingdee.top/gtxughftxu.html

PHP:  array_unique($arr);
来源：http://hz.zycfv.cn/gtsissjxic.html

JS:   [...new Set(arr)]
来源：http://hz.ivvv.top/gtwizivybu.html

TS:   [...new Set(arr)]
来源：http://hz.svipenyu.cn/gtmqcodymr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnxiangtu.top/gtrdohxmup.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gotoacloud.top/gtxobjuypg.html

Ruby: arr.uniq
来源：http://hz.tianlin.xyz/gtabdjhwou.html

C#:   list.Distinct().ToList()
来源：http://hz.chenjidiqi.icu/gtqfrcrjmv.html

[D16] 求和与平均值
来源：http://hz.jyoumei.cn/gtjerdgydh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shangyingyoupin.top/gtzqpcpssk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nanxinkj.top/gtmuwlqkta.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtgljyluyv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jyoumei.cn/gthqwcbzuw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xuetiantiany.cn/gtpdiipcek.html

Go:   // 手写循环累加
来源：http://hz.smart0.xyz/gtizwazugx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.guowangkeji.top/gtazkljfzj.html

C#:   list.Sum();  list.Average()
来源：http://hz.jianghu66.top/gtetizyiek.html

[D17] 最大值与最小值
来源：http://hz.xinyue.icu/gtkdewlyvn.html

Py:   max(arr);  min(arr)
来源：http://hz.zhongyouzk.top/gtkjfavxex.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenjidiqi.icu/gthggfzblo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sysykeji.top/gtrdmrzdeb.html

TS:   Math.max(...arr);
来源：http://hz.xuetiantiany.cn/gtbpviiwqp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sweek.top/gtxtqozduh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xylfe.cn/gtnbeivskm.html

Ruby: arr.max;  arr.min
来源：http://hz.nanxinkj.top/gtdjwzrmny.html

C#:   list.Max();  list.Min()
来源：http://hz.sweek.top/gtyjshgfgx.html

[D18] 扁平化嵌套数组
来源：http://hz.meibo888.top/gtlsjogxno.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cheryme.top/gtpqxdzmje.html

PHP:  array_merge(...$nested);
来源：http://hz.tianlin.xyz/gtegydiago.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jyoumei.cn/gtehifqtdv.html

TS:   nested.flat();
来源：http://hz.feifeiyinyue.top/gtyouqjubd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.wangdashe.top/gtxzfbbqee.html

Go:   // 手写双层循环
来源：http://hz.ehwqpu.com/gtpzpdenwf.html

Ruby: nested.flatten
来源：http://hz.zhixingplan.top/gtlgrubqev.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gogol.net.cn/gthpoqhhdy.html

[D19] 按字段分组
来源：http://hz.jyoumei.cn/gtwcatylup.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.guannengcc.top/gtyvsggxmn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.0kj1m.cn/gtkpdwjapa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinqigfzy.top/gtmglsjnww.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ivvv.top/gtahndzlvu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenzaomai.com/gthrjwqulm.html

Go:   // 手写 map[string][]T
来源：http://hz.316326.xyz/gtvspdcpzt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shangyingyoupin.top/gtowgymclv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jqgufenzy.top/gttghejzpb.html

[D20] 统计每个元素出现次数
来源：http://hz.yongpay.top/gtateqbids.html

Py:   Counter(arr)
来源：http://hz.zhengqikj.top/gtmhgzsfay.html

PHP:  array_count_values($arr);
来源：http://hz.yj20258.top/gtscfyzkkd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gzhubu.top/gtkfcsatya.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ydzc1.top/gtavofifvn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinqigufen.top/gturkvpqwr.html

Go:   // 手写 map[T]int
来源：http://hz.fzhhl.top/gtkkzjruij.html

Ruby: arr.tally
来源：http://hz.cheryme.top/gtdinxghiw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cheryme.top/gtwjtudthe.html

[D21] 判断是否包含某元素
来源：http://hz.52xcode.cn/gtfynyzush.html

Py:   x in arr
来源：http://hz.sxryk.cn/gtbtzstdit.html

PHP:  in_array($x, $arr, true);
来源：http://hz.redwolf501.top/gtocacvgjf.html

JS:   arr.includes(x)
来源：http://hz.yonumen.top/gtngpenssp.html

TS:   arr.includes(x)
来源：http://hz.jqgufenzy.top/gtotwroyfd.html

Java: list.contains(x)
来源：http://hz.zdqjudy.top/gthszptgni.html

Go:   slices.Contains(arr, x)
来源：http://hz.dianchejie.cn/gthfauqjtf.html

Ruby: arr.include?(x)
来源：http://hz.yj20258888.top/gttztydeds.html

C#:   list.Contains(x)
来源：http://hz.zhongyouzk.top/gtxtdrzosx.html

[D22] 复制数组（避免共享引用）
来源：http://hz.smart0.xyz/gtslhurhdd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xinyue.icu/gtvujhgnnr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tianlin.xyz/gtkkwaikly.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jqgufenzy.top/gteeedgnqo.html

TS:   [...arr];
来源：http://hz.yj20258.top/gtgkodlojq.html

Java: new ArrayList<>(list);
来源：http://hz.jqgfzy.top/gtfejiottp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sxryk.cn/gtzuktyxos.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xuanzx.com/gtgaqnxrly.html

C#:   new List<int>(list);
来源：http://hz.kuanghao11.cn/gtqibswkxt.html

[D23] reduce 累积计算
来源：http://hz.guowangkeji.top/gtczwpsidt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gogol.net.cn/gtvxkoryxq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.snrcjt.cn/gtxjcmzbhv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nwbrower.top/gtwzmgwyvz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenlongwang.top/gtltqtdjfh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nanxinkj.top/gtifkorkud.html

Go:   // 手写循环
来源：http://hz.shzxlz.cn/gtkcgdexer.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yj20258888.top/gtfatnbxqx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.mhx1999.top/gtdztmpwsg.html

[D24] 字典 / Map 基本操作
来源：http://hz.xziqi.cn/gtxsdcaagt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.feifeiyinyue.top/gtcautsnoe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yonumen.top/gtdhyogudw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jlsjyb.cn/gthdrifdlt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hongshengwenyu.top/gtltgeybyc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.bjfxy.top/gtvarhxkfk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.haohaochexian.top/gtccakjheh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yuanzhike.top/gtutdjibrh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gotoacloud.top/gturioeibv.html

[D25] Set 集合去重与交并差
来源：http://hz.fzhhl.top/gtywldiavw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yangfankeji.com/gtjerafsoa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.sweek.top/gtzjukiezz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.gzhubu.top/gtppuxqnit.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.dashuyun.cn/gtyavekpwc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.kuanghao11.cn/gteiebptvh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.meibo888.top/gtllbgvdjw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.9152youxi.cn/gtittqldlp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ywan-chungtsiang.top/gtuogwlchl.html

[D26] 数组转字符串
来源：http://hz.jianghu66.top/gtqxpaehfh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shanyushiyangkeji.top/gttstcsjbf.html

PHP:  implode(", ", $arr);
来源：http://hz.svipenyu.cn/gtlfmvurxk.html

JS:   arr.join(", ")
来源：http://hz.yuxming.cn/gtcsadtwqy.html

TS:   arr.join(", ")
来源：http://hz.wangdashe.top/gthhvzsuke.html

Java: String.join(", ", list)
来源：http://hz.guowangkeji.top/gtdtjkakdm.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cdnleiting.top/gtiamblmrv.html

Ruby: arr.join(", ")
来源：http://hz.cdnleiting.top/gthezbeioi.html

C#:   string.Join(", ", list)
来源：http://hz.guannengcc.top/gtwkcohsqq.html

================================================================================
来源：http://hz.ppjwa.cn/gtojjnjzgy.html

E. 字符串处理
来源：http://hz.tianlin.xyz/gtzojdrslw.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gthedpcgdk.html

[E01] 拼接字符串
来源：http://hz.ehwqpu.com/gtpkauyvvy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.daxiang520.top/gtjwmudyto.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hywenlv.cn/gtmdnnspdh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhixingplan.top/gtwgwgjmtl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cashguo.top/gtzdpwjjrs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xziqi.cn/gtxbifdkqr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.svipenyu.cn/gtzbstfdtm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hywenlv.cn/gtnohcsszx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cheryme.top/gtlubohjjo.html

[E02] 重复字符串
来源：http://hz.pycfn.com/gtfxzlbjlk.html

Py:   "ab" * 3
来源：http://hz.shzxlz.cn/gtwpfnqigt.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cqqwz.cn/gtypyhbvyx.html

JS:   "ab".repeat(3)
来源：http://hz.xylfe.cn/gteyohzdtb.html

TS:   "ab".repeat(3)
来源：http://hz.zhiwuduotai.top/gtmoutkaff.html

Java: "ab".repeat(3)
来源：http://hz.cqqwz.cn/gtpqlebmkw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.chenzaomai.com/gtwejcsvcu.html

Ruby: "ab" * 3
来源：http://hz.ivvv.top/gtlemjqtzj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yj20258888.top/gtubbtdqia.html

[E03] 截取子串
来源：http://hz.hywenlv.cn/gtyvmfcbxp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.vqdsnc.cn/gtwrkzjjcu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yangfankeji.com/gtbbughndy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.tianlin.xyz/gtrcdlthqk.html

TS:   s.slice(1, 4)
来源：http://hz.ywan-chungtsiang.top/gtlgtuzwxv.html

Java: s.substring(1, 4)
来源：http://hz.zdqjudy.top/gtylxvevlb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.iojbl.cn/gtkdixtukr.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hnxiangtu.top/gtonjlneda.html

C#:   s.Substring(1, 3)
来源：http://hz.sysykeji.top/gtxuscmpoo.html

[E04] 查找子串位置
来源：http://hz.iojbl.cn/gtpfnsktnc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sweek.top/gtikzjprlg.html

PHP:  strpos($s, "x");
来源：http://hz.gotoacloud.top/gtbygplbnb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.havefunace.top/gtdxqaymwb.html

TS:   s.indexOf("x")
来源：http://hz.guannengcc.top/gtkoovxraw.html

Java: s.indexOf("x")
来源：http://hz.hnxiangtu.top/gtrubxoxjl.html

Go:   strings.Index(s, "x")
来源：http://hz.yonumen.top/gtyoandpel.html

Ruby: s.index("x")
来源：http://hz.c1oappe.top/gtjfocvgfl.html

C#:   s.IndexOf("x")
来源：http://hz.fengsongda.top/gtugnlcjyz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinghuilouyu.cn/gtkpwskdbd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shuidangran.top/gtjksgebkx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.andypj.xyz/gtbiuwcjvn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.andypj.xyz/gtjgkbarkz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.pengpengdd.cyou/gtfswolals.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.316326.xyz/gthdrypcqo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.guannengcc.top/gttkjsawmi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhaomingkeji.xyz/gthhsdkmfg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.tian-w.cn/gtzrbkdfpa.html


<!-- 参考信息 -->