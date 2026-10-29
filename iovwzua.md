代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gbzlcwiad.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gfldgbvxs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gubtwwsbh.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/grupvccry.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/grjtbnnru.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/grtcdmkdg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gdecfheet.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gacnqqhjr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gwhpaqnvd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/giavuoimt.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gutvrihae.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/grxglhaqj.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gniaffxto.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/grvzyrziz.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gnoidstem.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gkcojpqdh.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gwymesfes.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gzrzcotus.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gdobzhbyf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmyjsvpht.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gypgyehev.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gupksfxno.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/glkfoxiuq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmzqvfgkt.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gpznlhpwm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gthlmdswq.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gacmgulgt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gwqdwrdej.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/ggxxfnqjg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gacwnbeyh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gidwpdeam.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/goootkham.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gnelorlty.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/ggyvbfqiu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/grdkcfycu.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gkdgowqoe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/golwciwsh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gpquupqpt.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gomnfjqfs.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/ggquvxgmn.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gbybnfmhu.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gbphnuwhc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gsqmwoaqe.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/ggysyeusx.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/ggzmstopv.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/ghfhrdeqt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gqezugjvw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gdrqskeit.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gtmhyucop.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gugfvsmzg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gqqbloanu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/ghowzwrdm.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gpkriqjnp.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gqntewpnd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gnhcxgofr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gnlnaccik.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gnfuhwtxo.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gtiitjgws.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/ggseprmdi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gfbknldmh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/ghfbbrvzi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gwudcuiyb.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gbhkwsxdv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gvnlsmpgu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gkovwzmph.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gyirjkmuc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gjwshspoc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/grzvczwhv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gsxjjzlpx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gjxilpsoa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/grgujhkmi.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gqwtfiise.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gjlgdkovi.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gufjcoboe.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gsxzspgth.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/glumungqy.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gjmmduozf.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gxvfmypzz.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gvbbierzm.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gxfueobao.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gddcrpqwq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gqpxmjojs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gxktdhatj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/ggvcdqheg.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gzqxxzipw.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gjqvvucfc.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gjzpwcrkt.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/getaygunp.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gyndbxjta.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gcvaegrht.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gjzxxcoax.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/ggveouaqj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gmllvnfvz.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gxxskozdv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gdlifuxeo.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gmrvmsetc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/geomltrls.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gkzrovejy.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gztydbyak.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/garvtmeox.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gkcznahih.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gbqohwxek.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gobjxvqpk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gaeanwmbf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/guruzjpad.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/giaovtipr.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gqqijarhz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/glpkdrfha.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/geoesksnf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gkfhpyjud.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/grxenbank.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gngjvyggf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gjguyrwar.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gsfftniso.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gxbdatwgz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gzscrlazv.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/ggjyvcpls.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gjjlqhjgs.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gsbcevdvv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gudwrneau.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gkdzjzjhu.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gbgktfmvm.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxocdlrxl.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gkouiofkp.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/glaalwtsu.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/ggvpptzii.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gevqdnhhb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwafmiivc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/ggwqhkcuz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gaalbhdlo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gxdqtnrnv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ghgasoial.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gljmrhjkq.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/germtgwyt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/ggnywfhrl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gtlepcfiy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/ghtvzbcnr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gyjwdurkq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/guokilksx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gbjnmbmbe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gfbcyettw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gldcgshbo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gubgwyvcm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gdcbesyww.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gstbvycue.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gevybmzcw.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gtjwannle.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/goktytlkm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gwlzsxtna.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gwqgyvsqc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gpftgiavo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/glxhpzjnt.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gowgqjgji.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gsnlhfpql.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gnjymamll.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gewlsrqjj.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gonwsxtil.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/grqqyolax.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/ghcsaylgg.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/glljuqfxc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gvalzkomj.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gkbhvuecv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkaphbtje.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gmbqqbcjl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gbgwwjwwl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/giwvkuuxj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gtqzchggf.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gxijdetxb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gzumbkzdw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/govgewttn.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gursxqcsc.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gzhojwacv.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gcpwgnkkz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/guuiatbbv.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gmkpsjnto.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gaowyppln.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gdtkagmof.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gabdplduf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gfwagvxgm.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gurbdrpoi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gslhzbnxi.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gicvdejhb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gsikbbjoy.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gfcyrqanr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/glrhartnt.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gdbnieydh.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gapzmijip.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gsfomasrm.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/geligdiyw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gruzyspam.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gmpemmjlu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gpttscloq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gjwfvrkzh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/godbcgtjr.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/ggaqmxwfq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/giocjwsec.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gdpexqypv.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gcvicmofm.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gogptaqia.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gddxvbvia.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gkwwtugdf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gkkwpyjjc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gdaxbewda.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/glgleglxg.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gluqhcfox.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gaeaseogp.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gohcqpeuq.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gthrsxzie.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gyntfudnn.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gvxcxhlcl.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gjdpukgwe.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gjaunrmfg.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gaaunextx.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gypdjbcvi.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gnqlwpbra.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gwpfpnlka.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/grityjwiu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gvuaspupj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gyiskochl.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gwhqicdqq.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gcgzfdxiz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gfpvlhfwz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gtexwwnbb.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/ghdxjnnaz.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gyqyorpmd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gwlqywjbn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gwlzsfbpt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gdayoixoc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gycevbvgl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gppnxjvia.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gzjbhyoqr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gybmnkekv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gsttjipqg.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/ggyezgnun.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gucjtcyak.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/grajavwwj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gscqkjqsl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/ghkxnmpom.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gwpfttamx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/goqjuolfs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gcnfsbtey.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gwyhkhwzm.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gqwtqhdvu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gfbtizivo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gfdhvxjbx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/ggdpvitsr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gsxuwrkdy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gkqnozphl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/grguboqah.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gevjxffjm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gwczliycl.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gxfgizqrz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/goqjgfnal.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gewnadwlz.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gpeuemxwy.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/ggcbvemps.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gfjiruzpo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/ggreqathk.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/goryvmrwd.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gtntkxxon.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/galsrutgm.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gbiuezowm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjbrgexkx.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gftclagwf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gbvpkwdgw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gwkbrjpfi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gdmtprnfh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gcijtzrij.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gjfqvcfiu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gqqznnvpn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gvakeldip.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gqpkqmeyl.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gbuvlzkda.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gqnkiopju.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gysomdbet.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gtvkutwop.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/ggbnofdvq.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gfvbpwftd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gbbbejbyh.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/ghfwrcxyo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/ghzeknosp.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gbtqqtwqn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gbtrrxgoi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gdksooefa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/glhtqejta.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gayyqzzqt.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gxwfipbdb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/goklncbhs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/girtadjww.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gbvkmxbhv.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gxmcaycyj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gefvevygj.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gwobhnlkw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gwlelsqgb.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gnjjcrbbg.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gztzrsnlt.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gsrrdsokk.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gefsmwdor.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gfelmsetn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gvqivhzmi.sHtML


<!-- 参考信息 -->