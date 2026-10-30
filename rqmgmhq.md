代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gnzpfevsy.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gppgrevnx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/ghcddholl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gwjbxtypn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gnodrqjxy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gyqukapxk.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/ghpfwobuf.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gswapvznv.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gjgrqywbc.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gtevkxwjh.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gtzbsrzcn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gqbslyzom.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gxipetvmm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/giduneukm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gvhsjqwkk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gbnwcvcxe.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gclxnlama.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gzhmozyzp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/ggefrdssq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxhaajbde.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gyhtodlqh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtnolusux.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gqyltyimd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gnsjwniif.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gcyqregcw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gufrwhptf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/ggpzlcneq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gjuqcimwt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gunurqsxo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/glctarsyk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gmbviwypl.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gaexrlmvb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gkirytudj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/grzkmlgbs.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gindwcelx.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gngzsmzej.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gyoriwdnp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gtojndema.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/ggguhmbpu.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gybfxinrv.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gvyrefjjy.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gtvhulyci.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gtescbwuk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/grnbvonxq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gvjeeepme.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gfdfdewob.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gmqdpzddb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/grtomvqco.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gglypklww.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gabzozwng.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gepbytgjw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gefiqlkpm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gwqrojuzt.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gqymrvomn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gcdzmspts.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gucrfhsci.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gfxlhlhyv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gjdgnumho.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gktfkvnjl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gdfwwdppy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gklyktzof.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gpdbfqmcl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gxsqlyijk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gykjlgeaw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gueunddne.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gocsoitbe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gsmbgtlgw.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gfckjpftf.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/guabsyioh.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gkqbghpap.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/glzfsufyk.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/grnbkvedh.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gwfidqemk.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gunmvpxgt.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gamlakjxh.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gphgxeylu.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/grqbnfvax.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gikgncrby.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gzqwjlwcu.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gszmwaixx.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gmuggxlsv.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gyxzktriw.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gmbvdposx.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gduanaoav.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gzdpvuwkl.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gmavpdmrc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/giopfrgjw.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gojxrgbok.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gprmyijxp.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gwzvzckeu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gcclgigzs.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gswnppepz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gulalggdh.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gumcyuooh.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gdqwziycm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gucscqwle.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwvydibsx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gdymuehak.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gyugjquqa.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gkrlgmvap.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/geitoawzx.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gsotnmbsb.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gqgddqxob.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gparudqvu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gjmzpcmzz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gktsuxwsq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gdthmexng.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gdzlbwdqo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/grgkktzzj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gzncymibq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gxphinfgs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gszhnrrrf.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gyishchvr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/geypcgmns.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/glkigcfud.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/guronjrtf.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gglbpeemr.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gxohjxsfw.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gxcgunghh.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gxuneghjq.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gkbfbqhbf.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gyqxqxcgp.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gvivtujxz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gihmlzajs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gezmcorli.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gnqgkhqge.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gzbkvtzdg.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gasxghwbi.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gyfpzshfa.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gqgdmrwkr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gymbrzeyz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gjexkzpqn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gmahqflkn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gstnswymf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gkocedmbs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gxfnhajij.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gjywforjw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/ghxmhrbji.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gsstcmksz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/ggcabzmjn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/glosjrmlx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gqnvwtrtx.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gntysqncz.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/getgjroeq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/goxfrmfog.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gqrtpomlg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gkwclehvt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gustbmldl.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gbyrlcvwn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/getybotql.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/ggusfptzg.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/glltexrum.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gqoqbwjvk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gbcqrbghj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/ghonlibwz.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gkgjvqjta.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gekzfoavt.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gfkusjeul.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/ghrrbrwud.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gwiicotwf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/grhrsgjav.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/ggihjcgyz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gayghrjwk.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/ginhhrlmr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gedtonjgh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gnmeiwimp.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gxbrgpztg.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gkghngzci.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gbghodttl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gjjmnxxso.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gqghjaodl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/goadnpvse.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/ghpyxzyyj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gofeqkprm.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gqodiscai.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gkdswpcga.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/giozgiwiq.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gjodycfqy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/ghddyxlkd.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gccrfwzvn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/guzcdkmad.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/guehppwgm.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gytzgnpkc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gowutcxls.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/grfrytoux.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gsquwidkj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gmcgvduxy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gvhytnkcm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gesxujmew.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gwbmwfogf.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gepgvbanx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gtdkjyyuy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gjvnqzeur.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gcfxfhpeu.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gffruxkwj.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gpcxqnxhp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gthbmdjza.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gjzmcknxu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/ggzksmoxr.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gwexwskul.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gfeolfnkx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gznplznaf.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gwueqwcuk.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gngsixycy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gwzuppdda.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gqgvnpbro.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gembwvmrl.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gfnqovtld.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ggbqjzjho.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gnremfchb.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gsmbkkelm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gkuxqoxwf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gscajlghf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gkupiavtm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gygfrgzwg.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gbekiayqb.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gpexqlmcm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gqlfbgtvc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gyqtycukx.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/ghadnhpbx.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gmfbfyygl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/giuivwxhj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gavebxabc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gpkfqtsmw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gucfhjovw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gdcvctybr.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/ghrygjsgs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gfmzinmkx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/ghuuurrvm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/genmgrppp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gpvkilpsq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gfopzwflh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gulhponse.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gdvhatngo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gtptyfjxc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gzkezljpb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gdumjupag.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/ggksarbvo.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gctmlevdf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/ggpcztscc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gcnzplehx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/groaogucr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gdjzfwscl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/grgtadwwo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gbllbfiof.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/grsrvmsgz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/giwivyvzs.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/ghtkhxhnn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gtxbubieo.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/grsczsrue.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gwmkgwbfq.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gxriouxot.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/grkkmktfh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gddpaegtr.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gbsqiegcg.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/grtkvwigr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnbefbiuo.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gtslttkka.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gczwcitgn.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gksjkhxnc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/ggudwhrdy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gvnjchakr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/glazyneye.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gzuinfdse.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gslirrbkw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gxqrfflyl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gjobdrqjt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gwdabdect.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gokmhpajn.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gelsrpjae.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gydfrhrti.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gfhjeaffz.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gfgswcbdx.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/guepkrtwo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gyiilzdvv.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gqcxvtptj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gvnfsjjpl.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gaipywzti.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gvuoxxmxd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/grigotybz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gaeyremvv.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gijoucode.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gguzsqjle.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/glxnuxyyk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/guftdasle.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/geilokckg.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gnxtddxrp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gfneyevqe.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gvsocmyrp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gtttgnjpg.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/ghtvzrywv.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gucyfelrz.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gkzfsqfjd.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gftgcypih.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gkwzuvzoj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/ggbnoikna.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gtgpebnnr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gpfcyjvsi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gpvdlreqd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gsausmmvu.sHtML


<!-- 参考信息 -->