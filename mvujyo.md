代发 wailian999

Ruby: a, b = pair
来源：http://hz.yuanzhike.top/gtaydfrlbv.html

C#:   var (a, b) = pair;
来源：http://hz.zhongyouzk.top/gttvrawwry.html

[C16] 函数 / 方法重载
来源：http://hz.mhx1999.top/gtwzvuqbqz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinghuilouyu.cn/gtepqtotky.html

PHP:  // 无重载
来源：http://hz.shanyushiyangkeji.top/gtwnqgcych.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hysaishi.cn/gtyhsdvuae.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.mhx1999.top/gtvdtfeuoh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.wangdashe.top/gtpxqremie.html

Go:   // 无重载：用不同函数名
来源：http://hz.hnqzz.top/gtfszvxfjq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jyoumei.cn/gtqwqwijhq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hywenlv.cn/gtyuegckve.html

================================================================================
来源：http://hz.jqgfzy.top/gtoodrygbf.html

D. 数组 / 列表 / 集合
来源：http://hz.ivvv.top/gtbpuiufrh.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtsskujbjj.html

[D01] 创建数组 / 列表
来源：http://hz.chenjidiqi.icu/gtfatbazdt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yongpay.top/gtjusdquwa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ydzc1.top/gtikfljwbn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.iojbl.cn/gtfikqqomc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.wangshuangyany.cn/gttadavbub.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.quarkkingdee.top/gtjfmtryuy.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hysaishi.cn/gtewqouqbh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shanyushiyangtech.top/gtwngyqfrh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhengqikj.top/gtngamkdky.html

[D02] 追加元素到末尾
来源：http://hz.zhengqikj.top/gtyiluzqnl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yj202588.top/gtrjzcxgdp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sufxvd.cn/gtgklraobo.html

JS:   arr.push(4);
来源：http://hz.nanxuanxn.top/gtljxqszbl.html

TS:   arr.push(4);
来源：http://hz.cashguo.top/gtksdhqlyz.html

Java: list.add(4);
来源：http://hz.hywenlv.cn/gtevxpoget.html

Go:   arr = append(arr, 4)
来源：http://hz.cashguo.top/gtwspbybge.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shzxlz.cn/gtnmrqehms.html

C#:   list.Add(4);
来源：http://hz.yueranfly.top/gtutcbvbsx.html

[D03] 在指定位置插入元素
来源：http://hz.yvedp.cn/gtgthmikqi.html

Py:   arr.insert(0, 0)
来源：http://hz.hywenlv.cn/gtavtvexre.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xingfuxueyuan.xyz/gtxukpymvm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hfpthk.cn/gtbbmkyxww.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.mhx1999.top/gtyiziartb.html

Java: list.add(0, 0);
来源：http://hz.aibaodan.cn/gtuqbdkseu.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yj202588.top/gtgxxgpzdr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.aibaodan.cn/gthreodsas.html

C#:   list.Insert(0, 0);
来源：http://hz.xylfe.cn/gtqvhgrdug.html

[D04] 删除元素
来源：http://hz.pycfn.com/gtybcfzfjr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xuanzx.com/gtcmawbgsv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.pycfn.com/gtihdifhut.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.daxiang520.top/gttcsmruxq.html

TS:   arr.splice(0, 1);
来源：http://hz.pengpengdd.cyou/gtnfxvbxmp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cheryme.top/gthotbkxnc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.0kj1m.cn/gtutivkmtw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.daria6918.cn/gtnoglqmjf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hnxiangtu.top/gtoevmvvid.html

[D05] 访问与修改元素
来源：http://hz.jinqigfzy.top/gtrcfujarv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtmtyictae.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gaohongyu789.top/gtbqhajukv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.chenlongwang.top/gtpbkpcalz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.smart0.xyz/gtaateyfal.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cucudq.cn/gtkhbvfgzc.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gtkkszzvbc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhoulong.xyz/gtwvkzgaoi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinqigfzy.top/gtktumymcn.html

[D06] 数组长度
来源：http://hz.jqgfzy.top/gtqvwrlomu.html

Py:   len(arr)
来源：http://hz.wangshuangyany.cn/gtfqqvawdg.html

PHP:  count($arr);
来源：http://hz.ydjk.org.cn/gtktxhegza.html

