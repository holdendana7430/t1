代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guannengcc.top/gtmnbrrdnq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jiagoushi.top/gtiediynil.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.fzhhl.top/gtijhbcfoi.html

Ruby: # 无泛型
来源：http://hz.chenjidiqi.icu/gtirjmpdfg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yongpay.top/gtuygipguy.html

[C15] 解构 / 展开参数
来源：http://hz.xingfuxueyuan.xyz/gtgwotyfyq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hywenlv.cn/gtzyhgubtn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhoulong.xyz/gtzytrguih.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xinyue.icu/gtfvaxlhyb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ppjwa.cn/gtbzzouqrp.html

Java: // 无解构
来源：http://hz.zhixingplan.top/gtbdwqhcey.html

Go:   // 无解构
来源：http://hz.gaohongyu789.top/gtrqqaklsp.html

Ruby: a, b = pair
来源：http://hz.gogol.net.cn/gtlpqlsexr.html

C#:   var (a, b) = pair;
来源：http://hz.ppjwa.cn/gtzkbyarzb.html

[C16] 函数 / 方法重载
来源：http://hz.meibo888.top/gtibqcfdtv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hfpthk.cn/gtquqgwgic.html

PHP:  // 无重载
来源：http://hz.chenzaomai.com/gtdheulkxr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenlongwang.top/gtezeynuom.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hysaishi.cn/gtrkwtsjqs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.snrcjt.cn/gthttketcj.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinqigufen.top/gtivtnwbay.html

Ruby: # 无重载：靠动态参数
来源：http://hz.bjfxy.top/gtnprrfhch.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhengqikj.top/gtioxnqkdx.html

================================================================================
来源：http://hz.yuxming.cn/gtqugwvtto.html

D. 数组 / 列表 / 集合
来源：http://hz.fzhhl.top/gtmvvrheup.html

================================================================================
来源：http://hz.shzxlz.cn/gtfadazlxv.html

[D01] 创建数组 / 列表
来源：http://hz.hysaishi.cn/gtcvlgxxra.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jqgufenzy.top/gtoaayifgs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ehwqpu.com/gtjxxjvhgh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhixingplan.top/gttvdgbcpj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yongpay.top/gtngbcbwic.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yj20258888.top/gtybtwhded.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shzxlz.cn/gtnmhuhjvw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yangfankeji.com/gtbgkwtfoo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xingfuxueyuan.xyz/gtedcufjcd.html

[D02] 追加元素到末尾
来源：http://hz.316326.xyz/gtlexzgzgf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.andypj.xyz/gtklzzzhin.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hysaishi.cn/gtnakvryxd.html

JS:   arr.push(4);
来源：http://hz.chenlongwang.top/gtdsgnoojr.html

TS:   arr.push(4);
来源：http://hz.cheryme.top/gtstoortff.html

Java: list.add(4);
来源：http://hz.hnxiangtu.top/gtjswsdrhv.html

Go:   arr = append(arr, 4)
来源：http://hz.zhixingplan.top/gtlltmdgvt.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.0kj1m.cn/gthtpqvpbk.html

C#:   list.Add(4);
来源：http://hz.cdnleiting.top/gtbpkiwhbp.html

[D03] 在指定位置插入元素
来源：http://hz.yvedp.cn/gtskywvrka.html

Py:   arr.insert(0, 0)
来源：http://hz.snrcjt.cn/gttfiiyyxi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.fengsongda.top/gteugewixt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.smart0.xyz/gtygqhjlyh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gzhubu.top/gtcqwfvxww.html

Java: list.add(0, 0);
来源：http://hz.aibaodan.cn/gtmralqqmh.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hammf.cn/gtbyyxirgg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.chenlongwang.top/gthavocsjn.html

C#:   list.Insert(0, 0);
来源：http://hz.gotoacloud.top/gtydezrdlc.html

[D04] 删除元素
来源：http://hz.yonumen.top/gtuqtltujs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.aibaodan.cn/gtiasmogkd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.iojbl.cn/gtnavtdflp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.dashuyun.cn/gtqalonetv.html

TS:   arr.splice(0, 1);
来源：http://hz.pycfn.com/gttlenjpsp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.nanxinkj.top/gtokorihyr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jiagoushi.top/gtmnqctjth.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.0kj1m.cn/gtpfncyvzd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.quarkkingdee.top/gtoheukptc.html

