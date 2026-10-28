代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhijiandao.cn/gtddknjqdl.html

[R54] 比较两个文件
来源：http://hz.yongpay.top/gtbxsmsuek.html

diff a.txt b.txt
来源：http://hz.ydzc1.top/gtebdclrtm.html

[R55] 压缩与解压
来源：http://hz.vqdsnc.cn/gtoaibmsay.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhongyouzk.top/gtcacjgxcx.html

[R56] 远程拷贝
来源：http://hz.0kj1m.cn/gtxpvoteta.html

scp file user@host:/path/
来源：http://hz.kuanghao11.cn/gtktbwvptc.html

[R57] 远程执行命令
来源：http://hz.jinghuilouyu.cn/gthfexcics.html

ssh user@host 'uptime'
来源：http://hz.fzhhl.top/gtufcbhiud.html

[R58] 下载文件
来源：http://hz.chenzaomai.com/gtyippmihg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shangyingyoupin.top/gtxnwrotzj.html

[R59] 发 POST JSON
来源：http://hz.yonumen.top/gthsfrghtc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.aizwys.cn/gtmldjmmhu.html

[R60] 只看 HTTP 状态码
来源：http://hz.andypj.xyz/gttbdevqxi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hammf.cn/gtnultzdnf.html

[R61] 磁盘占用
来源：http://hz.xuetiantiany.cn/gtnjaezduh.html

df -h;  du -sh *
来源：http://hz.cheryme.top/gtrozfmwac.html

[R62] 找最占空间的文件
来源：http://hz.jyoumei.cn/gtxlkrvuoz.html

du -ah . | sort -rh | head -10
来源：http://hz.guannengcc.top/gtbuhhyxjp.html

[R63] 内存与进程
来源：http://hz.jinqigufen.top/gtxqozcwbw.html

free -h;  ps aux | grep nginx
来源：http://hz.gaohongyu789.top/gtwlcmzvcl.html

[R64] 结束进程
来源：http://hz.gaohongyu789.top/gtchzmobkg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.svipenyu.cn/gthbncfquh.html

[R65] 查看端口占用
来源：http://hz.ywan-chungtsiang.top/gtdbbvzbjv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shzxlz.cn/gtkvzgsduw.html

[R66] 定时任务
来源：http://hz.haohaochexian.top/gtoamyzeud.html

crontab -e;  crontab -l
来源：http://hz.fengsongda.top/gtekdrvxdf.html

[R67] 生成随机十六进制串
来源：http://hz.wangshuangyany.cn/gtelyuudlf.html

openssl rand -hex 16
来源：http://hz.xinyue.icu/gtazgrxtfq.html

[R68] 计算文件校验值
来源：http://hz.shzxlz.cn/gtbpoqhbwy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenjidiqi.icu/gtpppqtmin.html

[R69] 生成随机密码
来源：http://hz.zhoulong.xyz/gtqaqvruaf.html

head -c 16 /dev/urandom | base64
来源：http://hz.tianlin.xyz/gtlifhqlok.html

[R70] 时间戳与互转
来源：http://hz.316326.xyz/gtmrcidvdp.html

date +%s;  date -d @1700000000
来源：http://hz.316326.xyz/gtqvslmrmy.html

[R71] 日期格式化
来源：http://hz.zycfv.cn/gthdqqcxzw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jlsjyb.cn/gtazgfqxfi.html

[R72] 等待端口就绪
来源：http://hz.jianghu66.top/gthqtkpqzo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinghuilouyu.cn/gtqkyoxblo.html

[R73] 分割大日志
来源：http://hz.yj20258.top/gtgbeekynv.html

split -l 1000 big.log part_
来源：http://hz.xylfe.cn/gtijhobvcq.html

[R74] 批量重命名
来源：http://hz.guowangkeji.top/gtupbbevft.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.iojbl.cn/gtfdllidzb.html

[R75] 导出环境变量
来源：http://hz.yj20258.top/gthdndhssk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.andypj.xyz/gtwidrtven.html

[R76] 使用临时文件
来源：http://hz.tanke756.top/gtkrmypwyo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hfpthk.cn/gtjlmvhlam.html

[R77] 读取用户输入
来源：http://hz.meibo888.top/gtcldznbgj.html

read -rp "请输入: " ans
来源：http://hz.jinghuilouyu.cn/gtbenxvehk.html

