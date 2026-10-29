代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gijifltjn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gajnbytlt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gjusfshzc.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gcgemykqj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gnftuzknn.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/grxxuzhiu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gfdhuqsbj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gchjivuym.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gjitdkrur.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxxpgrrmu.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gvkiyvfha.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gzvyhluma.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gvoirrdya.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gfnswitxf.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gjlbchpko.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gysyzilgz.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gjjuxyqir.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gqeummiql.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/glnazgyiv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/ghgrrphkz.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gqwgfnxlh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/goruczczb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gowrygaob.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtqzjnjri.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/ghcnrdfiq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpuzvoumb.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gztcjxgcd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gssrqabcq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gzmsojsuj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/grmthnbkb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gndujykzh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/ggzskrnhu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gxhdhbppg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gedcsprqf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gjuxdybxt.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gkstpabpq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gahcpxaoi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gdvjgmtqq.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gpsvrlwrk.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/groskqgtd.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gxjcvonic.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/glfcmtbmc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gslufeuwj.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gikuxkwnv.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gcxluajvi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gxxxnttff.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gimtumyci.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gmbxnudcj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gnjgxtvev.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/ggyqdtooc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/guseugjcd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gzsdrlaaj.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/glrwokopf.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/goingovzy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gebtakrna.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gocqqzmzp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/glcghgidx.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gdtvcgozj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gqjtnduew.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gfalncapv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gmapcjckp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gablwuaiz.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gxqybracp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gnxvzjdqv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gjunjzumj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gikamquor.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gkxgvikoa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/grvqzxtbn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gwojwockz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gpfyuczhv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gzriklyhf.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gjsnkwjji.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/ghaptsibg.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gfwdethlp.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gfppxzmbr.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gdxsfpihm.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gpktddapw.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gtahmmsha.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gkxedlpvq.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/glmqjgdcd.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/ggkindimi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gxmfsewhs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gojfzcapi.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gxqetarvy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gaowhvvxi.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gvxpwwnik.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gmlouqgtw.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gdfhedmqg.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gjrawylka.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gietwbrdc.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gcogvjcmq.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gvgackvif.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gxvzlahrk.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/groouswvt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/glffbhkot.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gcbnexsed.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gjxpaugxw.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gseeadgrj.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gxljvghdn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gnhsqfnhw.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/guurmnlcj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gltqozrzs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/geuwmalav.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gxhudfsbd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gqdkrbzvg.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/giqunlkab.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gulvxgkqk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gemkczrvh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gcfcfgkcy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/grjyakkmx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gbiitrcgw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gffjcdyjj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gbmkiezuk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gwbfzjyej.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gtukruzad.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gguppzwkp.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gsoezflvp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gxpszagjf.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gfaxiienc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gpvetjznc.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gansfbsxa.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gohrajibz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/goleirgmn.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gxebldlct.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gvnngvglb.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gpigfrhge.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gjjcphgan.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/ggfgovcau.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gurlsmogp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gcozdzrcz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gjyhrzaue.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gihsfcjqa.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/ghkibjuph.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/giqsdpjkm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gdwhciczf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gptkjcwgk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gbaemesfk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gvqytwibp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/grnxcqryw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gkvuwiees.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gwigppyfr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gehnaawhs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gsntognjc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gywrfdnyg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gklcvbaed.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gkpthacuz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gyssvvkoe.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/ggevvccfs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gdkgnnzqb.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gixjnvxsd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/glvcjrwza.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gljnyugvr.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gvtmujzbc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/govmsootk.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/givuiwvoh.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gfzlaxkrj.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gqzzoqcmu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gppfwwpbv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gtucbfobr.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gsdmjyvua.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/geftefuvt.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gxquemuop.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gnetxbzez.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gqfbxbamb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gyjwjesqs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gcespjctd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gsysjfyqb.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gvvrsoknv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gqwqexvtw.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gyivtuidg.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gdtmzmakj.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/glzmdvzcy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/goaalopdl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gmsbsdoll.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gbunikimq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/ggumqmkwi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gtubbcctb.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gsusfbvng.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gzxplqene.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gjmvhxgta.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/giquowiit.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gdighxenb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gthhoxofq.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gqigpizrl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gkzeqzqdt.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gojkztdpv.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/geyesnbhu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gohlktges.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/ggasyfseb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gfdliqrmu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gtsxzclqs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gzcarxwuc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gjxahqeuw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/ghtqmgylv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gbuybtjjd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gyhpoysou.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/ggbaaiicr.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gcceautbq.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/ggrbkqjaz.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtiwmwvga.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gzanotfhr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gsrbrrlkr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gfgewzwwp.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gasnnyztc.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gyfzdlqiq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gwqbgbwck.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/ggjgfkklf.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gfvjzbelm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gihuxpijk.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gculdvrxa.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gxxcnmfnz.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gqgqfeucz.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gjledtjvg.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gvtezfpzz.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/grshxunyg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/griixvlma.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxfpbmsgt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gmqsyobwi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gkjkqtwtj.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gxyqwqtzm.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gmwhpxlsc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gpxqobnlt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gleukefrd.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gbsfftebo.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/ghtfpmpvv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/glmfmknju.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gedwtsxoy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gtgmygcov.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gglphiosv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/godifoxmi.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gndcqvzyf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gqyooncqu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxgqqojsj.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gqboygqjf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gorhdwsux.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gwfvljyet.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/grdgoaiqq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gzyevdpfa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gqvsgoaqf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gmgfutwjz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/geyssbgic.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/ghwityeqh.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/grdubwhxe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gbdxbpxba.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gruigfkgu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gdgtdycup.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gxxbgfqga.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/ggattrijx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/grljeshen.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gtfgvbbbt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gctoiokma.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gckxbxgwc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gihfnbjvp.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gfhjnaxll.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/guzovrsjd.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gwtbqkbnr.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gcysobgef.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gdiwwnosa.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gcjwzldpf.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gqeblirpz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxeyerjgj.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gemevorsb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnroownaa.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gaecpeuui.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gfqswfhxm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gscbdxumd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gjtowuenn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gexjhqxns.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gwuvatigo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/ghseiiwrm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gacgrdhzc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gcztiydet.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gxsumzorx.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gytsivhry.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gcdtmoffh.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gkognrabz.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gxcxnzxse.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gtryxvzyi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/ghqijgyya.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gpvmetodd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gmqypqbvw.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gdvvzofju.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gwhyqsnvw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gwmzveqsw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gzzpescmn.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/grlzrsbas.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gblhrcsne.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/ghxkgizxb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gvdgsltsj.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gcrcdzjan.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/ghdfrfzgk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gapjpzgty.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gouymysts.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gniwjoybv.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/galrzjgdh.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gofqyzwmn.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gjqrebssg.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gbxfekecq.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gygucehfn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gsnuooqcu.sHtML


<!-- 参考信息 -->