[D05] 访问与修改元素
来源：http://hz.aizwys.cn/gtdkztfrpp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tanke756.top/gtyccdjemf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gzhubu.top/gtvrholyqd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yanxiufei.cn/gtedeuoehq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.kuanghao11.cn/gtftwenebs.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.havefunace.top/gtdyixzjzv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xuetiantiany.cn/gtnelmgxtf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.dashuyun.cn/gtqmnhinkv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangdashe.top/gtraucvput.html

[D06] 数组长度
来源：http://hz.shzxlz.cn/gtqwvzbbnp.html

Py:   len(arr)
来源：http://hz.yueranfly.top/gtfrddkhnw.html

PHP:  count($arr);
来源：http://hz.aizwys.cn/gtxgyuspcs.html

JS:   arr.length
来源：http://hz.ybcxt.top/gtkgwrtsne.html

TS:   arr.length
来源：http://hz.gaohongyu789.top/gtrbvrsdpp.html

Java: list.size();
来源：http://hz.zdqjudy.top/gtybawxkzx.html

Go:   len(arr)
来源：http://hz.yanxiufei.cn/gthrspeejg.html

Ruby: arr.length; arr.size
来源：http://hz.havefunace.top/gtbjktvvqp.html

C#:   list.Count;
来源：http://hz.iojbl.cn/gtenmngdcl.html

[D07] 切片 / 取子数组
来源：http://hz.birdmap.top/gttkpurzdl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhixingplan.top/gtgmovrlzn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhijiandao.cn/gtlirczscj.html

JS:   arr.slice(1, 4);
来源：http://hz.jinqigfzy.top/gtnjpzxaqh.html

TS:   arr.slice(1, 4);
来源：http://hz.zdqjudy.top/gtbpdrgpip.html

Java: list.subList(1, 4);
来源：http://hz.aibaodan.cn/gtsazzlekf.html

Go:   arr[1:4]
来源：http://hz.cdnleiting.top/gtaoqrcqto.html

Ruby: arr[1, 3]
来源：http://hz.pengpengdd.cyou/gtpcqgkuaa.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258.top/gtexfkwbql.html

[D08] 合并两个数组
来源：http://hz.jyoumei.cn/gtukbyiyuq.html

Py:   a + b;  a.extend(b)
来源：http://hz.nwbrower.top/gtdxkztyez.html

PHP:  array_merge($a, $b);
来源：http://hz.guowangkeji.top/gtvqmxxcel.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhengqikj.top/gtpzlrsrim.html

TS:   [...a, ...b];
来源：http://hz.nanxinkj.top/gtcpcmevdb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sweek.top/gtdulujofw.html

Go:   append(a, b...)
来源：http://hz.yuanzhike.top/gteuqgakyv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zycfv.cn/gtcfpykpei.html

C#:   a.Concat(b).ToList()
来源：http://hz.vqdsnc.cn/gtknhghrhw.html

[D09] 排序（升序）
来源：http://hz.0kj1m.cn/gtmbuailjx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtkgercgkq.html

PHP:  sort($arr);
来源：http://hz.c1oappe.top/gtwzzblwqk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shuidangran.top/gthpdtiaal.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hammf.cn/gtnrozmzef.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sufxvd.cn/gtttommmqz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.birdmap.top/gtszkysujy.html

Ruby: arr.sort
来源：http://hz.kuanghao11.cn/gtfilmoase.html

C#:   list.Sort();
来源：http://hz.yj20258.top/gtbwlqjmrp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cheryme.top/gtwaruofir.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jinqigfzy.top/gtxpyckqiv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.dianchejie.cn/gtfgsechnc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gaohongyu789.top/gtymdkyujr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhongyouzk.top/gtencmqopn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinqigufen.top/gtokjhfndp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.52xcode.cn/gtczfofubb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj202588.top/gtsjxwhauu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.9152youxi.cn/gtbprbpobu.html

[D11] 反转数组
来源：http://hz.yvedp.cn/gtewdopmlq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jinqigufen.top/gtebgbnlca.html

PHP:  array_reverse($arr);
来源：http://hz.xinyue.icu/gtiffrfurj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jlsjyb.cn/gtlcinxksd.html

TS:   [...arr].reverse();
来源：http://hz.wangdashe.top/gtujzgfcqk.html

Java: Collections.reverse(list);
来源：http://hz.sxryk.cn/gtkxyjtkuq.html

