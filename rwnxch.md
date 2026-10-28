代发 wailian999

PHP:  // 无重载
来源：http://hz.ehwqpu.com/gtwhjckfwl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shanyushiyangtech.top/gtkiziwjnb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hnxiangtu.top/gtdfthcbch.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nanxinkj.top/gtnnnsrezz.html

Go:   // 无重载：用不同函数名
来源：http://hz.ywan-chungtsiang.top/gtbshhcrmo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.wangshuangyany.cn/gtsdzpydli.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zycfv.cn/gtcxgmkkxq.html

================================================================================
来源：http://hz.hnqzz.top/gtrmczjoxe.html

D. 数组 / 列表 / 集合
来源：http://hz.jiagoushi.top/gtrlrfckza.html

================================================================================
来源：http://hz.pycfn.com/gtnjpaffxv.html

[D01] 创建数组 / 列表
来源：http://hz.hnxiangtu.top/gtqwrfsqgj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cdnleiting.top/gtfxesfdtt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.316326.xyz/gtnbrstyov.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hammf.cn/gtadsbjtmu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shuidangran.top/gtmnbagykx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nanxuanxn.top/gtcyxjdfjq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.nanxinkj.top/gtcizdafzv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.0kj1m.cn/gtmsongxcq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.nwbrower.top/gtrqzcwwaj.html

[D02] 追加元素到末尾
来源：http://hz.zhengqikj.top/gtiwbltxbn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenjidiqi.icu/gtuuhwhdas.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jianghu66.top/gtniubstce.html

JS:   arr.push(4);
来源：http://hz.chenjidiqi.icu/gtphkqpvbq.html

TS:   arr.push(4);
来源：http://hz.guowangkeji.top/gtunhgsitr.html

Java: list.add(4);
来源：http://hz.yuanzhike.top/gtgjlrzrct.html

Go:   arr = append(arr, 4)
来源：http://hz.feifeiyinyue.top/gtsepnovbs.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.nwbrower.top/gtyfoszwcv.html

C#:   list.Add(4);
来源：http://hz.jqgfzy.top/gtaqtwxcsz.html

[D03] 在指定位置插入元素
来源：http://hz.tian-w.cn/gtoovmqpkh.html

Py:   arr.insert(0, 0)
来源：http://hz.cucudq.cn/gtykjmknrv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xylfe.cn/gtqbsyfesq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ppjwa.cn/gtqcifgotl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yongpay.top/gtwsimroqw.html

Java: list.add(0, 0);
来源：http://hz.hnqzz.top/gtmkllfnko.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.birdmap.top/gttymjvwrf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cdnleiting.top/gthbztshqu.html

C#:   list.Insert(0, 0);
来源：http://hz.0kj1m.cn/gtptizoimx.html

[D04] 删除元素
来源：http://hz.jinghuilouyu.cn/gtdqguzqfn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ydjk.org.cn/gtkhtytaph.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hysaishi.cn/gtfuzerbbm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cashguo.top/gtqioqxcrd.html

TS:   arr.splice(0, 1);
来源：http://hz.wangshuangyany.cn/gtormbqwcw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.feifeiyinyue.top/gtbxldvmze.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shuidangran.top/gtihvefzhc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sysykeji.top/gtbqkgyysi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yuanzhike.top/gtdwzhwwld.html

[D05] 访问与修改元素
来源：http://hz.cucudq.cn/gtsexyobhz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtmqzfdvlb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daxiang520.top/gtlsmvmbak.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yuanzhike.top/gtajqfcraf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ywan-chungtsiang.top/gturpuvnvn.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.quarkkingdee.top/gtnqpogyha.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtoiyzekbe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtkgifsryh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.tianlin.xyz/gtbdjrgwjt.html

[D06] 数组长度
来源：http://hz.zhoulong.xyz/gtoljfvvda.html

Py:   len(arr)
来源：http://hz.snrcjt.cn/gtizjsdrss.html

PHP:  count($arr);
来源：http://hz.yongpay.top/gtpgjmayzy.html

JS:   arr.length
来源：http://hz.vqdsnc.cn/gtezpwhmwj.html

TS:   arr.length
来源：http://hz.pycfn.com/gtohqkapqv.html

Java: list.size();
来源：http://hz.xuanzx.com/gtkzujehbp.html

Go:   len(arr)
来源：http://hz.ywan-chungtsiang.top/gtjlkwwyfr.html