[R78] 交互式菜单
来源：http://hz.hfpthk.cn/gtefdyjxmc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.pycfn.com/gtqrusuxlu.html

[R79] 解析命令行选项
来源：http://hz.zhaomingkeji.xyz/gtsafuopwf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sysykeji.top/gtoxrrpvad.html

[R80] 查看脚本执行耗时
来源：http://hz.haohaochexian.top/gtsolrkyfh.html

time ./run.sh
来源：http://hz.zhiwuduotai.top/gtflswnfmx.html

================================================================================
来源：http://hz.dashuyun.cn/gtisjkxwxb.html

S. C / C++ 专题
来源：http://hz.jianghu66.top/gtdkpemplj.html

================================================================================
来源：http://hz.ydzc1.top/gtegtjjsjs.html

[S01] C：Hello World
来源：http://hz.sysykeji.top/gtiqnscvxv.html

#include <stdio.h>
来源：http://hz.sufxvd.cn/gtpglqtpgo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gaohongyu789.top/gtzhytfvdr.html

[S02] C：变量与格式化输出
来源：http://hz.ppjwa.cn/gtxoxsjsxr.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhijiandao.cn/gtnklggema.html

[S03] C：读入整数
来源：http://hz.yj20258.top/gtbmzcxdve.html

int x; scanf("%d", &x);
来源：http://hz.quarkkingdee.top/gtojsdachx.html

[S04] C：字符串复制
来源：http://hz.xuetiantiany.cn/gtrxfdhhqv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.bjfxy.top/gtbyxzdkac.html

[S05] C：字符串长度
来源：http://hz.smart0.xyz/gtzikazxro.html

strlen(s)
来源：http://hz.sufxvd.cn/gtzdssgini.html

[S06] C：字符串比较
来源：http://hz.xuetiantiany.cn/gtosfecgcf.html

strcmp(a, b) == 0
来源：http://hz.fzhhl.top/gtbvzzfwhu.html

[S07] C：数组遍历求和
来源：http://hz.jyoumei.cn/gtrgclkdaf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tanke756.top/gtuzcujhja.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxuanxn.top/gtptipltno.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhengqikj.top/gteisrzewe.html

[S09] C：结构体定义与初始化
来源：http://hz.cashguo.top/gtkqxzspdw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hnqzz.top/gtfkqbuuow.html

[S10] C：指针与解引用
来源：http://hz.shanyushiyangkeji.top/gtnrgrplgc.html

int *p = &a;  *p = 5;
来源：http://hz.nwbrower.top/gtsyzptvwz.html

[S11] C：逐行读文件
来源：http://hz.xziqi.cn/gtpxjmskeu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hywenlv.cn/gtgugkuzze.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ydjk.org.cn/gtfmaapipx.html

fclose(f);
来源：http://hz.fengsongda.top/gtijwgudxb.html

[S12] C：写文件
来源：http://hz.gzhubu.top/gtfnrfxycd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.aibaodan.cn/gtcnfzsvcw.html

[S13] C：宏定义
来源：http://hz.zycfv.cn/gtvvblvqik.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.pycfn.com/gtzbpvqpqg.html

[S14] C：枚举
来源：http://hz.mhx1999.top/gtlsuqgsst.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hnqzz.top/gtwqulhscu.html

[S15] C：类型转换
来源：http://hz.xuanzx.com/gtygfbzzhc.html

(double) a / b
来源：http://hz.birdmap.top/gtbnromgcr.html

[S16] C：位操作置位
来源：http://hz.xingfuxueyuan.xyz/gtuooxmnfq.html

x |= (1 << 3);
来源：http://hz.cheryme.top/gtlhxrsjny.html

[S17] C：安全拼接字符串
来源：http://hz.316326.xyz/gtagypixbg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xylfe.cn/gtprveewqc.html

[S18] C：命令行参数
来源：http://hz.9152youxi.cn/gtdwtmulqa.html

int main(int argc, char **argv)
来源：http://hz.gotoacloud.top/gtjbcpnpkc.html

[S19] C：快速排序
来源：http://hz.nanxuanxn.top/gtwlfuvvqg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sysykeji.top/gtsddepblr.html

[S20] C：二分查找
来源：http://hz.wangdashe.top/gtrtujdnik.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.aibaodan.cn/gtbwpvzkqi.html

[S21] C：字符类别判断
来源：http://hz.chenjidiqi.icu/gtscmhpsyl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.feifeiyinyue.top/gtgpdgkpnu.html

