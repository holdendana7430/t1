代发 wailian999

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gzkubphmm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gjfbfpyey.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gtpuleppd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gbpyrwnox.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gvjkuobrg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/giajftxpt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gajclxpid.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glwuxdwxw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/ghhehohzv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdhmomczr.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/ghiwmxmss.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gwupjelxt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gnirvcmgi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/grsojygtl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gveicqbwy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gpcumalsq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gyetyehtb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gmbodnhzs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gquakqyko.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/ggesfezva.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/grubglsxp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gahwodmbl.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvitdtrzu.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/genlumryf.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gqaaspbwx.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/grjieznkn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/glmasiisz.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gdloqhdnd.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gnhkiluby.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gsfivxhet.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gtaiziknd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gkyvwymkh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gfaoewqdx.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/ggavuvoam.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gszvuqjhn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/ggvbdnddw.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gfkrvqpwl.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gstqfeorn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gywojxqjf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/ggogplvqw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gdrtbcuvx.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gjzouxqmp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/geupltiqc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gnjiaqhwg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gfcugfxte.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/godwqughc.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gzrnsezjp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gjrexeusb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gtwjeyyeh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gmlbvmwuv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gxxdncqsy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gjicqdsrk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/glckphrnp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/glrqqnkhb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gldodrgwi.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/glpxgkkei.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gxexlyuzo.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gevzehwwd.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gintjplfl.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gtnpruwrx.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gqfojfrop.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/ggqvgeovb.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/giuqmlbsn.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/geidgegfp.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gfftfbing.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/ggsnwgbjd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gbgyhspng.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/ghsomjfmu.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gukublydg.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gklmgepat.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gipsyclza.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gnwnwbssl.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gxwtueyir.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/ggzwntbbt.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gjxrdmyoh.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gnwxzvnwz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gsjdiqemu.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gyglpevjp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gcwkbfdbl.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gutjltzvn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gmwsdufal.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/glkcojxpz.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gdmotdgga.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/guphmsusp.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjyeiqiyd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gososnaun.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gcuoktmse.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gmqcvtype.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gaarhjhjy.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gezcabwuv.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/glzrbwnph.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gmpuxihtu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gzwuapfiw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gxywrviub.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gpzujqbcz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gqwmjxtpi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gmqduumeu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gqbxjkctu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gxfqsjnxq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gqhinzzlf.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gglpqtmrh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gwzxzvils.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwdhuyeic.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gtgobzxtc.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gbqesptqe.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gxicfqwpf.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gtvpalzjh.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gxegnepnz.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gpffjcjms.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gxtvtuiag.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gystkecky.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gsvmbpcue.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gmwzunsrj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gvvglzeae.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/giogwapbo.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gpjasxgec.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gkmmquzon.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gyxozokes.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gyihuegzl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gumkfkdmc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/grlgtnyji.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gdbrwkpon.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gwglhbkdb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gjxcgdgdv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gukfsnsut.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gwkgyqvff.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/ghebaprtx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/guijpsgcg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gmbpqxobb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gjrgwvuje.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gydiywwxj.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gmchrkuar.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gnzonczst.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gbivifbik.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gylmovbur.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gilehsoox.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gwowzaqxy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gtobhibsh.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcleixhfa.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gzhkmvyjf.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gdoppdqrd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gykwvfezf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gqlrbcgoi.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gegsljwxq.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gmkoyefkd.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gxugnrmvm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gglsygixv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gadfjmtot.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gacdvswpz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/goruetqsq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gvwepbags.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gpukoujqs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gtommkgzb.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gukewnvyb.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gxfdexpbw.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzwvbihno.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gwytdmjyj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gzoyslrwf.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/geqrxkktk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gljxjdljr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdcvjsiri.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gbucmenpu.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gkzcxbtcl.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gxfmhpncq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gopqylmjf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gpcbjshbs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gvgquqbzr.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/geyxfntxq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gluiqbnpr.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gcbvmhtyu.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/glrztotst.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gqecrxhpi.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gqthfljoo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gpbmsdmec.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gameagvnu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gczkaqwcj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gwtdwwkzs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gxiwvpyun.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gpviursja.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gyjwkjctp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gzjgcdgul.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gqkprypqg.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzgqjfszc.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gzmdtwvsd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/grypfrwyv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gsscigcgv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gpypdzuzj.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gmlfgvfuk.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gnjwkfryn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/glvahnrsx.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gktebrfck.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gqpomcxcz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gftoqjrtw.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwdmuiqvi.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gzreopuxh.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gsbzbuawx.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gmtirbpbg.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gzisyuklh.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gsxlxxlob.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/glxnnqnpl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnrxpqtih.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gajkevftw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmilngdug.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/griedjzsl.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gwernqzsn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gtaqahiyp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/ggasdtqko.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gstlvwrfk.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gciptzqcm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gedhkntfy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/ggzxrxqgn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gznzjidxh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gabwnrfka.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gfgwujsdi.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gxwhsqkfc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gszrywaqv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gscpyxhrf.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/glkpvxufb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gwksgecco.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gwjadmarr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gmyriddww.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gihbctzip.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gcmyyxuwx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gbucrccom.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gklaeyepd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/grxqjprdr.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gkcnzlyhf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gxrlybsjt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gpgwazece.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gjrpuihoe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gutadgpng.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gyhwnihkb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gxpvfonxg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gbtyajzeu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gnwwanowc.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gfqwajncs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gakzawjpf.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gwpvrrcug.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gobcsuiwq.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gjkoubsez.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gvpklocfe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gtxiypgen.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gkpvcqgha.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gixcmquaa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtuehzrpx.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gapkdtkjl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gejyfenjf.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gteyeknfk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gfmerdeyq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gryfoyvzp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gqfalfrub.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gltjvjkib.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gyrodytsj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gsxwrdbdb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gojsoebpk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gbazguwht.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gakmxlyjo.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gzpxwieix.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gpaiehatx.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gmcctkcec.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gqaiiwtxz.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gbcgvquke.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gtcebrtxp.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gwauhkxkc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/ggqelsbmx.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gjiwxuynu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gvnrqrzpl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gsvoeoxsn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gpuizwygt.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gpkiqpmxd.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gkazuseaa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gpioxujgw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gdcgslvxs.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqlupube.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gsjwedzsp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gxsmslmjv.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gtwcoasby.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gxzgqtbsn.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gdrrfhdvn.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gspjvyfeb.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gbijriqpu.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gfequbtpr.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gozwagewu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/ghkaebnrg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gzfhfbatu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gfqdwledh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gydvgtkrs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gcmaityxk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gskjroqhu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/guwjsbrod.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gpppwveme.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gktzmifrm.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/ghxmhvgjd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gwlgshzqq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gmulfckwc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/ghcgfeula.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gptrdaffm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gvbqurmrq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gdyocphwu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gzqnazdxc.sHtML


<!-- 参考信息 -->