Go:   slices.Reverse(arr)
来源：http://hz.pycfn.com/gtovxgjqdr.html

Ruby: arr.reverse
来源：http://hz.redwolf501.top/gtigpnctjk.html

C#:   list.Reverse();
来源：http://hz.pycfn.com/gtihrnxpas.html

[D12] 查找元素下标
来源：http://hz.fengsongda.top/gttmcvksoq.html

Py:   arr.index(x);  x in arr
来源：http://hz.zdqjudy.top/gtgwiqxwxz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jqgufenzy.top/gtfrjqjrry.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pengpengdd.cyou/gtqrmbeolp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.redwolf501.top/gtlmlxukqu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.316326.xyz/gtdlildxut.html

Go:   slices.Index(arr, x)
来源：http://hz.yuanzhike.top/gtxobdkhid.html

Ruby: arr.index(x)
来源：http://hz.gzhubu.top/gttkioxtdv.html

C#:   list.IndexOf(x);
来源：http://hz.gaohongyu789.top/gtjqfjwlnj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.0kj1m.cn/gttgrcqhiv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jlsjyb.cn/gtfuivyzhx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shzxlz.cn/gtcagqltnw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hfpthk.cn/gtaycghvih.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gotoacloud.top/gtkgcfdzgg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gaohongyu789.top/gtwvxmzhfp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.svipenyu.cn/gtdfblcdns.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.bjfxy.top/gtmgknzhwj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.nwbrower.top/gtckzghlmz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhixingplan.top/gtbwroaqxy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinyuanbaomall.cn/gtmeolgkaj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xuetiantiany.cn/gtzkzqgopf.html

JS:   arr.map(x => x * 2)
来源：http://hz.yanxiufei.cn/gtsswyghla.html

TS:   arr.map(x => x * 2)
来源：http://hz.sufxvd.cn/gttdgvplic.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhoulong.xyz/gtonjuorfn.html

Go:   // 手写循环
来源：http://hz.ybcxt.top/gtvvkegjpb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ydzc1.top/gtzresbjvb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhijiandao.cn/gtkcgekeae.html

[D15] 去重
来源：http://hz.hammf.cn/gtdkxbbylt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenzaomai.com/gtnavxzsud.html

PHP:  array_unique($arr);
来源：http://hz.xinyue.icu/gtzkjthfbn.html

JS:   [...new Set(arr)]
来源：http://hz.svipenyu.cn/gtzbzimfhd.html

TS:   [...new Set(arr)]
来源：http://hz.zhixingplan.top/gtvqmicype.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.svipenyu.cn/gtzttxhbhu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pengpengdd.cyou/gtmrwsxmlc.html

Ruby: arr.uniq
来源：http://hz.xylfe.cn/gtohudxcwa.html

C#:   list.Distinct().ToList()
来源：http://hz.xuetiantiany.cn/gtayrbuyqg.html

[D16] 求和与平均值
来源：http://hz.yongpay.top/gtipgaoxyq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.nwbrower.top/gtyzpiamyo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinghuilouyu.cn/gttfgivydf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gaohongyu789.top/gtxjukxvcl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtwvnhskqz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.andypj.xyz/gtvnqjlnpm.html

Go:   // 手写循环累加
来源：http://hz.pycfn.com/gtzthxbxcc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhaomingkeji.xyz/gtcgjkkcis.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenzaomai.com/gtbzjxdrbc.html

[D17] 最大值与最小值
来源：http://hz.shzxlz.cn/gtspphcxqo.html

Py:   max(arr);  min(arr)
来源：http://hz.shangyingyoupin.top/gtiunyxhbo.html

PHP:  max($arr);  min($arr);
来源：http://hz.fengsongda.top/gtmgowgnnn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hnqzz.top/gtwrjjiavw.html

TS:   Math.max(...arr);
来源：http://hz.ppjwa.cn/gtyjarymgf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.wangdashe.top/gtakqzcmmu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhijiandao.cn/gtudbrlgdu.html

Ruby: arr.max;  arr.min
来源：http://hz.cheryme.top/gtglkpafgh.html

C#:   list.Max();  list.Min()
来源：http://hz.yongpay.top/gtafwmllop.html

[D18] 扁平化嵌套数组
来源：http://hz.yj20258.top/gtbfyuwpcj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.dashuyun.cn/gtolwgfaio.html

