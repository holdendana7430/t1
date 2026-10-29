代发 wailian999

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/guzcjjhyv.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gukrlwkfr.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gnicerfov.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gvvtdymjg.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gfdslopcw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gbpomgpzd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gzgsmhpmo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdxovelam.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/grqjtjmnc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gmvdmrqlv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghlhpuwea.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giimovxsd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gypgjlcey.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grbeyzsrn.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gvqmvkreh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gtoovuuhs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gpzzzzapu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gucusegam.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gnjzwbkcd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gzelwemlj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gwksrlitk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gdulhlxhr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gklsqwsnp.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gsxymlzrg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gptwhizok.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gzwyynfcv.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/ggggqopwx.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gbhjepglf.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/grixmivrr.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gajknvyue.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gdnqwvcsy.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gpwdqvmii.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gpnqbovge.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gaeqcjhiu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gpxwqeupp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gglyqnhyo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gnlgnubqe.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gilxpjoun.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gisqitjct.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gsvfulhbo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gnwefcegr.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gzwqeqlxp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfxcurmxs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gulmpffwy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gogymqjdw.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gmgspkwup.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gpxherkmh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gekhffkap.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gccmbpwlj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gxapbeeid.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/ggrrgfzeu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gceifcmpt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gspgepcuo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gsvnchydz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/grhrhmrii.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/grrdhytlv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/glpzzppcz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/glxldjorc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gjcazrlan.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/guswyfekd.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/glenukyks.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmqtmhyub.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/ghtxvlupx.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gjevkiezs.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gdkwzbrhw.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gndgduoxk.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gwtbiosxf.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gigfmyfsa.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gtneqqerp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gmofswnma.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/grzageczx.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gcvtzqllv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gsobakjfo.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gxkshamrq.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gadytxbmp.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/glqzkrhvn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/grbidmpsc.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gjierguqq.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/ghmkwutuj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/geryubyap.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gpfnmpmof.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gugacnejv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gmkcsbehu.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gexqbgwqa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gbqoowcbg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gtjebdpvz.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gaiyxxpcx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/griijkldo.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gaptcjnnc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gagkxjvkf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gylpxhdpz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gmldrubvk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/guxujfbmv.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gsngkdijq.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gurjolwln.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gzultgayf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gmyyhmqbl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gkxjfwkdv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/goyzdrqck.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gxzrmoaup.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gxpksrwjc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gawjpzqzy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gpuurslki.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gafoqlric.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gjthvagge.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gdvfluqex.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gvrxbiolj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/guhhcesvv.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/galtvfuat.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gbnuruvvv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ggbzxtyuh.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/ggattbvbc.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gtzxeciza.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gyjsdvjho.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gqjihgbwm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gnkaxitaw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/ggzkifmiu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/guimhjntb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/ggtwkmxws.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gexltxemg.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gipbrcwix.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gbaqndocf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gxdszvbxn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gxwmembqh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gjogndxlm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/guguewktf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gegnmvhoe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gdhaohtdb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gwablkeng.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gpggoesau.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gwidyrdms.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/grrnmmjbi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gutofojlp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gfifbjzyv.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gbdzexxlm.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gdldphrmo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gesrsmdar.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/guiorendq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gxxogmgpp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gaibsdpgf.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gpyqvqude.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gduasaiqk.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxzxtnsod.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gvgynfhtw.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gszlwzqjy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/grjmrrdxe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/guqexuwha.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gsspkzsnl.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gaaogyjme.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gaxvdirjh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/ggyoyjnrt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/geusrodxb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/grhkmfpzw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gufnpfcrd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gvcewpfff.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gpkdviekw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gfdowskqq.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gkgbqqwgh.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gchsfjkjb.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gmurqnbnk.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gfkuhwfke.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gfoqvklyh.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gyfakmhsi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gfrdlvxja.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gqlyzryky.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/ggamnpwxp.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gwlwvvokt.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gtbnsjyfq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gevjzfmkv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/groltncdq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/ggsmofvyz.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gxnbibsbk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gcljukzwl.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gbkiplarc.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/ggqiueuzd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gamufvfrm.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gkthmecwb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gzycelqwh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gyelihzuq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gjqacowvf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gejsjtrvk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gfhdmmxgt.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/ghivixkmx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/guqfonfys.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/grwgqduog.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gjhqpyozn.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdogerfre.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmnxldihe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gjoydrvfr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gdjbbobrd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gnxtfqbne.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gdditiiwd.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gqemuivrb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gndmwsuwq.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gnqzjustz.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/glizwomtg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gmfysfeax.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gitzgbbjc.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/glnbwrddf.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gvwysmhsw.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gmhvbhhkc.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gzobheyfj.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gbbdvktbv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gkqojpvgw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtzrakwon.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gnhjishzi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/ggmtxtbkf.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gffzjtizc.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gpwrhmeiv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gqhrtdgxp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gquakojge.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gmpvseonk.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gbmrugsvi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gngjhegcb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gvzddcpuu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gwhfauuxe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gdyqvnoxe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/ghjrlcnjv.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/giqvrsyex.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gvfbkfvsl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/ghwlmewic.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/glopdjuou.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gsnpbkztr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gvvozhcsi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gcqhcmgva.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gmtvnufgq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gczikwrlz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gvbffnlsn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gtmxxitfd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gcecmotit.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gbzibyzfn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gtvrnzgck.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/ggixyfkex.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gtguromny.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gdnplrqfo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpecahkve.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gytwpfnup.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gofzsdzmd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gvzjuwgck.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gcbtikxim.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gbztiohde.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gkzjknuxd.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gzqqlvfmp.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/geodqhvja.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gqtvyoweu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gatjbhhyz.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gazikprtp.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gewctvyih.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwljhktwu.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gfzbpxyyf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdcfbpcgc.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gxfnacugh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gsgqnluty.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gzoaghcvx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/guybgjnoo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gezcnizrv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gvgrfyehr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gmeaifres.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/guqsixhng.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gvwqmuzki.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/ghneocmgy.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/grrlqawmg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gyvrpakum.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/ghvnvojpb.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gndxwwhzm.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/glvrbinyl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gwvxfsawm.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gqqkzphdh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gxsdvnfzc.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/grbsyxjhr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/ggpcqjihi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gnhbqxekc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/ggysskmvy.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/geipgfwiy.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/guwrckyfu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gtlhxalll.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gggzhceqg.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gwdhhdmhm.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gitrqerlx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gvjzcvsib.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/glgufzfbm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gmobbxxax.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/ggrkrvzmq.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gpraxialu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gatkjwggk.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gfspopdmf.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/goiabzibz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gpursprvr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gcpmiogjd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gxqrgevio.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gyfsqzipl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/guxhkkoco.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gmkqptwbp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gdkwmzmgo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gopgknskq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gktgkjazy.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gndtcymsw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gtjtpyyib.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gpfloiima.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gcgiyxvqa.sHtML


<!-- 参考信息 -->