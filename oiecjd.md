代发 wailian999

ssh user@host 'uptime'
来源：http://hz.zhongyouzk.top/gtheeetewu.html

[R58] 下载文件
来源：http://hz.ydzc1.top/gtuxzwdgkv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hnxiangtu.top/gtkwptwttm.html

[R59] 发 POST JSON
来源：http://hz.9152youxi.cn/gtvnlevekj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinyuanbaomall.cn/gtbgmkvvkr.html

[R60] 只看 HTTP 状态码
来源：http://hz.c1oappe.top/gtbnmoswvl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangdashe.top/gtnuqtvwzg.html

[R61] 磁盘占用
来源：http://hz.meibo888.top/gtbgqyupaj.html

df -h;  du -sh *
来源：http://hz.dashuyun.cn/gtqgxmiwbi.html

[R62] 找最占空间的文件
来源：http://hz.aibaodan.cn/gtntejepoj.html

du -ah . | sort -rh | head -10
来源：http://hz.jinqigufen.top/gttlnhprnm.html

[R63] 内存与进程
来源：http://hz.cheryme.top/gtnriouapz.html

free -h;  ps aux | grep nginx
来源：http://hz.guowangkeji.top/gtoojzsczy.html

[R64] 结束进程
来源：http://hz.52xcode.cn/gtfrlfqlmy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhixingplan.top/gtcmrnaknm.html

[R65] 查看端口占用
来源：http://hz.mhx1999.top/gtohodkanq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.dashuyun.cn/gtqhhooyfy.html

[R66] 定时任务
来源：http://hz.9152youxi.cn/gttivbqgfa.html

crontab -e;  crontab -l
来源：http://hz.ehwqpu.com/gtxumjceus.html

[R67] 生成随机十六进制串
来源：http://hz.tanke756.top/gtmfztbbpx.html

openssl rand -hex 16
来源：http://hz.52xcode.cn/gtrvlcjjoh.html

[R68] 计算文件校验值
来源：http://hz.pycfn.com/gtbnopocmy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.wangdashe.top/gtimbqxtyg.html

[R69] 生成随机密码
来源：http://hz.cheryme.top/gtlbqkfuya.html

head -c 16 /dev/urandom | base64
来源：http://hz.zdqjudy.top/gtulqimjtk.html

[R70] 时间戳与互转
来源：http://hz.daria6918.cn/gtnqwdvida.html

date +%s;  date -d @1700000000
来源：http://hz.nwbrower.top/gtsnphchhh.html

[R71] 日期格式化
来源：http://hz.feifeiyinyue.top/gtpxhrgsao.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.fzhhl.top/gtnhrpvaqa.html

[R72] 等待端口就绪
来源：http://hz.kuanghao11.cn/gtypkiyxjz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.fengsongda.top/gtcpdbdikk.html

[R73] 分割大日志
来源：http://hz.shuidangran.top/gtzqtyghrm.html

split -l 1000 big.log part_
来源：http://hz.smart0.xyz/gtifgglcoi.html

[R74] 批量重命名
来源：http://hz.cheryme.top/gthfkqstrm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yueranfly.top/gtzjkzpifj.html

[R75] 导出环境变量
来源：http://hz.shanyushiyangkeji.top/gttqboctie.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenzaomai.com/gtidllfujq.html

[R76] 使用临时文件
来源：http://hz.zycfv.cn/gthlneihxb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhengqikj.top/gttrmaiutj.html

[R77] 读取用户输入
来源：http://hz.tianlin.xyz/gtdsfrvlkm.html

read -rp "请输入: " ans
来源：http://hz.0kj1m.cn/gtwhvmknic.html

[R78] 交互式菜单
来源：http://hz.wangshuangyany.cn/gtdcvivsvk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gotoacloud.top/gtiianexon.html

[R79] 解析命令行选项
来源：http://hz.cdnleiting.top/gtttznwwyn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gotoacloud.top/gthkfttnby.html

[R80] 查看脚本执行耗时
来源：http://hz.bjfxy.top/gtplayjqso.html

time ./run.sh
来源：http://hz.meibo888.top/gtletmsujm.html

================================================================================
来源：http://hz.52xcode.cn/gtrzydscww.html

S. C / C++ 专题
来源：http://hz.andypj.xyz/gtbzctizcl.html

================================================================================
来源：http://hz.yueranfly.top/gtategnjtx.html

