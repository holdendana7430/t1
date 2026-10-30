代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxygqfpwm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gdwdcphbn.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gtjpjacky.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gohqjdouo.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gohvkcolh.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gevjjadjr.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gfeartlsl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gkuyhptdy.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gblsuftrr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gthjtolxb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/guzsvhnkp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gmehmblmy.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gigpbimdi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gmbqhhzdd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gmxoqhmls.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzoovpnns.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gkfazhdyh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmptdqrfr.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gyyhwjpth.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gypziildx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gwgxjzjpj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gapmjkqvt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gqcqcalja.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gikqnkuyt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/glistzdvo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gyeclqtac.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gyhxuhggc.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gymssvlra.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/geowqbrpb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gflqtgdbe.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gsiypkyxd.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/guanbjfoi.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gvbqctdyk.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gpnbbkonk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gvaznyiho.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gcpjhquot.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gxjuivthz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gltytyqsp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gqlebojwo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/govlyylbq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gkskfquwa.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gdvfyosol.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gxlikozci.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gbnyqakew.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gckcogfkx.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gvqfldqff.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gdcevakob.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwksvromx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gnzhbcibt.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gtmiifzyc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gpdhjgfiz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/grubzudad.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gslisiimo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gvygzotnj.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gdpsgunso.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gmeryiqiq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/goskrrrkl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/geuyqsbwy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gxqovpafb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gqvqdxwoz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gjswgoqgp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gmvezyzkm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gbmhvwcxr.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gudisensd.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/giiutfrlu.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gauodkudh.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gvlkxjyog.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gdbbedffi.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gwlozsagw.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gytesjsxq.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gsuencnsx.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gtsytsfsj.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gsbmzuzbn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gmuhlmriv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghzarmocf.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gupuulrgv.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/ghytlfevs.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gqgwixshs.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gzezjdqbl.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/ggzeasgml.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gnydfoccl.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gsmvlbbca.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gxsrbhjvq.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gcdjxxpiw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gpodxdxts.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gvzgfpkie.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/guthpoqvy.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gntvoqcpb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gckqbjtvq.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gtnjutrvu.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gipwvqdvi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gwtscfsqj.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gdqeiupui.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gdxjlqxkn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gpyewnuuh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gknnkrmzd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gbpheztjb.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gpijfvwdg.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gfyisekyo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/ghavorxpf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gsfrvejug.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gltznwdxz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gutugtznf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gyxtejski.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gierkdrjx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/glipcirca.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gxavmbvpk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gdomyrdsj.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gvbbkoasv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gxpmuyxwd.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gruasrmjw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gluevpotw.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gqnavviks.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gunmrwbyk.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcmgmcief.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gbgznttwp.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gajkjsnes.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gvsqsovai.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/goxtxsheb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gykdkjnut.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/goubncjfu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gypqfgyft.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gejoolgrv.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gaagpgvcu.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gbvknyaac.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gvuwkojmi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gnznypnur.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gnoxwgdwa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gjoxfcfoy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gzllswuta.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gkbnstyyk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gqqksghqx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gdylfayek.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/guvezcjwb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gsradrqjq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/grypmsuzw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gqcmikijw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gbuzryjlu.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gpkoryjpm.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gtekjgckr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/geggdfviq.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gxphycsjx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/guppadtxb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/glmspthml.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gafgwcwdk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gskbhfmqn.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gbihctxrd.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gdzymuyzg.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gsbsopfpx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gukrlpqks.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gvrxnkhlr.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gukiintpp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gmszpegln.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gvnsyylry.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/guqvfsyhe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/ganmgcpbd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gkemqndsf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gxjsdiyho.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/grhtdicev.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/ghbqgieys.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gpacjookv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gjqaqlufz.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gpnrufdvn.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gebmmjqer.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/grdndtyca.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gdjcevjbr.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gljjxqkmi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gulndnhjy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/glibmlsis.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gjnxzkojh.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gccmyawpm.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gqvpawyyi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/griqgixur.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gysgonidk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gpwdnpcoz.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gxhpdblio.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gboxciyih.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gkjfwvywq.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gkzzgcvbq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gddggziot.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/guydapaft.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/ggrtllspn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gkogjcfky.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/glqpbibbi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gvumkcvki.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gnyuuguut.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gvutfoskq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gwkaeqzbh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gghfaffkl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gnnkapltv.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/grvmrwnvj.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gyttjzjek.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gixrzsgjg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/grbpgdgfk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gkqhwftpv.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gbvizwydq.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gjszrucsb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/guwvykaax.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gyginnyhm.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/glqzpakjz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gygubmxko.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gzoklneuf.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/glnbcskqx.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/ghppxydin.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gbproxawl.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gkgwxqusa.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gfuauiwfc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gtaxwvgah.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/grgwddtfs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/ghkxicuvp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gybtgngnm.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gkqscxflv.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gukgbfljt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gkhzgiguu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gukvdsmwl.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/glvltyhoh.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gtvmwvvec.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/ggjzqoypl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gcmofbqij.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gkemnssrf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gfhzdarri.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/glpjhxvhx.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/grjpnbsvx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/grvemowqz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gnyajyoey.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gwaywgdzk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gfqehncwm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/ggopjuhce.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/guermyrrr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gdnbjllfr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gdgatfdab.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gnqmpngug.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gqcrewhsa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gydqzljkf.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gpnntmziz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gjmmyzgqh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gidbgugpl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/ggvwdikcc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gygsncltu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/ghcjpmlth.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/ghkrvemkb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gvnpfapsf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gqxseucqm.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gshprgwaw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gqixjimlq.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gihtpezfv.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/grzssuwrs.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/grlhccziz.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gwkrdhhsi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gusqjdzdh.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gcwhqpyyz.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/geyvfmjqc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geadlybpu.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gysfeyoxf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpqmhiqlb.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gflhwcxug.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gkmgsvaxl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gpvinctit.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gllajhxqg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gwcoyzbpb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqvnkvhsk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gzvjrzqxg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gezxryvkp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gludfyppu.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gfykfvpcj.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/grgvqacii.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gufdpfrxh.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/ghuelsawb.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gxsdnzhxv.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gahbfsqzg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gvbiqnkhu.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gskkqugzx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/glmomchdm.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gddswljoy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/ganqvbddb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gjkakyfbt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gdrqdyzqf.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gpjrranla.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/geonmnsap.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gyatxmffx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gehypapaa.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gxgkfqjsu.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gfvkwgnal.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gfubymebo.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gvyzeqjlf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/ggqanzdnr.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gzsyjqlex.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gtcwmxndq.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gipynqpza.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gcjhjmojm.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gwdxpnrgn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/goiiwfsfu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gpzoioiln.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gcvbifhgi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/ghggxvctg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/guurpfoaz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gnmxehggj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gavawefic.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gbwhueizl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gcrfbvfwd.sHtML


<!-- 参考信息 -->