JS:   arr.length
来源：http://hz.cucudq.cn/gtnuyrurom.html

TS:   arr.length
来源：http://hz.pengpengdd.cyou/gtumjcadfw.html

Java: list.size();
来源：http://hz.fengsongda.top/gtrrmigthp.html

Go:   len(arr)
来源：http://hz.jiagoushi.top/gtnbsoijxr.html

Ruby: arr.length; arr.size
来源：http://hz.xziqi.cn/gtfkbvkbjz.html

C#:   list.Count;
来源：http://hz.cheryme.top/gtucwmzdss.html

[D07] 切片 / 取子数组
来源：http://hz.9152youxi.cn/gtvestgzce.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.bjfxy.top/gtrjmzwmnx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.9152youxi.cn/gtctrfwuqa.html

JS:   arr.slice(1, 4);
来源：http://hz.xziqi.cn/gturfppbqg.html

TS:   arr.slice(1, 4);
来源：http://hz.jiagoushi.top/gtlhwozuzi.html

Java: list.subList(1, 4);
来源：http://hz.zhoulong.xyz/gtvyprmwnd.html

Go:   arr[1:4]
来源：http://hz.bjfxy.top/gtzsbanwdm.html

Ruby: arr[1, 3]
来源：http://hz.pycfn.com/gtxbyotmak.html

C#:   list.GetRange(1, 3);
来源：http://hz.ybcxt.top/gtazfzgdmx.html

[D08] 合并两个数组
来源：http://hz.jlsjyb.cn/gtujwmxukl.html

Py:   a + b;  a.extend(b)
来源：http://hz.fzhhl.top/gtculqrkqs.html

PHP:  array_merge($a, $b);
来源：http://hz.aibaodan.cn/gthkwakbxb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jqgfzy.top/gtrlpvvwak.html

TS:   [...a, ...b];
来源：http://hz.yongpay.top/gtsimskpdq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.vqdsnc.cn/gtumthwwpi.html

Go:   append(a, b...)
来源：http://hz.ybcxt.top/gtxbghkrxt.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jqgfzy.top/gtonycedka.html

C#:   a.Concat(b).ToList()
来源：http://hz.guannengcc.top/gtmsdxbnex.html

[D09] 排序（升序）
来源：http://hz.9152youxi.cn/gtboqvrgxv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtzxxbmlrf.html

PHP:  sort($arr);
来源：http://hz.redwolf501.top/gthzbcjirs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.pycfn.com/gtigacvkdt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jianghu66.top/gtraoubqaa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhongyouzk.top/gtidwtzmce.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.wangshuangyany.cn/gtwnkzeeqv.html

Ruby: arr.sort
来源：http://hz.fengsongda.top/gttmnjmoqd.html

C#:   list.Sort();
来源：http://hz.ppjwa.cn/gtdrtmmcim.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shanyushiyangtech.top/gtxdaccprm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hnxiangtu.top/gtwhrwghek.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nwbrower.top/gtqxfaejqi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.svipenyu.cn/gtmltgdgvg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gtymydprwf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jyoumei.cn/gtttddytva.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jiagoushi.top/gtxeckgsnl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.dashuyun.cn/gtzkonelnw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinqigufen.top/gtzaiwarxy.html

[D11] 反转数组
来源：http://hz.sysykeji.top/gtlpdkqigk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cucudq.cn/gtdijbnlnz.html

PHP:  array_reverse($arr);
来源：http://hz.quarkkingdee.top/gtjtdgqspu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xuanzx.com/gtldibkudg.html

TS:   [...arr].reverse();
来源：http://hz.guannengcc.top/gtygrwolwy.html

Java: Collections.reverse(list);
来源：http://hz.zhoulong.xyz/gtnzckpaps.html

Go:   slices.Reverse(arr)
来源：http://hz.vqdsnc.cn/gtbxwgbpdu.html

Ruby: arr.reverse
来源：http://hz.ppjwa.cn/gthgzdtnba.html

C#:   list.Reverse();
来源：http://hz.yj20258888.top/gtwbinjrfv.html

[D12] 查找元素下标
来源：http://hz.yueranfly.top/gtusskobvz.html

Py:   arr.index(x);  x in arr
来源：http://hz.gotoacloud.top/gtwphuibcy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ywan-chungtsiang.top/gtdqkubepp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.52xcode.cn/gtdmvcqqff.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guannengcc.top/gtqeuprdgi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.pycfn.com/gtkqsgymjt.html