[S01] C：Hello World
来源：http://hz.52xcode.cn/gtmqrvqqdh.html

#include <stdio.h>
来源：http://hz.shuidangran.top/gtixztuezp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.dashuyun.cn/gtbwseictv.html

[S02] C：变量与格式化输出
来源：http://hz.jqgfzy.top/gtpjvaifdl.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhixingplan.top/gtdxwyvjdm.html

[S03] C：读入整数
来源：http://hz.mhx1999.top/gtdzdwhkpr.html

int x; scanf("%d", &x);
来源：http://hz.yuanzhike.top/gtvzybrkln.html

[S04] C：字符串复制
来源：http://hz.cqqwz.cn/gttdbxpcsd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.iojbl.cn/gtzjmdotxy.html

[S05] C：字符串长度
来源：http://hz.smart0.xyz/gtuloujayn.html

strlen(s)
来源：http://hz.sysykeji.top/gtkyntcmtu.html

[S06] C：字符串比较
来源：http://hz.pycfn.com/gtrjgqoulm.html

strcmp(a, b) == 0
来源：http://hz.sweek.top/gtljhnmtaz.html

[S07] C：数组遍历求和
来源：http://hz.jqgufenzy.top/gtrfjdrklj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yvedp.cn/gtnndwqoho.html

[S08] C：动态内存分配与释放
来源：http://hz.chenjidiqi.icu/gtmxrfsdch.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jianghu66.top/gtqxaepktj.html

[S09] C：结构体定义与初始化
来源：http://hz.yj20258.top/gtydeskqlh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hysaishi.cn/gtdmpsowxn.html

[S10] C：指针与解引用
来源：http://hz.cheryme.top/gtrapolipn.html

int *p = &a;  *p = 5;
来源：http://hz.jqgufenzy.top/gtqkywxoif.html

[S11] C：逐行读文件
来源：http://hz.redwolf501.top/gtposkkeqp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.birdmap.top/gtjwfphisd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cqqwz.cn/gtbhtwnmvf.html

fclose(f);
来源：http://hz.yuxming.cn/gtctnvoanw.html

[S12] C：写文件
来源：http://hz.yuanzhike.top/gtqepkqtng.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhaomingkeji.xyz/gtidnxnuxo.html

[S13] C：宏定义
来源：http://hz.yj202588.top/gtephplzsq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinghuilouyu.cn/gtaaclkqqk.html

[S14] C：枚举
来源：http://hz.pycfn.com/gtzsmouakj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zycfv.cn/gtnplmwafn.html

[S15] C：类型转换
来源：http://hz.jiagoushi.top/gtclyjydiz.html

(double) a / b
来源：http://hz.gotoacloud.top/gtfftiymqt.html

[S16] C：位操作置位
来源：http://hz.yj202588.top/gtbnvqdqce.html

x |= (1 << 3);
来源：http://hz.zhiwuduotai.top/gthuubdogf.html

[S17] C：安全拼接字符串
来源：http://hz.redwolf501.top/gtmvfctxxf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yangfankeji.com/gtfjldxeyn.html

[S18] C：命令行参数
来源：http://hz.hongshengwenyu.top/gtjrrwgchz.html

int main(int argc, char **argv)
来源：http://hz.yueranfly.top/gtxvfoyhrj.html

[S19] C：快速排序
来源：http://hz.ppjwa.cn/gtluvqxwbn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhengqikj.top/gtczqgngvn.html

[S20] C：二分查找
来源：http://hz.xinyue.icu/gtsshjapwd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yongpay.top/gtvyiwlrhk.html

[S21] C：字符类别判断
来源：http://hz.xziqi.cn/gtmlmtopry.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gzhubu.top/gtbvehpsqj.html

[S22] C：字符串转数字
来源：http://hz.c1oappe.top/gtdpmxddhs.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.svipenyu.cn/gtoevdgatn.html

[S23] C：随机数
来源：http://hz.nwbrower.top/gtpyclvjns.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zdqjudy.top/gtzgrweeeo.html

[S24] C：获取本地时间
来源：http://hz.tanke756.top/gtyefadayk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cashguo.top/gtnexmpwtr.html

[S25] C：内存拷贝
来源：http://hz.sxryk.cn/gthnavvdjg.html

memcpy(dst, src, n);
来源：http://hz.cucudq.cn/gtknszhsnq.html