[S22] C：字符串转数字
来源：http://hz.hywenlv.cn/gtgzrlngvd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.birdmap.top/gtekedhxxs.html

[S23] C：随机数
来源：http://hz.yuanzhike.top/gtcsiahndo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenzaomai.com/gtjleiqnmc.html

[S24] C：获取本地时间
来源：http://hz.zhengqikj.top/gtkerajcvb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yueranfly.top/gtuhosdyet.html

[S25] C：内存拷贝
来源：http://hz.zhiwuduotai.top/gtfwkmzunr.html

memcpy(dst, src, n);
来源：http://hz.chenzaomai.com/gtpjjqarly.html

[S26] C：内存清零
来源：http://hz.c1oappe.top/gtxvnvdzkg.html

memset(a, 0, sizeof a);
来源：http://hz.fzhhl.top/gtsrtprrfw.html

[S27] C：定义常量
来源：http://hz.pengpengdd.cyou/gtgerltyzn.html

const double PI = 3.14159;
来源：http://hz.yangfankeji.com/gtqogykphc.html

[S28] C：静态变量
来源：http://hz.fengsongda.top/gtkuqvqsxi.html

static int counter = 0;
来源：http://hz.aizwys.cn/gtmzybnffr.html

[S29] C：变参函数
来源：http://hz.wangdashe.top/gtckssiise.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jiagoushi.top/gthwlwyzpr.html

[S30] C：头文件保护
来源：http://hz.aibaodan.cn/gtmeypleiu.html

#ifndef X_H
来源：http://hz.cashguo.top/gtjqgskdzz.html

#define X_H
来源：http://hz.c1oappe.top/gtlqqhfgcx.html

#endif
来源：http://hz.gotoacloud.top/gtbjqgbwuo.html

[S31] C++：Hello World
来源：http://hz.sweek.top/gtyydlxcgv.html

#include <iostream>
来源：http://hz.yanxiufei.cn/gtlwclnjje.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xingfuxueyuan.xyz/gtmxmxbobs.html

[S32] C++：字符串
来源：http://hz.zhixingplan.top/gtwacgvxwb.html

std::string s = "hi";  s += "!";
来源：http://hz.jinqigufen.top/gtllclfyko.html

[S33] C++：vector 增删
来源：http://hz.haohaochexian.top/gtvbrbugiy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.aizwys.cn/gtptfmeqme.html

[S34] C++：遍历 vector
来源：http://hz.pengpengdd.cyou/gtbtmxwkov.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yonumen.top/gthswbpbvu.html

[S35] C++：map
来源：http://hz.316326.xyz/gtctxvbwav.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yongpay.top/gtbbpfcjdq.html

[S36] C++：unordered_map
来源：http://hz.wangshuangyany.cn/gtekkdwlbi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aibaodan.cn/gtnviccaey.html

[S37] C++：set
来源：http://hz.bjfxy.top/gthnfndomg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhongyouzk.top/gtncrmdcfe.html

[S38] C++：排序
来源：http://hz.fzhhl.top/gtimnhfxgg.html

std::sort(v.begin(), v.end());
来源：http://hz.mhx1999.top/gtacoofwqc.html

[S39] C++：自定义比较器排序
来源：http://hz.havefunace.top/gtzwymigen.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.wangdashe.top/gtokospjaj.html

[S40] C++：查找元素
来源：http://hz.hnqzz.top/gtbdgtfqfc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.havefunace.top/gtjmzdkfmt.html

[S41] C++：类与构造函数
来源：http://hz.yvedp.cn/gtkbdlctuk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ivvv.top/gtrrpntkrf.html

[S42] C++：继承与虚函数
来源：http://hz.sysykeji.top/gtbllomcir.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenzaomai.com/gtbxdarwng.html

[S43] C++：智能指针
来源：http://hz.chenlongwang.top/gtxutgpcua.html

auto p = std::make_unique<int>(5);
来源：http://hz.cheryme.top/gtrelwlmwi.html

[S44] C++：引用传参
来源：http://hz.shzxlz.cn/gtozfddvwy.html

void inc(int &x) { ++x; }
来源：http://hz.tian-w.cn/gtsfmphfir.html

[S45] C++：lambda
来源：http://hz.zhiwuduotai.top/gtdwkqspav.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jianghu66.top/gtoyddyvzp.html