PHP:  array_merge(...$nested);
来源：http://hz.jqgfzy.top/gtujkcsgcq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xziqi.cn/gtsncnqtzb.html

TS:   nested.flat();
来源：http://hz.yvedp.cn/gtwwaulcon.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gzhubu.top/gtakxndrou.html

Go:   // 手写双层循环
来源：http://hz.hfpthk.cn/gtgatbacdr.html

Ruby: nested.flatten
来源：http://hz.xinyue.icu/gtjpydwnkx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ydjk.org.cn/gtznrirsfp.html

[D19] 按字段分组
来源：http://hz.gogol.net.cn/gtpwrbrlzq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.52xcode.cn/gtlqmauhml.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shuidangran.top/gtygbraxxh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daria6918.cn/gtilkqbssh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yuxming.cn/gtruyfloyw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yanxiufei.cn/gtpnzkuytt.html

Go:   // 手写 map[string][]T
来源：http://hz.0kj1m.cn/gtrjyuimri.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.tian-w.cn/gtpnhrdnvn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yueranfly.top/gtbektnkvo.html

[D20] 统计每个元素出现次数
来源：http://hz.9152youxi.cn/gtbxlpgggn.html

Py:   Counter(arr)
来源：http://hz.vqdsnc.cn/gtcfcuzxin.html

PHP:  array_count_values($arr);
来源：http://hz.snrcjt.cn/gtswgzzjvv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ybcxt.top/gtmcrglqim.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shzxlz.cn/gthatdpsdk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinqigufen.top/gtdhxcryzh.html

Go:   // 手写 map[T]int
来源：http://hz.0kj1m.cn/gthaznecec.html

Ruby: arr.tally
来源：http://hz.meibo888.top/gtbszljfxp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hnqzz.top/gtnjatysms.html

[D21] 判断是否包含某元素
来源：http://hz.cucudq.cn/gtfeqatwnw.html

Py:   x in arr
来源：http://hz.xziqi.cn/gtramyjrze.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yj202588.top/gtekldzpqg.html

JS:   arr.includes(x)
来源：http://hz.guowangkeji.top/gtxzkytcej.html

TS:   arr.includes(x)
来源：http://hz.svipenyu.cn/gtbkfcpwxh.html

Java: list.contains(x)
来源：http://hz.yj20258.top/gtqnjscpwh.html

Go:   slices.Contains(arr, x)
来源：http://hz.pycfn.com/gtpupyeoex.html

Ruby: arr.include?(x)
来源：http://hz.hywenlv.cn/gtkiuywpqf.html

C#:   list.Contains(x)
来源：http://hz.snrcjt.cn/gtgkewefnn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jyoumei.cn/gtrtwkrfxu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yj20258.top/gtnyafbhnl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.birdmap.top/gtuvvwyxgd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yvedp.cn/gtxhjujxtd.html

TS:   [...arr];
来源：http://hz.smart0.xyz/gtervycnab.html

Java: new ArrayList<>(list);
来源：http://hz.jinyuanbaomall.cn/gtthernlnr.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.haohaochexian.top/gtbjiokayk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.c1oappe.top/gthnopkaxo.html

C#:   new List<int>(list);
来源：http://hz.yj202588.top/gtucfsiezg.html

[D23] reduce 累积计算
来源：http://hz.havefunace.top/gtdiqgbsbp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ivvv.top/gtgyrihqnm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhongyouzk.top/gtoihjtgxt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yongpay.top/gtqrtxtuuh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gtwjmrldth.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tianlin.xyz/gtjgzxdwtr.html

Go:   // 手写循环
来源：http://hz.birdmap.top/gtpukstbxt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cashguo.top/gttfwztqxu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ydjk.org.cn/gtruabhjxe.html

[D24] 字典 / Map 基本操作
来源：http://hz.gogol.net.cn/gtuvnnywyj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.cqqwz.cn/gtbmfabpno.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yanxiufei.cn/gtnxwbdqcv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.wangdashe.top/gtdgccijfp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.havefunace.top/gtiitdooze.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxinkj.top/gtxhpmsipw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ehwqpu.com/gtntvabxxf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jqgufenzy.top/gtxwxipfgn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.mhx1999.top/gtcbgmlcpg.html

