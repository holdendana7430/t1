代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gbwkboxqn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gzctfassx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gengjyeom.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geugsecdj.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gbyigpezq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/geadrlwkp.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gnkurrnvz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gqolvkdny.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gnavqvahh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gthitshgv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gqidbwxtl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gqxqjmqzu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gfdiqpwam.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gvcmqekwz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gmpyruvhr.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gtbggclwu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gyhrcvxue.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/ggedcsybr.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/goxvlruyh.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gltcgcvnx.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gjtaxqaxm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gbraacxdh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gvhkiuekk.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gfnryfkmv.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gwnhqxumf.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gtokkafbw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gfpooziac.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gxuycawxp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gwdcbqbpw.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gkktxbdkv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gbdqodnju.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gkgwlxqin.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gdqcvnqoa.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/grfmrohej.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gqikjlwmo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/glrpvgptt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gimohtsqk.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/glztqpetv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gezsidtuk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gaukwfkrf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gigdaloyz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gndnqcpqj.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/ghqskfyau.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gdmsyuwov.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gtdcpbukn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gkdeaxpul.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/goxlnkjut.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gylgdxwdf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gerseykfg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gxzawdzls.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gbbzcsiym.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gtydjocft.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gclaffhbq.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gfqevsbgd.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gbqneaxbt.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gvjxweahs.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gzhgfoxug.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkpyjmjlz.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gqkztqpyu.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gipudicfa.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gmbzyjdhk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gfqulwvux.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gbqeihpjk.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gptzlefuk.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gphuipnfc.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gandcnfcp.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gmoxjpwnp.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gqbszjqnz.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gzcpocbxs.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/goaxwzjwp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gwyhhghbm.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gznbwlwyy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/ghxlhooqc.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gbgvauxec.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/geytroaic.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/ghvivstbn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gxoykqpxk.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gcrmbptyo.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gtrbsqfcq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gtpojhelr.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ghvogwbfg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/ghodejywo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gxuroshmr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gxdyjckek.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gyonsppbq.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gdsxvlwjq.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gqlafdpbt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/ghinhqdgx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gztdeqnta.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/grdoavzmm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gzgdlhdlx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gmfgtzklr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gzhlfozno.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gffzqwlqi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gqymgfaum.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/garqofapv.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gktcrxbgu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/girdlkjjf.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gyhylxbsv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gintrizro.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/ghgprckii.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gfwmtulzs.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gyvvhzapw.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gcovhqpse.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/guhlafesx.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gfrikcirg.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gedmgzhzx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gxyxzmwib.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/geaeewcbu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gqwgvqpno.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gticydqqq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gchnjwdqb.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfuekvpgc.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gpdudcxak.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gclggxloy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gvurgokdt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/glatyocbi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/grigkxjir.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gtqwdgjon.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gjjhxpdqv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gdpxvdrui.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/glhdwxiva.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gcjblquit.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gswbykhro.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/ghkaabxhb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gynmezqqt.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gnbylmjpt.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gkmcqfzsh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gjpkaasou.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gcsasptfv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gjudgyxqo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gdzesdlnh.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gdeitcohq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gusvtfspy.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gllevoxiv.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gnlidgjxi.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gifmlhuft.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gfvfrapzb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gwoobmmbr.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gqieezjnx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gusqihcwr.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gyaizgjou.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gqvucmnzs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzkiaipgm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gyipevsbi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gkndulzcv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gyblghtda.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gajpybnzt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gxvmaklnq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gbmhjbyfu.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gfmmqmmkn.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gihqxqtgn.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gdnfhzftj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gcnozlyae.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gpbnhlopo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gwjylzdge.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/guhyrrfrw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gcwgjbqxr.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gddlvscsm.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gjfddhzms.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gazjhraeq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gyfvmszez.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gxfxzehvh.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/grcjibkrr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gcttjllow.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gbdtpqkhk.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gnoyosker.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfzpxhcbt.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gtdrxlkjt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gtrnrnggf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gpeszhgto.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gxryfjhqs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/glesydcix.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gpdtzqtzn.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gfqlqsdan.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/guzgzsezz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gfclxeuvv.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gsdhecjry.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxlxpmcja.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gvddpphll.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gujkghpng.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gcpuqqbei.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gsbzlpgzy.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/ghampckre.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gmzruubbj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gecrccpnr.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gueftattc.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gusyidjym.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/guqtsewrj.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gackbplrc.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gqndqageb.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gwytyoxlg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/grmeilhgb.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gaglrugam.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/ghwbfaift.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gpipwlrru.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gyvmsupxa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/grjsfmtqa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqkmtqxas.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gzrqkitnt.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gcdqufvxa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/geqdpxajw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gcjogmcfs.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/ghtserfea.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/guzidwzxq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gqzcncmbg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gyjjumfoo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gzdruwwyf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gpyjwvbqs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gwzhohxtn.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gnvzykahm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gvhywdtvs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gxnrretlu.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gkqrspavh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gouxksuir.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gipidotmc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/ghdmfuffl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gchdaknne.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gfdwtlhxd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gvixtyiqo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gbdyplulp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gyqfrvltf.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gnzyyizxn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/galmharib.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gwygbfcww.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gjppamupx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gahzbhoht.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gcfbmdmxj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gekduifum.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gzdnzdgho.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/grqsoacgb.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gapwweuxu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gqhvxaoba.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gzgcjxqby.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gxvabnbbb.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gqbpcudxn.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gbtwkezkd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gmfcginpf.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gwhtzzmgi.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gqswhlunj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvzbsopiq.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gdvnstchh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqdjwntgr.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/ggmcinvnb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gtfdzogjy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gezhbpdyh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gkxoxphly.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gbreadunt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gckyuvnyl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/grzincvjt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gfwfdzqgm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gudtrvvam.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnawvsuna.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gwktavyuu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gpugojyyz.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gcxyvlmjw.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gqdmtgkoe.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/glmqfzwxe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gjdmrirhd.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gwzdnwafq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gkwljszlu.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gkdtlsxkm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gmpclqvsf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/ggtpnklkh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/ggxofyxrr.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gimogiwrm.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/grgzobbel.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gimclljwn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/guakiersg.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gwijflxcp.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gcmimmwhr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gatctkjaq.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gcrbouefh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gwsrnbhbt.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gmrbqxbbl.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/giyxfxmwx.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gvubxyzxc.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/garisygcp.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/grtixtmgl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/ggcaperph.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gcxundyph.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gabhqytik.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/glwlobasw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gpwonxlne.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/geyptujeh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gaplkdkhz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gjoqybavr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gssfbzjxk.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/glcpwrktb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gmuuamgwa.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/guvfzdjpn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gstiqatsp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gzczryetd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gzugbcjnz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gyuukybbo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/glsszkgpp.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gacmnthld.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gfitkjwiv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gcbhoewur.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gzxlhwecg.sHtML


<!-- 参考信息 -->