[S46] C++：函数模板
来源：http://hz.meibo888.top/gtdwbogfvn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gzhubu.top/gtbvfoszaw.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhijiandao.cn/gtsxbaiyso.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.aizwys.cn/gtfwjytury.html

[S48] C++：逐行读文件
来源：http://hz.cucudq.cn/gtyiqsidll.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yvedp.cn/gtwwpknhgb.html

while (std::getline(in, line)) { }
来源：http://hz.feifeiyinyue.top/gtfyosrvln.html

[S49] C++：写文件
来源：http://hz.aibaodan.cn/gthafjwldw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shanyushiyangtech.top/gtlomounrb.html

[S50] C++：格式化数字
来源：http://hz.zdqjudy.top/gtqvvxoffw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gzhubu.top/gtutrpokph.html

[S51] C++：显式类型转换
来源：http://hz.wangshuangyany.cn/gtiqecwjhe.html

static_cast<double>(a) / b
来源：http://hz.svipenyu.cn/gtcoueqrky.html

[S52] C++：const 与 noexcept
来源：http://hz.chenjidiqi.icu/gtqkwdomxa.html

int size() const noexcept { return n_; }
来源：http://hz.svipenyu.cn/gtfmjqqkch.html

[S53] C++：移动语义
来源：http://hz.ywan-chungtsiang.top/gtvynnprri.html

std::vector<int> w = std::move(v);
来源：http://hz.shanyushiyangtech.top/gtpnsxoqpv.html

[S54] C++：异常处理
来源：http://hz.smart0.xyz/gtmkqtizmq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cucudq.cn/gtulwfzpsb.html

[S55] C++：结构化绑定
来源：http://hz.redwolf501.top/gtkmzdvxdp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shzxlz.cn/gtbmmcdtaz.html

[S56] C++：optional
来源：http://hz.fzhhl.top/gtcwifvbhg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.redwolf501.top/gtponxtwdy.html

[S57] C++：编译期常量
来源：http://hz.jqgufenzy.top/gtwxnhzisx.html

constexpr int N = 10;
来源：http://hz.meibo888.top/gtakpxzhhk.html

[S58] C++：命名空间
来源：http://hz.fengsongda.top/gtddpommpc.html

namespace ns { int f() { return 1; } }
来源：http://hz.yanxiufei.cn/gtrijwkccz.html

[S59] C++：静态断言
来源：http://hz.ehwqpu.com/gtqcqtvgip.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yanxiufei.cn/gthxxoermd.html

[S60] C++：遍历并删除元素
来源：http://hz.haohaochexian.top/gtpkqrgauq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yueranfly.top/gtkfopgbsg.html

================================================================================
来源：http://hz.shuidangran.top/gtocjwuulr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guowangkeji.top/gtbecznhuk.html

================================================================================
来源：http://hz.hnxiangtu.top/gtwnpsogun.html

[T01] Kotlin：Hello World
来源：http://hz.zhaomingkeji.xyz/gtkorndihh.html

println("Hello")
来源：http://hz.yvedp.cn/gtcnfleiiy.html

[T02] Kotlin：变量
来源：http://hz.xuanzx.com/gtuafxdxqp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhijiandao.cn/gtyyvzidas.html

[T03] Kotlin：字符串模板
来源：http://hz.jyoumei.cn/gtodabmhdh.html

"值: $b"
来源：http://hz.shanyushiyangtech.top/gtvfgzljki.html

[T04] Kotlin：空安全
来源：http://hz.hammf.cn/gtephgktsz.html

val n: String? = null;  n?.length
来源：http://hz.jianghu66.top/gtuzrjwzrc.html

[T05] Kotlin：when 表达式
来源：http://hz.xuanzx.com/gtfpxgamre.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gaohongyu789.top/gtmtjoscgi.html

[T06] Kotlin：集合映射
来源：http://hz.kuanghao11.cn/gtemxyumvx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.316326.xyz/gtntkchzga.html

[T07] Kotlin：集合过滤
来源：http://hz.yanxiufei.cn/gtydgpdhpd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xinyue.icu/gtetfdcehl.html

[T08] Kotlin：数据类
来源：http://hz.nanxinkj.top/gtlmszvkwx.html

data class User(val name: String, val age: Int)
来源：http://hz.kuanghao11.cn/gtklntolqd.html

[T09] Kotlin：扩展函数
来源：http://hz.hammf.cn/gtqcrycyqs.html