[D25] Set 集合去重与交并差
来源：http://hz.wangshuangyany.cn/gtuyetezqe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jqgfzy.top/gtrxetuyzs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yj20258888.top/gtknhzcxmk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.52xcode.cn/gtynohnaap.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.316326.xyz/gtlvpabnfx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.aibaodan.cn/gtjbmqgmoi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jqgfzy.top/gtrvchqfof.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.dianchejie.cn/gtqdakjenh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinghuilouyu.cn/gtnfhstoxz.html

[D26] 数组转字符串
来源：http://hz.chenjidiqi.icu/gtjngcfdpd.html

Py:   ", ".join(map(str, arr))
来源：http://hz.dianchejie.cn/gtnhhhzfsf.html

PHP:  implode(", ", $arr);
来源：http://hz.yj20258888.top/gtitozhcfq.html

JS:   arr.join(", ")
来源：http://hz.hysaishi.cn/gtbwyfvpae.html

TS:   arr.join(", ")
来源：http://hz.birdmap.top/gtjhcesjmf.html

Java: String.join(", ", list)
来源：http://hz.zhoulong.xyz/gtbebeyljf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.snrcjt.cn/gtefpcjzsb.html

Ruby: arr.join(", ")
来源：http://hz.zhoulong.xyz/gtfmgcedzp.html

C#:   string.Join(", ", list)
来源：http://hz.zhijiandao.cn/gtnshrcfel.html

================================================================================
来源：http://hz.yanxiufei.cn/gtaouvfvuu.html

E. 字符串处理
来源：http://hz.sxryk.cn/gtmadrpkjk.html

================================================================================
来源：http://hz.pycfn.com/gtzrwgzhjp.html

[E01] 拼接字符串
来源：http://hz.wangshuangyany.cn/gtqsfzhlha.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinqigufen.top/gttuerioxc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhiwuduotai.top/gtwhdtmgxu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigfzy.top/gtqxxjlqcz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cdnleiting.top/gtqlsgkehs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yj20258.top/gteydyndsu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.tian-w.cn/gtumcqemte.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.smart0.xyz/gtnwlfsrik.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.fzhhl.top/gtwmprblbu.html

[E02] 重复字符串
来源：http://hz.zhaomingkeji.xyz/gtivquggjy.html

Py:   "ab" * 3
来源：http://hz.yuxming.cn/gtjwakatmx.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zdqjudy.top/gtuoidnjth.html

JS:   "ab".repeat(3)
来源：http://hz.tanke756.top/gtihsjfqya.html

TS:   "ab".repeat(3)
来源：http://hz.cheryme.top/gtdtxndqej.html

Java: "ab".repeat(3)
来源：http://hz.zhaomingkeji.xyz/gtonrxhyuh.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.meibo888.top/gtzdghqgyy.html

Ruby: "ab" * 3
来源：http://hz.dashuyun.cn/gtywckbvfr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dianchejie.cn/gtkkdgesbt.html

[E03] 截取子串
来源：http://hz.shuidangran.top/gtgdpmojud.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinqigufen.top/gtyswjtktq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.tianlin.xyz/gtvurxgyoc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ydjk.org.cn/gtgkpvsqpx.html

TS:   s.slice(1, 4)
来源：http://hz.meibo888.top/gtbltwdlqd.html

Java: s.substring(1, 4)
来源：http://hz.andypj.xyz/gtdmzcyjdp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tian-w.cn/gtygkarkov.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.redwolf501.top/gtydgnpeva.html

C#:   s.Substring(1, 3)
来源：http://hz.haohaochexian.top/gtxoxzzryr.html

[E04] 查找子串位置
来源：http://hz.hnxiangtu.top/gtzgoaazyn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinqigfzy.top/gtznmletpn.html

PHP:  strpos($s, "x");
来源：http://hz.hnxiangtu.top/gtxrvveegt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yuxming.cn/gtqsyxpwoh.html

TS:   s.indexOf("x")
来源：http://hz.zhoulong.xyz/gtpxdwjizp.html

Java: s.indexOf("x")
来源：http://hz.tian-w.cn/gtoselktiy.html

Go:   strings.Index(s, "x")
来源：http://hz.ppjwa.cn/gtnkbsqlew.html

Ruby: s.index("x")
来源：http://hz.guannengcc.top/gtjpbotqdb.html

C#:   s.IndexOf("x")
来源：http://hz.daxiang520.top/gtzfcugdud.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.fzhhl.top/gtregimnok.html


<!-- 参考信息 -->