Ruby: arr.length; arr.size
来源：http://hz.gzhubu.top/gtajjmhypn.html

C#:   list.Count;
来源：http://hz.pycfn.com/gtyamwvxme.html

[D07] 切片 / 取子数组
来源：http://hz.hywenlv.cn/gtoluynqsz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhaomingkeji.xyz/gtlkzqcjpp.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.daria6918.cn/gtnamtjyxa.html

JS:   arr.slice(1, 4);
来源：http://hz.hnqzz.top/gtsqeudavs.html

TS:   arr.slice(1, 4);
来源：http://hz.andypj.xyz/gtlkualnkk.html

Java: list.subList(1, 4);
来源：http://hz.zhixingplan.top/gtdwjyiakz.html

Go:   arr[1:4]
来源：http://hz.9152youxi.cn/gttvvlwbdd.html

Ruby: arr[1, 3]
来源：http://hz.zhengqikj.top/gtdymeiggd.html

C#:   list.GetRange(1, 3);
来源：http://hz.shuidangran.top/gtdrkpnqjx.html

[D08] 合并两个数组
来源：http://hz.daria6918.cn/gtszudkshf.html

Py:   a + b;  a.extend(b)
来源：http://hz.yuxming.cn/gtbwogbkck.html

PHP:  array_merge($a, $b);
来源：http://hz.iojbl.cn/gtlxvtekwb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.wangshuangyany.cn/gttbtbsnkt.html

TS:   [...a, ...b];
来源：http://hz.tianlin.xyz/gtcwplxymo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.meibo888.top/gtdumcaswa.html

Go:   append(a, b...)
来源：http://hz.feifeiyinyue.top/gtyrmynksb.html

Ruby: a + b;  a.concat(b)
来源：http://hz.daxiang520.top/gtcpmqhydf.html

C#:   a.Concat(b).ToList()
来源：http://hz.ybcxt.top/gtufylqkng.html

[D09] 排序（升序）
来源：http://hz.bjfxy.top/gtgzvaxglj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hywenlv.cn/gtestjmywf.html

PHP:  sort($arr);
来源：http://hz.gaohongyu789.top/gtlhtrsjkq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.daxiang520.top/gtscnhxgvk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.smart0.xyz/gtzrufbddm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.nanxuanxn.top/gtwqnvgfiz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.daria6918.cn/gtayvhrpzt.html

Ruby: arr.sort
来源：http://hz.jinqigufen.top/gtlbrexvfg.html

C#:   list.Sort();
来源：http://hz.sufxvd.cn/gtaprxxmyi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.redwolf501.top/gtunxvbzpg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hfpthk.cn/gtljsoewaw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuanzhike.top/gtlzjlbhbj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zycfv.cn/gtxcnhxtmw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ydzc1.top/gthzqqjajt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinghuilouyu.cn/gtfdqtijph.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinyuanbaomall.cn/gtkxxhryld.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jqgfzy.top/gtopoplekt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenzaomai.com/gtqykoxytf.html

[D11] 反转数组
来源：http://hz.fzhhl.top/gthdfanjzw.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.havefunace.top/gtgtekdyav.html

PHP:  array_reverse($arr);
来源：http://hz.xinyue.icu/gtigannmne.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yongpay.top/gtygtsegyq.html

TS:   [...arr].reverse();
来源：http://hz.zycfv.cn/gtlmpindce.html

Java: Collections.reverse(list);
来源：http://hz.xziqi.cn/gtodutsfab.html

Go:   slices.Reverse(arr)
来源：http://hz.zdqjudy.top/gtvzpmrdjf.html

Ruby: arr.reverse
来源：http://hz.xziqi.cn/gtlzilgtvj.html

C#:   list.Reverse();
来源：http://hz.jinyuanbaomall.cn/gtdjfpcrhq.html

[D12] 查找元素下标
来源：http://hz.pycfn.com/gtembsmusn.html

Py:   arr.index(x);  x in arr
来源：http://hz.gaohongyu789.top/gttwtqrfbv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yueranfly.top/gtjqbcgzdd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.feifeiyinyue.top/gtlzbxmnpa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hysaishi.cn/gtckdefmeo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hongshengwenyu.top/gtrjjiwcwe.html

Go:   slices.Index(arr, x)
来源：http://hz.yueranfly.top/gtetayqxlx.html

