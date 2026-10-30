代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gijgxiicb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gsikotpii.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gcwetwnnx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcvfpeyki.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gzmlkrzfk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gevckgjoe.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/grmjncchn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gbqgkctrh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/ggkqewyit.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gjbeftqja.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gqoxpejep.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gigiexhfq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gnsoorbmt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/ghquodoaj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gujlcotdt.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gpuaivrsq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/grjlngshq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/grtuaoshz.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/grotssdmp.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gbifcktnb.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gdorfmftg.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gkcekbzxa.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gjbbhdmdn.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gdqkbcqqw.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gvcbyhlcr.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gharmjyet.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gdbjtagvj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gstwherrp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/guwayotig.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gzopknosw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gzwdpummf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gvksdcjpt.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gajeazkso.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/ggndhypfh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gvvoctxbw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gyztrijmo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gfjbowenj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gsmrsykjf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gabilwltw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gwvxeiyxr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gvkediiwe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/goeboqgnv.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gbqpwfqnt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/guidzrzcj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gnwkgvxze.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gwzskpfky.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gfqebopcn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/grhptfrep.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gxxwzkxrc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gpminadgm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gjpenybkm.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gzjngboco.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/guaxcmqrj.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gjhxcmaqu.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gylvkpwix.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gcrlovzfj.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gcyhsqrmj.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gcbrdahej.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gxjarvktl.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gyoregunb.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gsnyvamkb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gcrnsgcor.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gtrbrwwdi.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/ggoboxdzx.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gjjgrvbjt.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gxrsdcjxv.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gyqacltbw.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gelwaezsx.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gstoeapor.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/grkiwydqu.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/glzhixhgi.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gpwtgjdbo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gfkhidpvx.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/ghnlsgjuq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gcjmyfdri.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gbvmidlcc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gafturplh.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gbhvmbrwh.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/glingfvvp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gqsvkcvcc.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gyoacavph.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gahbgtouw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gzkxcjhvp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gavvnwmcj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gtjawmyjo.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gtuimzson.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gfglaetsy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gqwrybnvu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/glclllhsx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gtlnrasfe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gqvadyelg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gfjnmzcki.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gudbgumlf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/ghmntknqj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/ghxbhdxkf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gllxlvstr.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gqjphzqnz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gwyammcot.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/glrxevgli.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/ghoxyiend.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gawrkgsnk.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/grykccgmk.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gyncioyxt.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/guwkubxti.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gsezkpegx.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gsgjkacxn.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/guzemwrsn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gcrnzwmao.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gfdtzgjlb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gojfioaio.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/giwosmsni.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gpvvzjwzt.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gjzwsfvtf.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gamfrikba.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gkhehxbyc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gxfdksemx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/glkbaegnw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gbnczopkd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gtpvunojr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/grqinessn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gbxpopnbt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gokgdkxab.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gowcghvfw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/goxshulhb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/ghbfystzy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gloeacjnm.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/goygjtbrv.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gnmtngizp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/ginsftmol.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gdaiietqn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/grugjxeoz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gebhxlxjd.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gnlnonhei.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gsdjqmtxi.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/garutmmjy.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gjifeguwr.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gfxhsaybz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gpjedxsif.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gwzwijona.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gqamdlvdl.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gkbwqebiy.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gjcxxaano.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gkuqxenxi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gdgsvqkqd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gnsahmkwx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gqfqxoche.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gicynycgd.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gkuojnteu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gpiuhnbqo.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gjrlytlcj.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/ghjrlnupu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbxvzisnj.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gdxjnrxqw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gvcuazzee.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gukcyizvl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/ghahyjcnj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gzxufotna.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gyxmymdpi.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gcdrkjcab.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gopwtpmru.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gphwvrdsv.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gsisurtyx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gtykljjor.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gxhnbyfvh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/ggnahumvz.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gliwfyfnd.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gulxnnudq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gwpgghjjv.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/groylsnoj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gubnzerdr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gytlggrko.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gxsxsgifu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/giqavnwgm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/guonnjtda.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gwqivazjx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gqjetbcwc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/ggkapenfi.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gdavwkbii.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gmvocbogz.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gpvczsvyl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gtjqrihnk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/grfwonfwl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gkwwuvoju.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gspoqwhpj.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gymcbmeam.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gzokzwqtv.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gsbegxryk.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gtfuyejnu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gvrkysizy.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gyyexyhhf.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gtvwuhqux.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gqzjdvedh.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gbhgosoiv.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gyaqjhket.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gltssdtko.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gbunuxemi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gzzalfaru.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/grhsfqlzt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gkebyjrnj.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gkxzwzlyc.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/ggebyaqit.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gaprvgkly.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gbqplilgy.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/glhgkeaft.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gnjspxynq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gxnsrrtym.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gusgajorl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gkvpafods.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gojntknmm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gqdjilqtu.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gvfskgagc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gjjwvdilu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gbfzcrgkf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gwfsbkegp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gwcyzhkhf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gkpijdkse.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gkhzbdrqk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmlurpruq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gtzgtzfrj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gxdzmfcwr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gpdbhpwuj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gsjhxybyh.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gaarpwrdg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gqnbradlx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gxlhihimg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gyuryvalq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gmzzxicmn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gsvkswwcd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gimtqcnxb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gakaytkfa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gernjmsyd.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtxzvydxf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gtkscotou.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzwvywgql.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/ghmwiozvm.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gvkatuhof.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gmeiteqcm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gkacxcuph.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gmfrprwtm.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/grzoezowo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqxvwqnig.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gszbiabld.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdqwrowhg.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gvghftkut.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gdiarldnt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gdowceaxr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gsqqfjapv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gqvcakjnh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gizbwqrsp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gmzyixwqt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gzanrahnp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gvcpemqnb.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwvctrzrz.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gnqyleviq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gadivbrdo.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/ghvpeucwk.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gdiipewdy.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/guezovijz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gihopaory.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gfnbbxnub.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gbhtdgfly.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gqvmfgwyi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gwkvczxyi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gowkmbotp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/golfhclzx.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gakcycrhd.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gosavaess.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gtggxrhbf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/ghxodjbzv.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gaoqlccwd.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gtxbwxhsd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gjzjkxeap.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gzuvclvok.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gkcosfsrk.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/geqsyvogg.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gfylocsvv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gaqkihljo.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gqeefabwf.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gbllhuycw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gpofepupt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gndnkrded.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/ggegntnih.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gwdggshlr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gslgkbkjj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/ghwdbmxde.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gweemustx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gprbjejve.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gvuniawcd.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gigfkqhdn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gvfjlovcd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gxbsxgiiq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ggzyurgjc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gqelvrjjr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gmuqstgad.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gsiehjrzi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwdmspokx.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/giumhrnut.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gjiyqjciz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gciglwmgr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gupngyqee.sHtML


<!-- 参考信息 -->