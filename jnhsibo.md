代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gnekkgtvp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/ggjqqiigb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gywevjoak.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqzgrkipx.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gstdzjthl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyajjwonz.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gpjobcngd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gkqmphxae.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/ghmjwaxdz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gjzyswbso.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gqcpjhufn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gzndgwugr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gqdwwpafa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gaamyuwde.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/ghbmuhvex.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gfypdpfjf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gdckpmlwo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gumospnsc.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/ggzplvxqz.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gkahhmfwc.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/ghupjmgyt.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gmydfsjrk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gxfajjxfp.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gcyoysgww.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/guuguwzkg.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gqixqkzld.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gvizaflpg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gghzcqaaz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gcgzflwmk.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gqmpjsijm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/glxrewlur.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/ggonpwlmk.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/ghuzlvqgk.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gvkmeybaf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/ghxothkji.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gahusencv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gztzbmvyv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gazgzglmn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gnliytscr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gmrcfapyv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/ggywvmykp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/guyitmxkr.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gdzmihlfb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gjykjuucp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gdaathwfn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gegrwucwl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/grocjoilc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/grodpfduv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gurwfemxw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/grxdcsvzc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/ghavxjdit.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gbtvmafrn.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gbwibfjgf.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/grtbcydpj.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gmxlytvpd.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gjozviafl.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gahergshw.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gueahlhvb.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gjzrwvqcg.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gamftxjkb.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gillauoyu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gefksaaba.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/godvgdpav.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/ggejeofkb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gvdgaitcb.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gjygfjsop.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gdiaurrzx.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gqxcmkdjl.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gvwcooxor.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gplwvwjbl.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gvpbgvgcl.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/giobjknul.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gujrvxpkl.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gnlxuzhbc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gusaootyf.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gthefhjzr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gvnnleenh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gbsnnkmwc.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gwyoxradk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/glgsthlhu.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gkqklogxj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gvtynjyzw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gaxrmfjka.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gquuqwkhd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gglybbnyg.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gmxkavpje.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gvpysjjoq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/guibbszyv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gblixlmzs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gjetjfana.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gklbfvvcs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gfbiygmjf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gfvwprnvr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gigtfpzgi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gmbehtlxp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/ghhvnpvyu.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gfldyrysk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/grltdqevb.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gunavfgae.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gigtlgawv.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gxuthdvfk.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gjadlrekb.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/geplvqaeh.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/glbcxkrjb.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gxeuwtcba.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gkwtlqwfy.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gxxkvbrvp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gmpoupyuu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gorpwmahf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/guogsayad.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gatyixnuy.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/glkuwtwya.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gpknpptcu.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gkphkzqdp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gxizkfyqt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/ggvfuzgof.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gflhvudab.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gfaeythwv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gklvhlarn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/glbcqhepj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/grfdjbzzr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/grrbglbdr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gxkomzqow.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gvobirysj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gzrnubddg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gkzfytobg.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdjhidgxk.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfieutreg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gwnylsybu.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gsrhmiggt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gwkhvgdtw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gexpgfpmx.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gsnlzdzcc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gmuyxscjg.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvfbyzkxp.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/ggkpbocao.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gqbdawwca.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gnqpkzxrs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/ghhazovdo.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gfybfuoom.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gprloeczw.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/ghcfjmjsq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdmeuvtcc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gafksbwya.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gdbteexsg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gemugultt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gpkcxywym.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/goszpjzdv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gtlcwkoie.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gxdfsdkyc.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/ggkndcvam.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gcigfgfrx.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/grdipeixn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gtzbjbvbk.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvliwvswj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gqpgjdfru.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gusawkzlj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/glarpmuto.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gzjwiwhns.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gubqzilds.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gsgdwihbr.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gldcjhggq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/grygopvwu.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gsevbazym.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/ginbopvzl.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/grsbrnxkh.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gnqcnjfvb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gcsmefwfr.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gywalyhfk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gengtrayc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gnimmtxur.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gmfkrquyz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gatxhurev.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gifdnkrpp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gokwmxiyy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gywgjyiki.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gespnnrvr.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gorhteauh.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/glebrqlzj.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gwyqooxwq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gqznqlnqo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gcvvootgh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gfthjzmsx.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/ginwfiwcd.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gilaxelxw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gbkuzdgva.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/guduzxzmb.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gpszhzcqf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gqeckdrih.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gwogyqlmz.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gktlavgeg.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gasqmwmxj.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gnwdtjyev.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/glxqiptoy.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/grxhvycnk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gmqsvxhol.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gxpjfrmyv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/ggxygrzoq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gvbmxrdea.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gqosyrisb.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/ghtwuwkfx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gnxwuvwdz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gmbbdvxdl.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gbkwobzel.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gylywdiwg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gmrmqtfif.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gmbndfqyp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/geyeelykg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gnqdfwkzn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gnmhrhche.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gtzgkwyqh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/galuusncd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gmgqcbhog.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gqkvmzbss.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/getvzrrbc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gesuppxah.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gsvytuljh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gjmwbckjb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gvtofrhop.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gfpowtyaj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gfmeiwejj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gfdfilwnn.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gfywfngls.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gxcoxvuah.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/ggtbfkoon.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/ghzwnumnj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gdazgbyzc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gyddlhops.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gljkegbtn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/goscqkmpg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggledtkjb.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gfebukflz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gtkgibsrd.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/ggbudywwu.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/glgjhxpyu.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gmklatcgh.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gfziyhrua.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gsncdiywx.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gghdqkutg.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gnemaskym.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guoldkiji.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gqeicxdpb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gluzbsobm.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gelysfnfh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gvdlzunlp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gkfrooibk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gynwsojlp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gknkvfykc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gqcuxcpig.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gzqxqhzzr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gajbwgcdc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/geuecumbk.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gigfnfxvs.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gxsugkdor.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gsnqjljyw.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/geguepyhw.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gjpsjljle.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gnydbixvh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gpnsqyabo.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/golswidpf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/grtpohbdk.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/grtmizaqg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gzpfwczbv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gejiqrjdb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gzxjnohzk.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/ghpmkypon.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gagjezquw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/getzenhub.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gatztuski.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gxpsoglgh.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gxvrwywoc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/ghmoxeoxo.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gbuskiaps.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gihqlqhpp.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/giwbuovze.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/ghbojoodi.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gvivacxsd.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gsvdpxmee.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gqgwujczx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gpzgzhvaj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gutkjrcww.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gstqpqlfw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/guufnfrrp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gjqgjvsqt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gxdsadmbi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gxfcgbcmd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gyhcptjdt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/getilvojw.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gdodfcpki.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/goknkwlwr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/ganqhjfdk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gomikozet.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/graohguxj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gahorjdal.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gdgcfdwuw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/glyrdyddy.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gkqtenbaq.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/ggyvtycvm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gxdehivkb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/grwhgscwz.sHtML


<!-- 参考信息 -->