Ruby: arr.index(x)
来源：http://hz.cucudq.cn/gtmkfogsuw.html

C#:   list.IndexOf(x);
来源：http://hz.yj202588.top/gtqqstissl.html

[D13] 过滤（保留满足条件的）
来源：http://hz.fzhhl.top/gtqhotdldh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhengqikj.top/gtubugbksj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xuetiantiany.cn/gtdyayjqca.html

JS:   arr.filter(x => x > 3)
来源：http://hz.mhx1999.top/gteenmhgca.html

TS:   arr.filter(x => x > 3)
来源：http://hz.svipenyu.cn/gtuwnxhcxj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.havefunace.top/gtofhnlmrg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.sufxvd.cn/gtmwgstboy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.dashuyun.cn/gtwjnvlpug.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ehwqpu.com/gtzeedypta.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jyoumei.cn/gttzyzqlvt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.9152youxi.cn/gtknfgoafl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.guannengcc.top/gtnjahnmsu.html

JS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gtxhqvnqhh.html

TS:   arr.map(x => x * 2)
来源：http://hz.gzhubu.top/gtbccgiaqf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ywan-chungtsiang.top/gtczncdgju.html

Go:   // 手写循环
来源：http://hz.0kj1m.cn/gttxdbisrl.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hnxiangtu.top/gtqiofjsel.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zycfv.cn/gtfwiboysy.html

[D15] 去重
来源：http://hz.chenzaomai.com/gtlesooefv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.vqdsnc.cn/gtlymzieop.html

PHP:  array_unique($arr);
来源：http://hz.xziqi.cn/gtbqfvnpqg.html

JS:   [...new Set(arr)]
来源：http://hz.cucudq.cn/gtqqzjsrye.html

TS:   [...new Set(arr)]
来源：http://hz.sweek.top/gtfetjtraj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yueranfly.top/gtfghjizjr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.sxryk.cn/gtntcxlzfw.html

Ruby: arr.uniq
来源：http://hz.ywan-chungtsiang.top/gtjidyecya.html

C#:   list.Distinct().ToList()
来源：http://hz.bjfxy.top/gtypqlhqgb.html

[D16] 求和与平均值
来源：http://hz.svipenyu.cn/gtigteepwl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hywenlv.cn/gtafaqwtfv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.aibaodan.cn/gtwjcwdyht.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nanxuanxn.top/gtiwesbhkj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yvedp.cn/gtqigcpxzy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.kuanghao11.cn/gtuqjijsyk.html

Go:   // 手写循环累加
来源：http://hz.tanke756.top/gtgvawrgwa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xuanzx.com/gtzlsybszu.html

C#:   list.Sum();  list.Average()
来源：http://hz.gaohongyu789.top/gtnxcmrxix.html

[D17] 最大值与最小值
来源：http://hz.hnqzz.top/gtcrzqiwhb.html

Py:   max(arr);  min(arr)
来源：http://hz.mhx1999.top/gtczuyxmgo.html

PHP:  max($arr);  min($arr);
来源：http://hz.jqgufenzy.top/gtnrpbipnr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yj20258888.top/gtdgdwramd.html

TS:   Math.max(...arr);
来源：http://hz.jinqigfzy.top/gtqndynxrk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xuetiantiany.cn/gtgqomkzkm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ivvv.top/gtsfjwmbuc.html

Ruby: arr.max;  arr.min
来源：http://hz.andypj.xyz/gtluscldjq.html

C#:   list.Max();  list.Min()
来源：http://hz.mhx1999.top/gteptswaoh.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangkeji.top/gtkcaxowtb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.havefunace.top/gtxvlliedt.html

PHP:  array_merge(...$nested);
来源：http://hz.zhiwuduotai.top/gtsugjcpzo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sweek.top/gtifnhrmtv.html

TS:   nested.flat();
来源：http://hz.sysykeji.top/gtpzrqtawu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gaohongyu789.top/gtpyqexhsf.html

Go:   // 手写双层循环
来源：http://hz.zhengqikj.top/gtobebltyw.html

Ruby: nested.flatten
来源：http://hz.gogol.net.cn/gtimxqaiiy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ybcxt.top/gtethsaeep.html

