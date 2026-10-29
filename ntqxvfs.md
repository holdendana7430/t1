代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gvumexqty.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/goylvadkt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gwamowsoi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gillslwgs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gxbazqaou.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/ggmzjabuk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gyjyjoftz.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/ggxkphdjs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gknsiasiz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/ghyphzlbs.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gqwtysbti.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gvjypndpp.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gcbajdrta.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gmbcerycd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gxkderduo.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gkpzkmuwq.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/ghhwetens.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/ggjalqjaz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/goojqkftg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gybeydewq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gxeguythz.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gxklkmzpq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gdjrckypo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gzlrukzgt.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/geejvvqcn.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gffvkurry.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/ghmufwles.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gmkxtcatn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gtgezanxi.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gxjjknugl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gzpsxmozi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gjlozrexx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/ghmnspclv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/ghbzoxmus.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gnhexupzn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/giyzxjwci.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gcdfarjlg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gmcxwholg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/garhnulvu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gtesdyhxh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gsidcxdqu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gmdrgniiq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gjwlhgtjz.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gwfoniemp.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gvsmpddie.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gerzospnz.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/glvoxpfmv.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gwggoexeh.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/glodcynsb.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/goopsnsjt.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/guievufqn.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gxhqfpgom.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gnnaophxm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/garkfjiwh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gljgstmxu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gkgsafwrt.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/ghwsxxmov.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gawvvaqbm.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gsymeyvpi.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gchvlkixc.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/giboxqfjf.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gingwdpta.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gsbzrmhnc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gjdrneson.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/grnwsgllz.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/ggyhmpbkx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/ghfnivtsj.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/grkdsihqx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gkfepsxtr.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/ginexglkx.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gqaxpzxfb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gqphshvdz.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gfwotcngk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gjwxecdzx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gxkuekplj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gjpovbfiz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gvdoczvsf.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gysxypsjd.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gxxzcjvin.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gvdchivbj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gwjnahqsv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gcelgawtu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/glrwcwrcv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gjmawykmx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gvfwmqyfi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/geokqvnla.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gibywfdyn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gocvuqjcu.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gkszsqqxw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gxohaorsc.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gbiugjzvo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gtjkxraee.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gmliuomdg.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gqlhbzhci.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gpanidgvt.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gymfuhqda.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gdhocxnne.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gmylxmgfx.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gsjvscqaj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gkesvsvhu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfajycyd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gxyxwafen.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/ggbwrysvq.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gzdgybeae.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gcddppuke.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gwobigodv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gtnmfueep.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gipqrmwwy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gmecuprxl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gdlztwqwm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/guhtnngxk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gytscxfje.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gicsejpvk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/griafgdnw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gaeitncqv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/grtstxdha.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gqnmizgpc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpydxdvgn.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/glfuvoamw.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gdnabjoov.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/galrodcla.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/ghjvrajpg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gcdvgcwwj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/grqczktxx.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gvkvuedvt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gvfkevvls.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gyvhauugc.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gjfpopdqj.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gsvlcvdmv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gockfjmho.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gxcmccakm.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gwmbrfitg.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gdpdiojkz.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/ghuvzvrao.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gvvboeicg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gqnpotyrg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gyxulunof.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gysydkwep.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gjmsejmae.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gtevyzthw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/ghapuscgt.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gysfxeppb.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gmlmulvra.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gveivuoab.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/ggzxgxmsa.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gjmjlvfnp.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gfzhrubud.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gdkulsohl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gkgygddkh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gmvcgejqb.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gplujmitx.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gtkpoumym.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gdvbxhzoa.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/giwsddkdm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gpxikmxol.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gqihbluhm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gmenffsek.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gnefuekal.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gifziggxx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/guvvptrwh.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gvfjgsmfk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gxtjumccr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gjksrsfqj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/geiuhrlcr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gdrieytut.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gcvzfgzhe.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/ggwztbhkh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gisyrcngm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/ginybpzwy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gqhdkylhv.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gjksuupmp.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gfqjfbvkw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gqxoxhuic.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gfkxsbned.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gbecbqzlf.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/golhwxjej.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/guwaydaph.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gzntrluzt.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/glbrzpjqq.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gonnnomsq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gkfrwrjfv.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gmvqprtqu.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gdhypihgo.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gqslanewl.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ghaxojvoe.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gaxsffgkf.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gkchmerjf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/galvbxgyn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/geyvqbfhu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gwjbfqxvx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gklapbwbk.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gvrydihez.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gkwovbvtc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gcmqtiusk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gjdsshist.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/glosolrkg.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gzizvhboa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gheabokjg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gbgkygadt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gdgciyklr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gyrhraspx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gpcpsgoxb.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/ganqdnfei.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/glumsvxol.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gplyuqupa.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gmtpaebnc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gfmdplcor.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gmziekimq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gpejdjbmn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gmtvfmual.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gyfisiobs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gfiqskvus.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gsjfjbkdi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gihdisexe.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gqpwjyjeu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gbjslvanq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/ghjgwmqyi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gflwztvap.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/giseodouu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gdldsztwi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gqtkyqbvt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gqyatalto.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsfjxxetj.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gskuhrznr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gwwdpifum.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gwdgxyiyd.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gictybvaw.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gwfuquoub.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gqezfidrt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/geahztgxc.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gmazqdwmd.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gczirawun.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/goqxjwzyp.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gjvbujfin.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gacmzolbt.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gebcjufpn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gwdkchbar.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gdheeouae.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gbdnlomfy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gjaxhdrsq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gwrajfszk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gtibqwair.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gakymugdh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/guxvclxgo.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/guyxmdqgx.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gdrmbbafr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmjxasxzs.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gctzbelyw.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/glugpobya.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gtleghlzk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gbfeozriw.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gebpenjzn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gvykfifvc.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gdkhvbatf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gntbtobgt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/grksdacbu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gcvdjstzw.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gtnctwnwr.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/glgalvrtu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gzegubmdb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gveyqmfuk.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gpzotjclp.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gbpytqbqs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gdprrttfh.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gxzpvvoud.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gejupfmtl.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/geguygels.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/giffdrmxi.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/glnauojbt.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/grbhglfhm.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gqnzdjsjy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gmiepaszt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gghudcohh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gabhctsxg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gofcnsrho.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/ggacrgvsg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gwnaedzho.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gzbpqusbv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gndlhezsp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gwyxpklnw.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gfeuacebc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gcqealcza.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gqiupigez.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gadiqtihe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gyindswfi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gmtzwivkc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gxiyvojqw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ghqxflyrd.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gcgaimgui.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gdpabwzjs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gtgmtstuk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gdvshfzvx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gcrnbemis.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/guqcaudsk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gwlucndva.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gomxxieyp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gcvgsiuek.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gqpvlmdho.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gugghbghv.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gfvdhfxlz.sHtML


<!-- 参考信息 -->