[S26] C：内存清零
来源：http://hz.hammf.cn/gtzkrjppue.html

memset(a, 0, sizeof a);
来源：http://hz.nanxinkj.top/gtmimsehti.html

[S27] C：定义常量
来源：http://hz.meibo888.top/gtgecgpkib.html

const double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtvwekplyw.html

[S28] C：静态变量
来源：http://hz.yongpay.top/gttprtjnws.html

static int counter = 0;
来源：http://hz.sweek.top/gtsjqqxrtz.html

[S29] C：变参函数
来源：http://hz.havefunace.top/gtmlsjaodt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhengqikj.top/gtekbzhbdf.html

[S30] C：头文件保护
来源：http://hz.smart0.xyz/gtjyffoclr.html

#ifndef X_H
来源：http://hz.andypj.xyz/gtksagkabq.html

#define X_H
来源：http://hz.zhoulong.xyz/gtpqgsyfrh.html

#endif
来源：http://hz.daria6918.cn/gtxstxqjfm.html

[S31] C++：Hello World
来源：http://hz.c1oappe.top/gtxkuldugv.html

#include <iostream>
来源：http://hz.ywan-chungtsiang.top/gtfqmglmry.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yuanzhike.top/gtfeapmyid.html

[S32] C++：字符串
来源：http://hz.havefunace.top/gtnydfomop.html

std::string s = "hi";  s += "!";
来源：http://hz.shzxlz.cn/gtggpnfixk.html

[S33] C++：vector 增删
来源：http://hz.xuanzx.com/gtmafnufhw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.chenjidiqi.icu/gtnbplrxhl.html

[S34] C++：遍历 vector
来源：http://hz.zhaomingkeji.xyz/gtsatnxsah.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jyoumei.cn/gtvjgqdisk.html

[S35] C++：map
来源：http://hz.shuidangran.top/gtxfwtjecg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gtxffjvicz.html

[S36] C++：unordered_map
来源：http://hz.yongpay.top/gtakkqfhqj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jyoumei.cn/gteorjodca.html

[S37] C++：set
来源：http://hz.shangyingyoupin.top/gtacpsvjdd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.0kj1m.cn/gtfhsgzpxr.html

[S38] C++：排序
来源：http://hz.havefunace.top/gtngsimrko.html

std::sort(v.begin(), v.end());
来源：http://hz.feifeiyinyue.top/gtifbnadaw.html

[S39] C++：自定义比较器排序
来源：http://hz.ywan-chungtsiang.top/gtpcnggpmq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shzxlz.cn/gteumufjkm.html

[S40] C++：查找元素
来源：http://hz.yongpay.top/gtyuptwezg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zycfv.cn/gtpnzmhcfd.html

[S41] C++：类与构造函数
来源：http://hz.wangshuangyany.cn/gtnpxfybtt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sxryk.cn/gtsvbsxpob.html

[S42] C++：继承与虚函数
来源：http://hz.yj20258.top/gttgyepzyk.html

class B : public Base { public: void f() override {} };
来源：http://hz.yanxiufei.cn/gtubfjcefe.html

[S43] C++：智能指针
来源：http://hz.52xcode.cn/gtfxhshwhk.html

auto p = std::make_unique<int>(5);
来源：http://hz.yangfankeji.com/gttzojbylv.html

[S44] C++：引用传参
来源：http://hz.aizwys.cn/gtripsvhlq.html

void inc(int &x) { ++x; }
来源：http://hz.wangshuangyany.cn/gtizpuptmp.html

[S45] C++：lambda
来源：http://hz.nwbrower.top/gtbokyjxsv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ybcxt.top/gtnbwpzhoo.html

[S46] C++：函数模板
来源：http://hz.yonumen.top/gtzdgzqmsm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ppjwa.cn/gtchsuwnbk.html

[S47] C++：结构化绑定遍历
来源：http://hz.tanke756.top/gtfzyfugyl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.guannengcc.top/gtbjbpobwy.html

[S48] C++：逐行读文件
来源：http://hz.gaohongyu789.top/gtefpdppds.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinqigfzy.top/gtymavqwfi.html

while (std::getline(in, line)) { }
来源：http://hz.316326.xyz/gtejksrcfr.html

[S49] C++：写文件
来源：http://hz.gzhubu.top/gtlexguklo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydzc1.top/gtphbvdzom.html

