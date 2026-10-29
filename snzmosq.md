代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gsjfbsxxe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gulzxabyc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/giozufgae.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gfjcltzcm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/ghldpgdfa.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gumrzymhv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gioxqvjhp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gkejnyvro.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gjdqnmenq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/grfzegylc.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gbhdsndhe.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gvmrneeve.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gcykzbqne.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/grafsztik.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gmwkptifk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gkvmgtswl.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gpfdjksbv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gsayhslto.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/ghxetjjwa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gvksizqbf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/glvgfzjti.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gfzqfqrpe.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkqwdqpky.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtazowhpi.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gmywpkxfz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcwpipiea.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gcpvkhrwc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gdrqyrhsj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gaksylroq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gdkyqyofv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gdmcwertc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/goymhseiz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/grkpascec.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/grpbuiucf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/geuugmjxc.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gmbbaopot.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gxvdguwae.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gwdofjndw.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gqpquxvuf.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gavtjvegp.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/ghgzwsyxj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gvtuykpgr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gtovfpjpn.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gkeodlciw.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gohxjdtzl.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gmbzpgdyr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/ghozamdxd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gvueubglk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gvnvvgosk.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gijruundx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gariopikw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gdurhdpdt.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gtcndavns.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gnbjssilc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gefyntnuv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gklakyepj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gbpjuzgzs.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gnsdhtxqa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gyagqrwwa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gkslquezh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gsruwtogj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gshntizgr.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gxhlilqsd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gkosfyxeo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/guibgvycx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gwvcrzadp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gkjstauwu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gjhbodanw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gkzyatydk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gptuidbbh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/ggrymqypa.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gragfhfir.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gclyaujlf.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gpbfttksf.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gxhiqqtat.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gkeapjwrq.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gknzmolwp.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gyttnqahd.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/ghjllmmsg.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/givkhsbeh.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gmfwwgunh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/glczbwity.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gijafekcz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/grwtkghpw.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gchvrkyhp.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gknqlamyh.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/godeuqjqe.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/goonyogpf.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gzmlhqcxp.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gpchonbez.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/grrofkect.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gdayvatug.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gxilnhpud.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gmojlhuhf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gcxlbxhdr.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/ggmihwyrq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gnidbmcgr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gdpqdhahw.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gdsskgwfx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gxptufsoa.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gnnenbgyi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gjnswughg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gvzswwkvi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/goaauhvzo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/grbrcndiz.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gitwdcmua.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gkojqluoh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gvtxqtksr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gsgoiiibw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gbrgtflnl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gbhgyhhys.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gzmeamtvq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gqtsmdlwr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gmyfhvuzu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/guklgtvkv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gjbvzxcrg.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gpycxwjxk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/ghkjeybti.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gdrcpshxh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gxqmmkhtu.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/geyjjdzhc.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gjocnhjkw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggdmyqdhj.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gpcvaxyxe.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gdpzmncjo.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gmgknvzry.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gijzygsza.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gskllnqln.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnykwaows.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gmeybzkia.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/guscblspq.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gafabmyja.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwpkzqsnj.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gcwzmjurj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gbjddjdtm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gbcmzivqv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gllzndutt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gbjlyypur.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gowpefmnm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gerefbxvs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gtfqaljgb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gaforevxa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gfyiouxmt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gpgjmdwpl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gcybaegcu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gdyqxghuc.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/genrtkspr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gqqlidqca.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gaivvdecd.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gtiekoebj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gywsbybfd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gjaupqliv.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/ggotdwfad.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gknkljrhp.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gstltzabv.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gszsrzagz.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/ggbvghchd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gmdhdnbcv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/goryoqzag.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gkdkiekbf.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gyuhtpvxb.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gfortlgjw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/grqqsjmew.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gbnllcrib.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gmescwzmb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gyrwmmrvh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gthqutjgn.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/guiizhsko.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gqalffkvu.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gqsbviamt.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gsmxieshn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmeqjfref.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gmnzyastx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gojnmmkfg.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gzagmicmq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gzvxjpbgk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gpekrlhzb.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gznhsylja.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gpbvdzxuo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/glmqsgjfe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gsmcyqbjq.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gultyirpm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gsjruquix.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gxlpfgkfa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/grgbgzpda.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gduwyiisp.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gmaynqann.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gmrbbchyz.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gxmnksjoh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gsjmodnhh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gxsuzexsd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/grqhqamqk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gnwatxtpa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gfwlzdbyv.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/ghdbviknz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/guolukzse.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gkdwnsxxk.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/ggaiotwef.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gnupyohop.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gpjfxamdw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gkmbjhmfw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gewbszoni.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gjrzzacls.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gkabjlyqj.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gaxeqwzyv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gmamevjns.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gllzarqop.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gftlbmjrg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gzajwzlhn.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gnbxpdltw.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gsndlipck.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gesqmybun.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gedqqdhsb.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gqtifunvp.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gpepgmjpt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/ggbtlhsnp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqpvwnidt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/glfilnsyl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gqqqlhcwd.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gmmnnrglh.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gkqzkfwen.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gvcevohgh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/glxqinzde.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gagksnniu.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/ghyfafgok.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gdyrekqaq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gwsjnrfjx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gnigzrlqf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gkcffkygh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gthltbvic.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gluydsqjq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/glxpbsqnu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gyyacsxrj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/geilixufh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gzvxvgsnn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gjxnfargt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gyihnwpqc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gkszitelt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gstcpmtvi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gytfverna.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gavjwhisl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gqdjqdabd.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/geaxodhtp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/grmlnlbsy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/geoaxlfnw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gmkbxkhdp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gpphkvnxu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gujdffhev.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gxvtllvbm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/ggsdiicmk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/guqxnooib.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gvybppdcd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gvvqtcood.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gfntkiyfd.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gkfovlxqc.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/guzfjzizc.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gkfojwwmh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gaonujqby.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/goggcnsjs.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gatuiohwh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpqavtssi.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gbuodnvop.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwpbgjpib.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/grepytvnq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gkzozpuyq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gtmfclqex.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gwlbxzcmz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gauicpcep.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/ghgvtqmus.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gfzwfmqkj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gfasoqczr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/grqmsyjik.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gltwysljt.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gtxsoamxj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/ggizcszsa.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gkshrmljz.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/grmfocwmv.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gvbixekhr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gjhfzkgux.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gfnsmsbvf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gxwlyapxc.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gtbruigdq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/giivdtnkz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gqahvvoxm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gslpsrjhf.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gtryizjzj.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gyfqwwibz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gebibxksb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gndnypbtf.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/givqwunkg.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gvribogmi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/goiotrakm.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/ghutswsbw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/guifnktya.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/giusuvqhn.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gdgckfubc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/ghvwoleak.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/giuokzixz.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gooozxxyp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gnbjlnbwh.sHtML


<!-- 参考信息 -->