fun String.exclaim() = this + "!"
来源：http://hz.jyoumei.cn/gtnlwupvla.html

[T10] Kotlin：默认参数
来源：http://hz.cdnleiting.top/gtutnzjlyi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yonumen.top/gtdtizzhjh.html

[T11] Kotlin：协程
来源：http://hz.316326.xyz/gthscrwesn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhiwuduotai.top/gtmhpuapjx.html

[T12] Kotlin：解构声明
来源：http://hz.cheryme.top/gtdjrcebtd.html

val (a, b) = Pair(1, 2)
来源：http://hz.andypj.xyz/gtumzsssma.html

[T13] Kotlin：只读 Map
来源：http://hz.xinyue.icu/gtjileznzx.html

val m = mapOf("a" to 1)
来源：http://hz.tianlin.xyz/gtembgzbtf.html

[T14] Kotlin：循环
来源：http://hz.ydzc1.top/gtzdjmgqen.html

for (i in 1..10) println(i)
来源：http://hz.guowangkeji.top/gtmsnxlmtp.html

[T15] Kotlin：接口
来源：http://hz.aibaodan.cn/gtoqiapaqp.html

interface Shape { fun area(): Double }
来源：http://hz.yj20258888.top/gtuljcjzds.html

[T16] Swift：Hello World
来源：http://hz.yj20258888.top/gtzvuldosy.html

print("Hello")
来源：http://hz.hongshengwenyu.top/gtqeshzsbf.html

[T17] Swift：变量与常量
来源：http://hz.xuetiantiany.cn/gtkwbsrkup.html

var a = 1;  let b = 2
来源：http://hz.xylfe.cn/gtmzwkjotw.html

[T18] Swift：字符串插值
来源：http://hz.sysykeji.top/gtpbduvnzi.html

"值: \(b)"
来源：http://hz.guowangkeji.top/gtgsapcusx.html

[T19] Swift：可选绑定
来源：http://hz.zhixingplan.top/gtqoaynfih.html

if let n = opt { print(n) }
来源：http://hz.aibaodan.cn/gtjpjctijx.html

[T20] Swift：数组操作
来源：http://hz.nwbrower.top/gtefxdcyhy.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.tianlin.xyz/gthbsnppam.html

[T21] Swift：遍历
来源：http://hz.bjfxy.top/gtjryspnyx.html

for x in a { print(x) }
来源：http://hz.sweek.top/gtxlrtlbba.html

[T22] Swift：字典
来源：http://hz.cdnleiting.top/gtbcjpjgbi.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yangfankeji.com/gtfzfwczie.html

[T23] Swift：函数
来源：http://hz.nanxinkj.top/gtiikqhcrq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yuxming.cn/gteorqbnmx.html

[T24] Swift：闭包
来源：http://hz.daxiang520.top/gtueydbwmt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zdqjudy.top/gtpcqldbvx.html

[T25] Swift：结构体
来源：http://hz.jqgufenzy.top/gtkgwjytsf.html

struct P { var x: Int }
来源：http://hz.zycfv.cn/gtlujkzige.html

[T26] Swift：类与重写
来源：http://hz.yuanzhike.top/gtdqomezrj.html

class A: Base { override func f() {} }
来源：http://hz.jlsjyb.cn/gtjyqydgwm.html

[T27] Swift：错误处理
来源：http://hz.zhixingplan.top/gtztaggkle.html

do { try f() } catch { print(error) }
来源：http://hz.tian-w.cn/gtsaefpnmx.html

[T28] Swift：枚举
来源：http://hz.chenjidiqi.icu/gtxeglbpyy.html

enum Color { case red, green }
来源：http://hz.jyoumei.cn/gtbktnqyff.html

[T29] Swift：guard 提前返回
来源：http://hz.sufxvd.cn/gtswslfrhu.html

guard let x = opt else { return }
来源：http://hz.sweek.top/gtwjttppcf.html

[T30] Swift：协议
来源：http://hz.xylfe.cn/gtqoxkmsfn.html

protocol Shape { func area() -> Double }
来源：http://hz.xylfe.cn/gtdnraoakr.html

[T31] Lua：Hello World
来源：http://hz.nwbrower.top/gtdxmekzks.html

print("Hello")
来源：http://hz.shangyingyoupin.top/gtybtvijtv.html

[T32] Lua：局部变量
来源：http://hz.yuxming.cn/gtexhihqdb.html

local a = 1
来源：http://hz.yj202588.top/gteujbxuoe.html

