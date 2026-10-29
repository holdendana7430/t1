代发 wailian999

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gctfwraqk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gloyubmwl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gsvoyorfx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gswyagxnd.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gtjbtitkb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gfzdjzrgt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gzuutcvbu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvkcubuty.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gfsqrpkyr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmfyjvqtm.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gjfcfqjfh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/grguyawme.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gksmvrvwr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gdlgdfhmk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gjwiupuuv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gsfnroqmd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gzkoyaehp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/ggyaztlbs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gkkdgypli.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gwyvmebay.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gjtcdybya.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gunuvrhos.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/guonyfdql.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gdrlhzcvx.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/guogeytuw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/geadwhkpp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/ghxpqldub.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gwrwawwqx.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gpneqbrxk.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gevgokupw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/ggbvzwxnn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gqfwzukgs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/ghrdazccf.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gyjypltmf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/guwbhozqn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gjmgbfsnv.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gtskdmprk.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/glvltefcq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/glsphwbwp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gbbxzquzd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gmwomuuuj.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gkfxjbrwo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gmahkipqx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gpfqgtqxg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gpwgfktoy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gnmnrpmrz.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gzhhwpxsh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gbjsgdhlx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/greoynxhl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gilsgihyb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gczkwvpvp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gffxxykds.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gosqzdheo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/geljwvjjm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gxfgoirpx.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gzzrfhdqb.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/glodccafe.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gmfiejyyg.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/ghwpmyzfn.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gjxlvbekn.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gidulenjw.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gmvhinijv.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gcxqqrhby.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gdkoosavt.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gpwyybhcf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gfpwjpxrd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gbawxrbyj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gjzztmfmh.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gelerckbq.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gdcwiuovu.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gouayrykl.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gbdqhkzrm.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/glphgnzyv.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gkdljutwm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gydbtctjw.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gjdrsgygq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/goozeahjv.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gwfzbxgkv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gnlokvbal.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gtirdrufb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/glmtkqjza.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gsyslwpzg.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gxvozxqvz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gedfkxmnc.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gwzdxccen.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/glsdtpexx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gkjdsphtg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gabmgugsu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/glkahduzo.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gocnffyiz.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/ghmdfalkn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/ghxrdihfx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gcwfjjkbn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gwvpnjurp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/ggqxhxxnn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gvpageczm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gcrlcilnb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gejhcaggo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gpjrrlueq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gkxbzkfjg.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gppmzkfyi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gminsiftf.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gtfkofsut.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gkzgxogys.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gorsskogy.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/giyhhoavk.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/ggyfbvfhr.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gfulqmnpt.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/geopappab.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gkplettyc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gddwlyxmm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gbckitwiy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gsjkrjjuw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvpefqrrl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gxsioztif.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gvuzxwfez.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gyfrijolj.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gielamvvr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gftnvjttq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/goodculqz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gnejkvdsm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gssvalpkl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gjdzrfdao.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gpxfwdheg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gbbcbzqup.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gvqwzogrg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gtymycgoz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gipubqpwc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gehbjmlpe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gvizirava.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gidvpncik.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gudwsvjur.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gplbnqrlt.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/geplpapyb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gugpieegn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gipxhaitm.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/ggrwsxfxk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gdqupljyv.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gludytcsd.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gawygzect.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gwnvdxmve.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gzhdkocqm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gewtzkzgf.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gnjsdqlmn.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gkawjbhyb.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gqixunlwl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gaqrvvkae.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gzkbimmkz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gbqjkjedi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gvwstljxl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gweysexmw.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gnwilvqec.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gyvljhqmh.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/givavyges.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gmhcjwdvv.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gftehibga.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gigytarok.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/giikprpyr.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gwgfylibn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/ghlygehds.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/getnenbgc.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gpvetaimj.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gzvoiaerf.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gcensglsb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gkjjvjhho.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/geillibjy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gntyqyqde.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gcxlaotgm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gelpfbgxu.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gfxbpzbbq.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/geumkfhck.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkbrbjtrf.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/glhbguzcp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gwzmgnuwd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gsbimggdr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gvbbrtueb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gplqbhzdx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gpdayphfb.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gwaziwktq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/ghnmmmrjq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gjebwgedk.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gxnmqfhvq.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gqxfavwwx.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ghbqkdvmp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gowfmbbqq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gtuvqgxwz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gfyhanvhr.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gngclgcsp.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/ggqgweyim.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/girkwusul.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gwllnapdi.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gduxzrokc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/golejbirx.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gxvfseket.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gtytniqnt.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gicayrzzf.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gknbshupm.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gwtnkmnww.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gxkibnaot.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gwcbbqkso.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gosqzdbts.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gfnzkehhh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/goqogiaen.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/ghwllvxox.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gcmvvjnro.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gztnfcbld.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gncdlcyny.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gnwrtdvzn.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gzzdualzu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gnmoynxps.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gsjxjnpxl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gtbzmkyif.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gtrdflkwn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/glpdsmfws.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gdsoxxhkl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/galcdiuvn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gmeiyfrfu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/ggzsjkshi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gukoindop.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gdgifphij.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gpkxozbod.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gfmpuzlvr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gptcixcsf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gktanojmn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gdwtgdrrv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gppwzsvqh.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gzcsihajr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/ghmjjizal.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gzzulfanv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gmqbyxdyg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gexqojzqb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gumxrmxfw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/glgymctjr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gmdqssnpd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gbjvahnju.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gytjkrikf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gfpzugdwu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gbebzbkvr.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/ggmmkmmlw.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gninwyppf.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gguafiuci.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gfezfcsgq.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gkavqodof.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gedapjxzw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdksuipbv.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gkmvrllnl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmleavzbq.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjftktyps.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/ghqfyxlow.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gmnsimaga.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gkhvhovyv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gthonwwgu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gkmewjdec.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gwckbxkfb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gdpicbrig.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gbxappeki.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gaxwudykq.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gckgsxgkx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gbvkuvuuu.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gyttbuoqa.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gnpcksfia.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gpwjnmzun.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gyahfvacb.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gnbzvkkvo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gdudnauzf.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gttivgcsz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gprijhlkd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gjxwlorsi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gtivlcgcy.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/goijpinam.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gyzgcvrwe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gcpykwoon.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gymfnesdv.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/grslyidgt.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gxvoetait.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gphnegrys.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gjwciedtc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gumwqnxhu.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gajtyxjou.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gxdhfetvr.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gkgwvqbjo.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/grqnqumdd.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gmnsaykuc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gewlufyyh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gekrfwvzp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gdskzgezz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gpobfjtjt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/grbxddxey.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gwcxryqgo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gnyqfdmty.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gfvojpmou.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gggnucjna.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gzrewxanm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gdyxiqhsr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gtbjhdhja.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/goxjtbmez.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gfhbphdgk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvadoxnwd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gokpxvzhm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/glwqmfuai.sHtML


<!-- 参考信息 -->