[S50] C++：格式化数字
来源：http://hz.sysykeji.top/gtkyxhshkt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.wangdashe.top/gtgikwobsm.html

[S51] C++：显式类型转换
来源：http://hz.svipenyu.cn/gtuubggaqu.html

static_cast<double>(a) / b
来源：http://hz.hysaishi.cn/gtbbkwmyid.html

[S52] C++：const 与 noexcept
来源：http://hz.fzhhl.top/gtgjwblrpf.html

int size() const noexcept { return n_; }
来源：http://hz.jinqigfzy.top/gtxfpfwfkp.html

[S53] C++：移动语义
来源：http://hz.hnxiangtu.top/gtprogfmyh.html

std::vector<int> w = std::move(v);
来源：http://hz.zhaomingkeji.xyz/gtcwojtbmf.html

[S54] C++：异常处理
来源：http://hz.cheryme.top/gtwdzwvegg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.aibaodan.cn/gthtlkgoyv.html

[S55] C++：结构化绑定
来源：http://hz.jlsjyb.cn/gtujctdnvc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cqqwz.cn/gtecmrtejo.html

[S56] C++：optional
来源：http://hz.yangfankeji.com/gtwkijvzad.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nanxuanxn.top/gtdyeypobw.html

[S57] C++：编译期常量
来源：http://hz.bjfxy.top/gtbrwwfeyb.html

constexpr int N = 10;
来源：http://hz.zhaomingkeji.xyz/gtqiquzhqz.html

[S58] C++：命名空间
来源：http://hz.yuxming.cn/gtvgaiieqo.html

namespace ns { int f() { return 1; } }
来源：http://hz.bjfxy.top/gtclnzibih.html

[S59] C++：静态断言
来源：http://hz.ybcxt.top/gtntdpxgtq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ywan-chungtsiang.top/gtlfjdklso.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangkeji.top/gthxdaryvj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nanxuanxn.top/gtyrvmzkrl.html

================================================================================
来源：http://hz.jiagoushi.top/gtkuidalpv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gogol.net.cn/gteohphjof.html

================================================================================
来源：http://hz.tanke756.top/gtdpslcwiq.html

[T01] Kotlin：Hello World
来源：http://hz.aibaodan.cn/gttldmejpi.html

println("Hello")
来源：http://hz.xuanzx.com/gtuwhrilbc.html

[T02] Kotlin：变量
来源：http://hz.c1oappe.top/gtyjlcibrz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.haohaochexian.top/gtrsndjito.html

[T03] Kotlin：字符串模板
来源：http://hz.daxiang520.top/gtzqakhgro.html

"值: $b"
来源：http://hz.zhengqikj.top/gtxrmcxatq.html

[T04] Kotlin：空安全
来源：http://hz.cashguo.top/gtqdtpzbpw.html

val n: String? = null;  n?.length
来源：http://hz.nwbrower.top/gtvcbcuqvr.html

[T05] Kotlin：when 表达式
来源：http://hz.kuanghao11.cn/gtsxxmxzuc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xylfe.cn/gtuoteudap.html

[T06] Kotlin：集合映射
来源：http://hz.yonumen.top/gtkiuohqcy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.aizwys.cn/gthhmtygyr.html

[T07] Kotlin：集合过滤
来源：http://hz.ybcxt.top/gtpkxvgxfq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj20258.top/gtgmdrjyrh.html

[T08] Kotlin：数据类
来源：http://hz.jinqigufen.top/gtijobhkam.html

data class User(val name: String, val age: Int)
来源：http://hz.feifeiyinyue.top/gtvinkhypl.html

[T09] Kotlin：扩展函数
来源：http://hz.bjfxy.top/gtougtibmk.html

fun String.exclaim() = this + "!"
来源：http://hz.feifeiyinyue.top/gtcnlsfmhp.html

[T10] Kotlin：默认参数
来源：http://hz.jqgfzy.top/gtippggftn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.c1oappe.top/gtxzhvwhbl.html

[T11] Kotlin：协程
来源：http://hz.hfpthk.cn/gtnwjzsifg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zdqjudy.top/gtvqzcnsot.html

[T12] Kotlin：解构声明
来源：http://hz.yonumen.top/gtoftisslr.html

val (a, b) = Pair(1, 2)
来源：http://hz.yvedp.cn/gtyudbvjzv.html

[T13] Kotlin：只读 Map
来源：http://hz.hnxiangtu.top/gtlkoyfnit.html