[D19] 按字段分组
来源：http://hz.havefunace.top/gtgexwrkfp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yangfankeji.com/gtytkcxtax.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.iojbl.cn/gtagsctwqg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hnxiangtu.top/gtroeeoajf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinyuanbaomall.cn/gtpcfjauvt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zycfv.cn/gtpmrzornc.html

Go:   // 手写 map[string][]T
来源：http://hz.havefunace.top/gtvrntmyzv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhengqikj.top/gtlbbdwwvw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.fengsongda.top/gtzyrppkpb.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgufenzy.top/gtvcimxufp.html

Py:   Counter(arr)
来源：http://hz.guannengcc.top/gtsoevwnij.html

PHP:  array_count_values($arr);
来源：http://hz.ywan-chungtsiang.top/gtumglrrge.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhaomingkeji.xyz/gtoabvuvxy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.smart0.xyz/gtcsakibdn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhengqikj.top/gtyuimppen.html

Go:   // 手写 map[T]int
来源：http://hz.jyoumei.cn/gtombrxjwj.html

Ruby: arr.tally
来源：http://hz.ybcxt.top/gtpoucxsjd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ehwqpu.com/gtpvdewlpn.html

[D21] 判断是否包含某元素
来源：http://hz.ydzc1.top/gtqispqczx.html

Py:   x in arr
来源：http://hz.aizwys.cn/gtrthcsqxr.html

PHP:  in_array($x, $arr, true);
来源：http://hz.haohaochexian.top/gthhcnuyjr.html

JS:   arr.includes(x)
来源：http://hz.sweek.top/gtgvmaiexk.html

TS:   arr.includes(x)
来源：http://hz.yanxiufei.cn/gtrtcgiqeu.html

Java: list.contains(x)
来源：http://hz.gogol.net.cn/gtfteqsonk.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenjidiqi.icu/gtwbwofynp.html

Ruby: arr.include?(x)
来源：http://hz.cdnleiting.top/gtbpgcqavd.html

C#:   list.Contains(x)
来源：http://hz.daria6918.cn/gtubcwnanv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zycfv.cn/gtyceqtspu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hywenlv.cn/gtondwqzga.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.haohaochexian.top/gtrmmttpgu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zycfv.cn/gthjqqchtk.html

TS:   [...arr];
来源：http://hz.aizwys.cn/gtelmzfalm.html

Java: new ArrayList<>(list);
来源：http://hz.gotoacloud.top/gtqbpxfbvs.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cheryme.top/gtwfbdmowt.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gzhubu.top/gtubihvkxk.html

C#:   new List<int>(list);
来源：http://hz.316326.xyz/gtgfgvtjev.html

[D23] reduce 累积计算
来源：http://hz.jinqigufen.top/gtfwvvksrk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.vqdsnc.cn/gthotedzti.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.svipenyu.cn/gtdhlroyyr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jqgfzy.top/gtvqhdgpxf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydjk.org.cn/gtgdbrtxqf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.iojbl.cn/gtoiwkjwaz.html

Go:   // 手写循环
来源：http://hz.gzhubu.top/gtnuwqaafy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shuidangran.top/gtdnmjjmbw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ivvv.top/gtmdajwsia.html

[D24] 字典 / Map 基本操作
来源：http://hz.0kj1m.cn/gthrszgsii.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.andypj.xyz/gthzihynzr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.chenlongwang.top/gtuerougtq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ybcxt.top/gtwrxaroag.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yuxming.cn/gtprjhhxoe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.meibo888.top/gtpmbvtotx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jyoumei.cn/gtucywqhhc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhijiandao.cn/gtnnqxkkgw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhixingplan.top/gttbfguplv.html

[D25] Set 集合去重与交并差
来源：http://hz.feifeiyinyue.top/gtlhduwyvs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.316326.xyz/gtbpduujzs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.tianlin.xyz/gtqpcmoatd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ybcxt.top/gtkgvhduat.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.snrcjt.cn/gtdkhuhlvy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ivvv.top/gtyqutfypu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.kuanghao11.cn/gtgjfruxht.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yj20258.top/gtqjfodjxg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.aizwys.cn/gtjzzpegfl.html

[D26] 数组转字符串
来源：http://hz.andypj.xyz/gtilqzbdea.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jqgfzy.top/gtlejzuxkb.html

PHP:  implode(", ", $arr);
来源：http://hz.pycfn.com/gtziucvxuy.html

JS:   arr.join(", ")
来源：http://hz.guannengcc.top/gtycfxbwiw.html

