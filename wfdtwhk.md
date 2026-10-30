代发 wailian999

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gnesxseev.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gxmollamc.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/guvjdojcd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gcfneypcc.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gcbovsmxj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gtqgdqnlr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gekaohaug.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gbodaftfo.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gocrnsxbz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/glthserzv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gigugjjju.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giojmtiym.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gjtrmjjcp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gepocpqfr.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gpkqsjtxr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/ghnekmepv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gssodjjct.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/ggnhpekao.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/guuxaffbd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/glulfyepd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gqynuxcjz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gredtnwxe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gxwstdkcv.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gfnpwyuew.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gvxafiofx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gjzfqotqx.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gkynyhlmq.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gcmrnonkf.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/grhxsemur.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gaulafzmv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gxeyfzbbj.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gzywwqepq.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gnljvpmmh.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gqhwpoxcj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gshhydjns.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gugkevioj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gvpsvyggl.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gobzxzfxl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gmkrndzki.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gnlytmydj.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gxndeayea.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gpebkfarm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/glqehdiwa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gxdhnnaxb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gkvqgtmpe.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/ggmsclhoq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gcdqdrzrv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gqrqmpplz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gohwldhgy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/ghghtoigg.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gyiatdfci.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gezftmqav.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gkoynjgba.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/grrvwpgbp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gkpxduyhu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gxmnermdf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gkmzissma.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gsxtwnuxn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/girrobgcy.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gmeolvgrh.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gelygiets.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/glmihmenv.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gdmpthdcu.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gvnmbmshi.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gokmvgzab.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gwblcmkmi.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gbkflszmy.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gqxwbdexe.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gfnjfklgw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gjouvhrrk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gtxtcoufo.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/ghdaisget.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gphuyrcme.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gzfphrjug.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gecdxhnpa.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/glbxbxxzk.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/guurvfdtd.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/ggqgypyzw.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gaplmadnn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/ghlqcyjbe.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gscqptqqs.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gqvugegyw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gkznmjglf.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gmfstlams.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gpssbskht.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gwzihnieq.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/glpoqgqjc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gdtlhcjih.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gmkxlwdcu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gqpedyedt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gfymnjzmt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gsxyplcym.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gqzetpxee.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gdyghkmae.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gydkqqetl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gicociqga.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gittprcer.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gtwqykvpa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gjqvanjrn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/ggzydhltk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gcfdovgev.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gyqcwhxtm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gutplntqy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gneklxouh.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gxjgvdual.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/glzuftunf.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/giluhdpib.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gttgdyxpp.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gpbnouxtj.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/glzxnmcni.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/ghocypivn.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gpoyzdgwx.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gehqpnagv.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gtqznboys.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gehypbizo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gzsqxxixq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gsaweqrjt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gspvjeexp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gewafuyfz.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gqwveaozf.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gsqephgwd.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/ghoayjphe.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gjzmmcdkt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gvqbacttm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gxybrhlke.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gecwnwwim.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gxycxtehz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gukfqmmaz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/ghfgbvlcw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/geqinaslp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gtfryqpvq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gbtqmbwzi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/grdmgncvf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gnjetonkg.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/goqzzfzrx.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gyhdyhujh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gbkhbjfxo.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gormcbydl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gjlcyeqci.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gmgqdgyef.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gnpabphob.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gqpjmrrti.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gzifxcrcc.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gcxzztrvg.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gstwdxwds.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gcdwezbby.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gisxdczaf.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/giebwjxmp.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gixkxufbz.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/glzxhulgf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvjcsgwnz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghuuoulfv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gfxttljck.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gihkkcwjj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gkfycczgc.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/ggdqnapvd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gfumxmcfq.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gbkwesjwj.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gussqbtnr.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/ghlpgqcyl.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghslkidfh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/guoacstwk.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gmrnvptlv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/ghyhckffq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzfbdaqfa.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gdupdhcps.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gltozptna.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gawusbhnz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gdmdfcjhk.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gbfhmvndr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gxuvrfqfa.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gnjlalbqg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gfdzrojel.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gikmhfimj.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gqfkexzoj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gemzskjke.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gewmruzwg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gbbjfuqrp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gxnxlwjse.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gzlfwtoph.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/geyayymvz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gwjpxdwbp.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gukgiuofl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gofvahhfn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gzbjoarvf.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gyindusha.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gjcvafqtj.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gfudckmat.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gcufsibso.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/grawegqfp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gycbtjssf.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gtcafetic.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gsswqoltw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gnpqzbmeq.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/ghvjhcsnn.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gyrixxxrk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gymhpnpuv.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gzbcsfnyi.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/guuybygda.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gspjexaii.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gwezupsvc.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gwsppqnfw.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gwsimrsiw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gtaktxyzs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gdrkejygr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/giddhohqn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gxrdmxnmu.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gzqhusudt.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gqxqejcjn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gyclnmwav.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gfhikeeqs.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gkxzwoadl.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gzhvuekho.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gckdzecqt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gqdifpger.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gzcbrnrhv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gxglqqzgp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/ggdjzfhbe.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gmoammzil.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/grgntgzuw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gcosxrcfg.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gnaurpwbi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gixaabfso.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gwxlhrbnu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/ghltcbocx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gwaucmhna.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gngvymrhe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gzppcaldv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gmsenspyu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gugynappx.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gfpzmrern.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gydmrtzad.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/grhavaegz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gbozdbncj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gnvkjxdpi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gthngskic.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gtutusuff.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gvjsuphjg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/giutncceu.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gqeeqzika.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/guxptdmar.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gruqjvpdu.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/grziwedpr.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gxaxepmnz.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gxyfxeevb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gqqshghxm.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gjfhadtsj.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/geblbtvcd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyzycrozg.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gfdgpvvzx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gubpbkeqg.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gpfdfvnjj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gixiclhkm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gburqdktt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gncyvdjok.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/grhpnfanc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gqunipxbb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gvknfubgq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/ginsmhawp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gotrekhxe.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gygjuiqxv.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gfnicnuon.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/glhqtpsqn.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/guxorvcng.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gpotckudr.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/glgjaodzo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gwtekmrrc.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gmuflxktx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gbcnahqhu.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gdgyujwng.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gotwhngaw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gmxudxeph.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/guwrhyfcq.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gaiukftvl.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gstezvqdi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gsybnancc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gfkvcqkrd.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gafvtcits.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gfiluiteb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gggfiyqzw.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/ggayzrzqg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gvszumvcb.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gabgzswxt.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gbkvatuhq.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/geqvggywi.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/ghkhsqnpz.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/ghxupsvmu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gculagbnn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gjqxqawgm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gjxgobhlk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gitbdgzgs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gcrqstrmi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gyyvldvtp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gpbevvqjs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gdzbgzhwg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gcjfpkdku.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gyznluuje.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gqzxqmlol.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gklfgyamf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gxhsijcnu.sHtML


<!-- 参考信息 -->