[T33] Lua：表（数组）
来源：http://hz.sweek.top/gtjhghzgri.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shzxlz.cn/gtlohevqhl.html

[T34] Lua：遍历表
来源：http://hz.cqqwz.cn/gtybzzuyso.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.iojbl.cn/gtwqwjxejw.html

[T35] Lua：字典表
来源：http://hz.pengpengdd.cyou/gtcezbilgy.html

local d = { a = 1 };  d.b = 2
来源：http://hz.sufxvd.cn/gtthppowas.html

[T36] Lua：函数
来源：http://hz.jinqigufen.top/gtywgkytxv.html

function add(a, b) return a + b end
来源：http://hz.pengpengdd.cyou/gtbrbsfoeg.html

[T37] Lua：字符串拼接
来源：http://hz.zycfv.cn/gtoltprgis.html

"a" .. "b"
来源：http://hz.gzhubu.top/gtghdetvkr.html

[T38] Lua：条件
来源：http://hz.mhx1999.top/gtyyqkifvo.html

if x > 0 then print("正") end
来源：http://hz.xylfe.cn/gtbddxcgls.html

[T39] Lua：模式匹配
来源：http://hz.c1oappe.top/gtmypgfyca.html

string.find(s, "%d+")
来源：http://hz.ehwqpu.com/gtbladkzho.html

[T40] Lua：元表
来源：http://hz.gzhubu.top/gtnrmkzzvf.html

setmetatable({}, { __index = base })
来源：http://hz.jyoumei.cn/gtfouttmfg.html

[T41] Perl：Hello World
来源：http://hz.yonumen.top/gtynisqqso.html

print "Hello\n";
来源：http://hz.mhx1999.top/gtzaywcazt.html

[T42] Perl：变量类型
来源：http://hz.xziqi.cn/gtgckimcjr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shanyushiyangtech.top/gtibuprfrf.html

[T43] Perl：字符串插值
来源：http://hz.yj202588.top/gtplhcsxbc.html

"值: $a"
来源：http://hz.zhongyouzk.top/gtoszxeprb.html

[T44] Perl：条件
来源：http://hz.svipenyu.cn/gtflmnlqha.html

if ($a > 0) { print "正"; }
来源：http://hz.fengsongda.top/gtrstjppze.html

[T45] Perl：数组遍历
来源：http://hz.fzhhl.top/gtcfdsupgu.html

for my $x (@arr) { print $x; }
来源：http://hz.sufxvd.cn/gtggfnqrsi.html

[T46] Perl：哈希操作
来源：http://hz.hammf.cn/gtiqgkuxum.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ivvv.top/gtdofrbdym.html

[T47] Perl：正则捕获
来源：http://hz.zhiwuduotai.top/gtljlbnphi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinqigufen.top/gtpgooapqy.html

[T48] Perl：正则替换
来源：http://hz.52xcode.cn/gthdgqccac.html

$s =~ s/old/new/g;
来源：http://hz.jinqigfzy.top/gtextvqven.html

[T49] Perl：函数
来源：http://hz.redwolf501.top/gtzthjtbbw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yanxiufei.cn/gtantemfsn.html

[T50] Perl：逐行读文件
来源：http://hz.andypj.xyz/gtcavrihkw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jyoumei.cn/gttboroega.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.smart0.xyz/gteecskzjw.html

[T51] Scala：Hello World
来源：http://hz.shanyushiyangkeji.top/gtemtnxzaf.html

println("Hello")
来源：http://hz.chenzaomai.com/gtknybpfho.html

[T52] Scala：变量
来源：http://hz.cheryme.top/gtqdzwctpn.html

val a = 1;  var b = 2
来源：http://hz.9152youxi.cn/gtvrhbbtvz.html

[T53] Scala：字符串插值
来源：http://hz.ivvv.top/gteugtwhxc.html

s"值: $b"
来源：http://hz.aibaodan.cn/gtpkqvotho.html

[T54] Scala：集合映射
来源：http://hz.ppjwa.cn/gtakdrdpfw.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.kuanghao11.cn/gtzkbjjppa.html

[T55] Scala：集合过滤
来源：http://hz.ppjwa.cn/gtrvcgypxg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.smart0.xyz/gtuzbzukxn.html

[T56] Scala：样例类
来源：http://hz.zhoulong.xyz/gtwclyfsgg.html


<!-- 参考信息 -->