val m = mapOf("a" to 1)
来源：http://hz.jiagoushi.top/gtpprbcoqd.html

[T14] Kotlin：循环
来源：http://hz.jiagoushi.top/gteomikhrv.html

for (i in 1..10) println(i)
来源：http://hz.yvedp.cn/gtnfacaign.html

[T15] Kotlin：接口
来源：http://hz.cqqwz.cn/gtvrozhyob.html

interface Shape { fun area(): Double }
来源：http://hz.pycfn.com/gtfgrryvmx.html

[T16] Swift：Hello World
来源：http://hz.yj20258888.top/gtmzgawqcq.html

print("Hello")
来源：http://hz.quarkkingdee.top/gtvfqentwe.html

[T17] Swift：变量与常量
来源：http://hz.jinyuanbaomall.cn/gtdtaigkor.html

var a = 1;  let b = 2
来源：http://hz.sufxvd.cn/gtisdgemvu.html

[T18] Swift：字符串插值
来源：http://hz.yvedp.cn/gturxukdih.html

"值: \(b)"
来源：http://hz.gzhubu.top/gtpwkgvkng.html

[T19] Swift：可选绑定
来源：http://hz.dianchejie.cn/gtdkkqvrtu.html

if let n = opt { print(n) }
来源：http://hz.zdqjudy.top/gtoyfjgwpk.html

[T20] Swift：数组操作
来源：http://hz.aizwys.cn/gtwpculesg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.nwbrower.top/gtiydwnqda.html

[T21] Swift：遍历
来源：http://hz.xziqi.cn/gtzvvgdvhg.html

for x in a { print(x) }
来源：http://hz.cucudq.cn/gtgdjvuozd.html

[T22] Swift：字典
来源：http://hz.tianlin.xyz/gtifhyxwfq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhengqikj.top/gtmtdkwnyp.html

[T23] Swift：函数
来源：http://hz.jqgufenzy.top/gtxvugawfp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.tanke756.top/gtjvnjodcz.html

[T24] Swift：闭包
来源：http://hz.sxryk.cn/gttysbyhyr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hongshengwenyu.top/gttflslyhl.html

[T25] Swift：结构体
来源：http://hz.cashguo.top/gtwjfpfelv.html

struct P { var x: Int }
来源：http://hz.smart0.xyz/gtzhrcxrox.html

[T26] Swift：类与重写
来源：http://hz.yanxiufei.cn/gtycshrydz.html

class A: Base { override func f() {} }
来源：http://hz.ydzc1.top/gtncogezbg.html

[T27] Swift：错误处理
来源：http://hz.0kj1m.cn/gtxvijdcca.html

do { try f() } catch { print(error) }
来源：http://hz.fzhhl.top/gtynnbljto.html

[T28] Swift：枚举
来源：http://hz.hnxiangtu.top/gtryasbuxw.html

enum Color { case red, green }
来源：http://hz.zdqjudy.top/gteukhztxz.html

[T29] Swift：guard 提前返回
来源：http://hz.9152youxi.cn/gtnszjrkvb.html

guard let x = opt else { return }
来源：http://hz.ywan-chungtsiang.top/gtfencfnbw.html

[T30] Swift：协议
来源：http://hz.zhixingplan.top/gtetdcqiud.html

protocol Shape { func area() -> Double }
来源：http://hz.wangdashe.top/gtyhlnxtir.html

[T31] Lua：Hello World
来源：http://hz.cqqwz.cn/gtbbnrwvds.html

print("Hello")
来源：http://hz.shangyingyoupin.top/gtayjbwanf.html

[T32] Lua：局部变量
来源：http://hz.tianlin.xyz/gtngmxitww.html

local a = 1
来源：http://hz.52xcode.cn/gtrhcnbbfn.html

[T33] Lua：表（数组）
来源：http://hz.xinyue.icu/gtjpdqpryu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xuetiantiany.cn/gtgefsxcpt.html

[T34] Lua：遍历表
来源：http://hz.jiagoushi.top/gtdfolvcgq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cdnleiting.top/gthvmvkfkd.html

[T35] Lua：字典表
来源：http://hz.gzhubu.top/gtpvttiuiy.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yueranfly.top/gtpwhwrlrp.html

[T36] Lua：函数
来源：http://hz.yongpay.top/gthkbutzmo.html

function add(a, b) return a + b end
来源：http://hz.jqgfzy.top/gtqbmitfnw.html