TS:   arr.join(", ")
来源：http://hz.fengsongda.top/gtveklhpnz.html

Java: String.join(", ", list)
来源：http://hz.cqqwz.cn/gtnhkttwcp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.aizwys.cn/gtbclvfrkx.html

Ruby: arr.join(", ")
来源：http://hz.hammf.cn/gtpysppizb.html

C#:   string.Join(", ", list)
来源：http://hz.hongshengwenyu.top/gtyubawuje.html

================================================================================
来源：http://hz.zhengqikj.top/gtocyterai.html

E. 字符串处理
来源：http://hz.zhongyouzk.top/gtigteferq.html

================================================================================
来源：http://hz.zhijiandao.cn/gtoiinrcgx.html

[E01] 拼接字符串
来源：http://hz.guannengcc.top/gttnmvhiic.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dashuyun.cn/gtfrsmcekc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.wangdashe.top/gthtqjyyuy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aizwys.cn/gtbgztieqx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.pengpengdd.cyou/gtnxixvuxr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.daxiang520.top/gtuvkdgpjj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yongpay.top/gtsalnhtig.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shanyushiyangkeji.top/gtvnkgvcjg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cashguo.top/gtlkfsqbuc.html

[E02] 重复字符串
来源：http://hz.tian-w.cn/gtdipuwdig.html

Py:   "ab" * 3
来源：http://hz.jqgfzy.top/gtslsvsqhg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhiwuduotai.top/gtagekzqnb.html

JS:   "ab".repeat(3)
来源：http://hz.gaohongyu789.top/gteqbwwpxt.html

TS:   "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtpxyuvxpq.html

Java: "ab".repeat(3)
来源：http://hz.chenlongwang.top/gtinpxmczv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.bjfxy.top/gtpplebzge.html

Ruby: "ab" * 3
来源：http://hz.feifeiyinyue.top/gtqvczeeoa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.tian-w.cn/gtmhagcoci.html

[E03] 截取子串
来源：http://hz.cdnleiting.top/gtthrqevex.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinghuilouyu.cn/gteqxzjedp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.fengsongda.top/gtnuafqrxs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.guannengcc.top/gtndoapzao.html

TS:   s.slice(1, 4)
来源：http://hz.snrcjt.cn/gtmrogxpsq.html

Java: s.substring(1, 4)
来源：http://hz.shzxlz.cn/gtahymxdjf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tianlin.xyz/gtmxvoapqk.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gogol.net.cn/gtzmkjwhed.html

C#:   s.Substring(1, 3)
来源：http://hz.hongshengwenyu.top/gtsmqcswrs.html

[E04] 查找子串位置
来源：http://hz.yuxming.cn/gtpnoiwaff.html

Py:   s.find("x");  s.index("x")
来源：http://hz.chenzaomai.com/gtkqencbyg.html

PHP:  strpos($s, "x");
来源：http://hz.hnxiangtu.top/gteqsktidz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sufxvd.cn/gtahsjoiqz.html

TS:   s.indexOf("x")
来源：http://hz.aibaodan.cn/gtbmzjtxeb.html

Java: s.indexOf("x")
来源：http://hz.zhiwuduotai.top/gtarcjeysh.html

Go:   strings.Index(s, "x")
来源：http://hz.yvedp.cn/gtjeizsynt.html

Ruby: s.index("x")
来源：http://hz.hysaishi.cn/gtruoxvpfi.html

C#:   s.IndexOf("x")
来源：http://hz.ybcxt.top/gtuvlfbbbt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ppjwa.cn/gtmyiueuki.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.daxiang520.top/gtwxrolfgk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.meibo888.top/gtjnrgqldk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xuetiantiany.cn/gtmjfszrtr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hongshengwenyu.top/gtyszxpmat.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ybcxt.top/gtzdnkemhy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.redwolf501.top/gtfyfvmlws.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.nanxinkj.top/gtjykvgupr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xuetiantiany.cn/gtoplznzjf.html

[E06] 替换子串
来源：http://hz.zhoulong.xyz/gtgukhirht.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.dianchejie.cn/gttxkqiirr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.andypj.xyz/gtogejrort.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtaoeeksrc.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yanxiufei.cn/gtoxfapceg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtmshywhcy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yongpay.top/gtcxzrlswy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.redwolf501.top/gtclrfdlpg.html


<!-- 参考信息 -->