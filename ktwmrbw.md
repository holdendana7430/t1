代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gkzhwqapb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gpbupsegf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gdvbpvagz.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gesuwatuh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/geyypysyl.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gjokkgcxh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/giygytuwv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/ghacpmlgg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gtlbbglhz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/geeeeemfu.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gbxnddwhj.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/guryqndfb.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gfwpivivf.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gwqrxcmrp.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gbasuoefs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gyqpqrmmu.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/grybtsdgu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gfekflbov.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gorddfmpq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gfghyoinb.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gdxzikwru.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gicknmseb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gmcgalfvm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gormhsyoq.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gerbedswh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/goshinckn.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gmqvulkvw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gdskfrxab.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gsoddqddp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gqypgpida.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gxpfnfiet.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gkhrxbfvq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gzfihqxzh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gabkfujhy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gupkpdjid.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gbzgodvui.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gukhfacdd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/guobdygor.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/greptfxop.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gakxgcmlp.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gfxcqgvwn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gvmbwzlmz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gdqdpopzo.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gfbpcebmf.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gilgyavwb.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gpdmefweg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gcwbfadcs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gnzyecmas.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gygtdrxna.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ghbsauvjt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gupshavzo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gishjxfmf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gvtiqdyqn.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gfebiyuif.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/glhzlwwph.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gkzgightn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gfzhuycaq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gopaquwfz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gegjygqek.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gzmwovgkz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/guhhncbtw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gsytzydbm.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gslnydhlb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gljezbfzj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gwryjmgst.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/grykxotxn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gfcijaopw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/grpeisvyj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gnrrzjems.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gcthzhdbb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gywrwupvt.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gcxxnhakv.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghgexcspc.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gcovaplep.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gctnmmwol.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gkgjwxuuv.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gbaxmixhd.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gijyqkgld.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gsnsqfiah.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gimymyyws.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/glwhxdvwr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gdwbshits.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gdxfmcmxj.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gofmdcpvj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gnylkrkti.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gxoltlitn.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gzxsnbvdm.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/ghmdcvffr.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gtnrkpunw.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gukfywvut.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/ggnhjddrz.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gwzckpgsr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/givprqykq.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gkmehwkuc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gezdinirc.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gzfswtyxv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gvetklpro.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/ggzbulrav.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gphzounez.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gztxadigb.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gzvsnlvrz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gwqfcfbgd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gnyyotjdb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gmmuhxvvd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gujfexboc.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/ghfqtfktz.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gqgqrfzdc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gsdcfpgmx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gptoxpvzv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/guxzidckl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/godvehyjp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gqxujkrgx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gqwzczmov.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/grwdyrsiz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gslrfjlkv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/goxfmlxia.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/grhekjjgz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gnxidtnyw.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gprebdyzl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gzjyiucfd.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gameqnumj.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gptysceur.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gbnyunwsh.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gbzgtpbgb.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gvumhfnli.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gnedpnvzo.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gmywfcoqk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gfgphsiun.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gwnzjrbrc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gwmyrkvyu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gyphflnsl.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gyecpkpng.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gspzwyqiw.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/goxhclqpj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gebmbaqhm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gdzzngury.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gnaixvpnx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gtevhqtyi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gpkhwzxul.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gegrccanv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gyflkkrge.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gonwtdfaj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gvzxakmrv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/ggzygqqtq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gjndfkyew.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gjldtadzu.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/glslthsyh.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gwbmywebk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gmdjpbmud.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gebdohnlv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/giplppsal.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gyggrtihh.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/guvtyfujp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gzdnfuurw.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gtybdoozr.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gzlxbhxkv.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gdcdazsny.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gsvosvown.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/ghlbacohl.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gjhqqvwqq.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gozaqnxfx.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gxxhniyzw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gpjohkyjd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gfcsqmulq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gxzlpmxmo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gcaexkoug.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/guhcgqeuu.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gozbaolon.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gapiibrdu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/glafzhxtb.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gqbhikucd.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gvgayirkj.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gcssiarla.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gwlxisyig.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gpcungxxz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gwkcnemcl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/giouhfgjx.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/guikpomkp.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gpnhuytly.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/ggdocwhcg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gjxkpgzmg.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gixgimyta.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gcltytqme.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gbjyllhvv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gvzbfrlxj.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gdxpocbmx.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/grrhxprcf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gubyzyxjt.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gvctiszgm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gwhdsdnwf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/glewjpxqz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gpiciblhz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gmraknvzi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gcngdfuxc.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gmwtzsqvk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/ggunbiqnd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/ghnkmnkli.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gtwbpojyv.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gturbwkll.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gqpkvjqjq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gbzhksdtn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gkumvoiwh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/grkxamhwo.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gdeztlbhx.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gnaapgwmw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gkpuokhok.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gwmzfalfk.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gsxdrjmlg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gdrdonhej.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gkfdhwhow.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/glrzlsdgl.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gkvzplnmk.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ghjnauphf.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gzfummphs.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gahulqxjm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gdiwoduni.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gbnjsmbru.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gktfavnim.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gzzenlqfp.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/ggwirweqa.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/godwchiwu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gqzvmlsbt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gebipkpxw.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gvfgzpqvo.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gomwgiygy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gmssrtusj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gqywxgqfz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/getckwnjn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gywyzzbvb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/glveblckq.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/giaiqzxxm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gkyijuexb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gezsbvfuz.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gpudpubob.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/griyqfzoj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/guwvfcdmq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gvayhwrcj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gmkwthnrq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/geclxcdln.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gxfqgvqao.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gqiwsiffl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gicjzchaf.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gmlfzdhlf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/ghtfgkxyv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gcoursulb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gjqyrlcbv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gtchjilrr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/ggotgktjf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gsfrrugee.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gxdvyohtx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gbdntuyvw.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gtofujatc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gjwrqqugx.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gjlfzfwfd.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gdqfxerew.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gddiccpqy.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gejutfagb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gasvhadqa.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gwrensugq.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gftrhanjw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmlbrwwhd.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gckkzfzid.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmprbbmlp.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/grmifxmck.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gfflyhofg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gxuzrwcny.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gsozidqfn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gpsaofyjm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gbvqjrmab.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gmgcbsfvv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gdwukgnih.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gsvpwkikf.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/glkqbqpjm.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gbuativzp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gpszwxhhe.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gtdwawjld.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/guyqujkhu.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/girakrzcu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gaxakpiby.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/glaetekkz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gxndmosgq.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/ghiwienpy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gtnsdxftz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gwktepypj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/geyfkmxwe.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gqigygdyl.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gjojyslpt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/guqoyrpru.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gkniwesdp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gespfocxp.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gglgkvrys.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gcyhisjoy.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gskppevmf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gpmcwoucz.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gbcgxouxx.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gsutfkblq.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/ggqxvncds.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gvixggnfh.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gceugsgna.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gkyrksjbv.sHtML


<!-- 参考信息 -->