[T37] Lua：字符串拼接
来源：http://hz.zhiwuduotai.top/gtprqojsfp.html

"a" .. "b"
来源：http://hz.andypj.xyz/gtarkicesg.html

[T38] Lua：条件
来源：http://hz.tanke756.top/gtkicszayx.html

if x > 0 then print("正") end
来源：http://hz.xylfe.cn/gthoygelrp.html

[T39] Lua：模式匹配
来源：http://hz.gogol.net.cn/gtkdqcujfo.html

string.find(s, "%d+")
来源：http://hz.sxryk.cn/gtrvgvggol.html

[T40] Lua：元表
来源：http://hz.fzhhl.top/gtctluwpts.html

setmetatable({}, { __index = base })
来源：http://hz.hywenlv.cn/gtiptzzczn.html

[T41] Perl：Hello World
来源：http://hz.cheryme.top/gtwwwzwcfg.html

print "Hello\n";
来源：http://hz.nwbrower.top/gtghupwxup.html

[T42] Perl：变量类型
来源：http://hz.zdqjudy.top/gttqziwhul.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jyoumei.cn/gtmetehczt.html

[T43] Perl：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtpxofiydl.html

"值: $a"
来源：http://hz.nwbrower.top/gtsczltbfb.html

[T44] Perl：条件
来源：http://hz.c1oappe.top/gtwegcveiq.html

if ($a > 0) { print "正"; }
来源：http://hz.aibaodan.cn/gtcxqzxybx.html

[T45] Perl：数组遍历
来源：http://hz.xylfe.cn/gtfezhsmtm.html

for my $x (@arr) { print $x; }
来源：http://hz.redwolf501.top/gtbtozxoio.html

[T46] Perl：哈希操作
来源：http://hz.pengpengdd.cyou/gtihjtuoms.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.kuanghao11.cn/gtjavwpuvl.html

[T47] Perl：正则捕获
来源：http://hz.ppjwa.cn/gtshranbuw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ehwqpu.com/gtvptuagmh.html

[T48] Perl：正则替换
来源：http://hz.yonumen.top/gtnuyywdat.html

$s =~ s/old/new/g;
来源：http://hz.jianghu66.top/gtntszurea.html

[T49] Perl：函数
来源：http://hz.yueranfly.top/gtrspnnter.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.shangyingyoupin.top/gtdbzxxdls.html

[T50] Perl：逐行读文件
来源：http://hz.guannengcc.top/gtrgrxvuga.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhixingplan.top/gteqpeuzxm.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.mhx1999.top/gtqmztgggz.html

[T51] Scala：Hello World
来源：http://hz.hongshengwenyu.top/gteuiodnbz.html

println("Hello")
来源：http://hz.gogol.net.cn/gtdhzdqhcd.html

[T52] Scala：变量
来源：http://hz.yangfankeji.com/gtnhcchjtt.html

val a = 1;  var b = 2
来源：http://hz.yangfankeji.com/gteaiktdib.html

[T53] Scala：字符串插值
来源：http://hz.shangyingyoupin.top/gtbpcpwhfq.html

s"值: $b"
来源：http://hz.ybcxt.top/gtvprdxxdj.html

[T54] Scala：集合映射
来源：http://hz.hnxiangtu.top/gtuwyhlaue.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yj20258.top/gtgqytseye.html

[T55] Scala：集合过滤
来源：http://hz.guannengcc.top/gtuchqyiju.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jinghuilouyu.cn/gtfddknedu.html

[T56] Scala：样例类
来源：http://hz.hongshengwenyu.top/gtqyaoqlhs.html

case class User(name: String, age: Int)
来源：http://hz.aizwys.cn/gtezubbwwj.html

[T57] Scala：模式匹配
来源：http://hz.andypj.xyz/gtyhedrfzo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xinyue.icu/gtvplzhiph.html

[T58] Scala：函数定义
来源：http://hz.shanyushiyangkeji.top/gtnjucynzq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.haohaochexian.top/gtjoujgyyj.html

[T59] Scala：循环
来源：http://hz.zhengqikj.top/gtmalmggck.html

for (i <- 1 to 10) println(i)
来源：http://hz.andypj.xyz/gtopxnukdy.html

[T60] Scala：折叠
来源：http://hz.gaohongyu789.top/gtslwtngyy.html


<!-- 参考信息 -->