Go:   slices.Index(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtsxuvfnvx.html

Ruby: arr.index(x)
来源：http://hz.ivvv.top/gtfywjuvcx.html

C#:   list.IndexOf(x);
来源：http://hz.yuanzhike.top/gtluebrpea.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gzhubu.top/gtsizkgmqo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nanxuanxn.top/gtygceyfli.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.quarkkingdee.top/gtoukrlyll.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangtech.top/gtylmhhxnw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sufxvd.cn/gtbztqrpuq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ybcxt.top/gtyucrdxcu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shanyushiyangtech.top/gthbhaxxfm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.316326.xyz/gtlbmyzade.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.gotoacloud.top/gtavvsfatz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ppjwa.cn/gtxeposxop.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yj20258888.top/gtdqbvywkx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cdnleiting.top/gtpygiujjq.html

JS:   arr.map(x => x * 2)
来源：http://hz.yangfankeji.com/gtdtkmocuu.html

TS:   arr.map(x => x * 2)
来源：http://hz.tanke756.top/gthsalopmo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.aizwys.cn/gthmgnjgsg.html

Go:   // 手写循环
来源：http://hz.sysykeji.top/gtabxngbci.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ehwqpu.com/gtyygxstcd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cucudq.cn/gtpguxosay.html

[D15] 去重
来源：http://hz.jinyuanbaomall.cn/gtdjywazbz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.redwolf501.top/gtpoypzmim.html

PHP:  array_unique($arr);
来源：http://hz.wangdashe.top/gtocjkixnv.html

JS:   [...new Set(arr)]
来源：http://hz.zhiwuduotai.top/gtmepozfsa.html

TS:   [...new Set(arr)]
来源：http://hz.yuxming.cn/gtkvasilwv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj20258.top/gtgznhfxmj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tian-w.cn/gtwoghgqlc.html

Ruby: arr.uniq
来源：http://hz.xuanzx.com/gtqjiqglei.html

C#:   list.Distinct().ToList()
来源：http://hz.cucudq.cn/gtqqfgaagu.html

[D16] 求和与平均值
来源：http://hz.zhijiandao.cn/gtnfnumwxu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.redwolf501.top/gthgmmpspy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.kuanghao11.cn/gtedlqeczy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daxiang520.top/gteqccljaj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.0kj1m.cn/gtmhrvdlcv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gaohongyu789.top/gtuydktbuj.html

Go:   // 手写循环累加
来源：http://hz.jqgufenzy.top/gtltntbenj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.snrcjt.cn/gtwpteemly.html

C#:   list.Sum();  list.Average()
来源：http://hz.pengpengdd.cyou/gtrgsupgas.html

[D17] 最大值与最小值
来源：http://hz.jlsjyb.cn/gtwuclsvdj.html

Py:   max(arr);  min(arr)
来源：http://hz.jiagoushi.top/gtbimefhav.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxuanxn.top/gtorsgfgyx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yuxming.cn/gtgvzyddjp.html

TS:   Math.max(...arr);
来源：http://hz.hnxiangtu.top/gtongsofta.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.nanxinkj.top/gtivpxxrzn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yuxming.cn/gtotwswqyc.html

Ruby: arr.max;  arr.min
来源：http://hz.meibo888.top/gtegmivnwu.html

C#:   list.Max();  list.Min()
来源：http://hz.hywenlv.cn/gtezeverst.html

[D18] 扁平化嵌套数组
来源：http://hz.hnxiangtu.top/gtqanzkyec.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenjidiqi.icu/gtqvkzihyu.html

PHP:  array_merge(...$nested);
来源：http://hz.shanyushiyangtech.top/gtifzlgtbm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xingfuxueyuan.xyz/gtxmekkhjt.html

TS:   nested.flat();
来源：http://hz.gzhubu.top/gtmjrascem.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ydzc1.top/gtbuhcavsm.html

Go:   // 手写双层循环
来源：http://hz.jinqigfzy.top/gtgfonaent.html

Ruby: nested.flatten
来源：http://hz.jqgfzy.top/gtplfeeegr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtzwwfenaw.html

[D19] 按字段分组
来源：http://hz.dianchejie.cn/gtmnuffnjw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hongshengwenyu.top/gtrizodidf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nanxuanxn.top/gtjxcjclmr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ivvv.top/gtcwxmzvlv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xuanzx.com/gtfhiahhni.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dianchejie.cn/gtkifrqmpz.html

Go:   // 手写 map[string][]T
来源：http://hz.hfpthk.cn/gtalwsudsy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.daria6918.cn/gthcemofkg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.wangshuangyany.cn/gtlnlhlzpw.html

[D20] 统计每个元素出现次数
来源：http://hz.hammf.cn/gtqnruinak.html

Py:   Counter(arr)
来源：http://hz.xuetiantiany.cn/gthlpwnfme.html

PHP:  array_count_values($arr);
来源：http://hz.nanxuanxn.top/gtdsinkvdq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuetiantiany.cn/gtgunoekjg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ydzc1.top/gtkummuisw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xuetiantiany.cn/gtlmqabeeg.html

Go:   // 手写 map[T]int
来源：http://hz.xuetiantiany.cn/gttoemmiuq.html

Ruby: arr.tally
来源：http://hz.ywan-chungtsiang.top/gtemdupsrp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.guannengcc.top/gtancyukks.html

[D21] 判断是否包含某元素
来源：http://hz.jinghuilouyu.cn/gtkhyycmva.html

Py:   x in arr
来源：http://hz.jinqigufen.top/gtzifqcyhf.html

PHP:  in_array($x, $arr, true);
来源：http://hz.chenzaomai.com/gtyixwcadg.html

JS:   arr.includes(x)
来源：http://hz.yj20258888.top/gtudykpfeh.html

TS:   arr.includes(x)
来源：http://hz.tianlin.xyz/gtsyldjfxq.html

Java: list.contains(x)
来源：http://hz.tian-w.cn/gtwdokhjgm.html

Go:   slices.Contains(arr, x)
来源：http://hz.bjfxy.top/gtfdkccybx.html

Ruby: arr.include?(x)
来源：http://hz.316326.xyz/gtjwtofvms.html

C#:   list.Contains(x)
来源：http://hz.wangshuangyany.cn/gtyvgieosl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhiwuduotai.top/gtvcaubutu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.fengsongda.top/gtpumljdgm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cucudq.cn/gtwgcyytuf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hysaishi.cn/gtocbuxoow.html

TS:   [...arr];
来源：http://hz.9152youxi.cn/gtnufnavjl.html

Java: new ArrayList<>(list);
来源：http://hz.chenzaomai.com/gtyecqtvfi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.52xcode.cn/gtauffozlj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gotoacloud.top/gtgwdttzxs.html

C#:   new List<int>(list);
来源：http://hz.0kj1m.cn/gthpauaiam.html

[D23] reduce 累积计算
来源：http://hz.yvedp.cn/gtypiouekg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yueranfly.top/gtprpxbacm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.316326.xyz/gttonvqdzo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gaohongyu789.top/gtnubiigup.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fengsongda.top/gthlieuitd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yuanzhike.top/gthhipzubg.html

Go:   // 手写循环
来源：http://hz.chenzaomai.com/gtykvlmykg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhoulong.xyz/gtdalajfke.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ydzc1.top/gtazmwqhal.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhixingplan.top/gtddcwgwkw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hongshengwenyu.top/gtaowanubg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yongpay.top/gtuosagugd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yuanzhike.top/gtwrdgdfpc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.bjfxy.top/gttpzpkphn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yj20258.top/gtcvgksvxj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.0kj1m.cn/gtphflgrkb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.andypj.xyz/gtseiijcvj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.pycfn.com/gtuqzhsflo.html

[D25] Set 集合去重与交并差
来源：http://hz.vqdsnc.cn/gthjbsbnel.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.c1oappe.top/gttfhhoafi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.guowangkeji.top/gtzhetpryr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yuanzhike.top/gtyansbfbb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.redwolf501.top/gtyiyfbixv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jlsjyb.cn/gtzcfdscvd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yuanzhike.top/gthipgjxnp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shzxlz.cn/gtqhuwpnpx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.nanxinkj.top/gtqdogpein.html

[D26] 数组转字符串
来源：http://hz.chenlongwang.top/gtcjcwsjtg.html

Py:   ", ".join(map(str, arr))
来源：http://hz.316326.xyz/gtrssusekk.html

PHP:  implode(", ", $arr);
来源：http://hz.zhaomingkeji.xyz/gtcmtkgicn.html

JS:   arr.join(", ")
来源：http://hz.hongshengwenyu.top/gtyvyjxzqf.html

TS:   arr.join(", ")
来源：http://hz.zycfv.cn/gtbxowhjhk.html

Java: String.join(", ", list)
来源：http://hz.jianghu66.top/gtfbxewwue.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinqigfzy.top/gtqehputru.html

Ruby: arr.join(", ")
来源：http://hz.xuetiantiany.cn/gttrnccpam.html

C#:   string.Join(", ", list)
来源：http://hz.yj20258888.top/gttribkmhb.html

================================================================================
来源：http://hz.gogol.net.cn/gtwxmflbxi.html

E. 字符串处理
来源：http://hz.tian-w.cn/gtqmmpecns.html

================================================================================
来源：http://hz.hammf.cn/gtjflmatps.html

[E01] 拼接字符串
来源：http://hz.aizwys.cn/gtewghmvem.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hammf.cn/gthlhxvwpz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gogol.net.cn/gtrkawiuuo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenzaomai.com/gtgbcnfmhy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jiagoushi.top/gtrycyucmh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenzaomai.com/gtbinaadkv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.havefunace.top/gtzjnrwqpc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.guannengcc.top/gtqwcjippu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhengqikj.top/gtljiksqfz.html

[E02] 重复字符串
来源：http://hz.jqgfzy.top/gtsvsmobss.html

Py:   "ab" * 3
来源：http://hz.vqdsnc.cn/gtjzdtoynx.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sweek.top/gthqoiadad.html

JS:   "ab".repeat(3)
来源：http://hz.yuxming.cn/gtlhcxzrmo.html

TS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gtosqxfwpe.html

Java: "ab".repeat(3)
来源：http://hz.sufxvd.cn/gtoyclarex.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinghuilouyu.cn/gtzykmsnlb.html

Ruby: "ab" * 3
来源：http://hz.ehwqpu.com/gtnbpctzhj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.pengpengdd.cyou/gtqienlmyf.html

[E03] 截取子串
来源：http://hz.jqgufenzy.top/gtoetopest.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hysaishi.cn/gtfcpkfwxe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.fzhhl.top/gtsqgpoiqq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.feifeiyinyue.top/gtafyueskj.html

TS:   s.slice(1, 4)
来源：http://hz.sweek.top/gtikwcoaay.html

Java: s.substring(1, 4)
来源：http://hz.yueranfly.top/gtageknzzo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tian-w.cn/gtgkaogpqd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gzhubu.top/gtlpzklxka.html

C#:   s.Substring(1, 3)
来源：http://hz.feifeiyinyue.top/gteemggjxw.html

[E04] 查找子串位置
来源：http://hz.hnxiangtu.top/gtcngjgryg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jianghu66.top/gttvvrcdaw.html

PHP:  strpos($s, "x");
来源：http://hz.tianlin.xyz/gtgkdxgcjf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hnxiangtu.top/gtykuapepa.html

TS:   s.indexOf("x")
来源：http://hz.xuetiantiany.cn/gtiglhcahq.html

Java: s.indexOf("x")
来源：http://hz.cqqwz.cn/gtavizmzpq.html

Go:   strings.Index(s, "x")
来源：http://hz.sufxvd.cn/gtrizlrsuo.html

Ruby: s.index("x")
来源：http://hz.ydzc1.top/gtfpaxykfh.html

C#:   s.IndexOf("x")
来源：http://hz.zhixingplan.top/gtqpcyarvp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cqqwz.cn/gtbjdutwjd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ybcxt.top/gthgcjjvhz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jlsjyb.cn/gtruoxualz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cqqwz.cn/gtgloyxhaj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.52xcode.cn/gtznnyuytn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hfpthk.cn/gtembfrglz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nanxuanxn.top/gtjpuepynp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hongshengwenyu.top/gtxqhzbtci.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.vqdsnc.cn/gtxhaonzes.html

[E06] 替换子串
来源：http://hz.sufxvd.cn/gtcjqtafhd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.guowangkeji.top/gtpztbsxxd.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yj20258888.top/gtaejnlhaz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtlabucsml.html


<!-- 参考信息 -->