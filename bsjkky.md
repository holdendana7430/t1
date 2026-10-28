代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nanxuanxn.top/gtwjurwdtn.html

[R48] awk 取指定列
来源：http://hz.xinyue.icu/gthyrbrqgi.html

awk '{print $1, $3}' a.txt
来源：http://hz.guowangkeji.top/gttnhxwctg.html

[R49] awk 带条件
来源：http://hz.jinqigfzy.top/gthvavoazw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.aizwys.cn/gtlavsyxoh.html

[R50] awk 求和
来源：http://hz.cashguo.top/gtjygecbum.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ydjk.org.cn/gtylfmykoq.html

[R51] 排序去重取前几
来源：http://hz.tanke756.top/gtleufpqoi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nanxuanxn.top/gtmjadofhu.html

[R52] 统计行数
来源：http://hz.zdqjudy.top/gtnhapuenw.html

wc -l a.txt
来源：http://hz.smart0.xyz/gtijeeztvg.html

[R53] 查看文件头与实时尾
来源：http://hz.jyoumei.cn/gtvzwsqqcp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.52xcode.cn/gtumoojpav.html

[R54] 比较两个文件
来源：http://hz.cqqwz.cn/gtycmacawx.html

diff a.txt b.txt
来源：http://hz.c1oappe.top/gttzmvqngf.html

[R55] 压缩与解压
来源：http://hz.dashuyun.cn/gtugaktrea.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yj202588.top/gtrswvnacb.html

[R56] 远程拷贝
来源：http://hz.zhaomingkeji.xyz/gtcypbwwab.html

scp file user@host:/path/
来源：http://hz.zhixingplan.top/gtchlnkhpv.html

[R57] 远程执行命令
来源：http://hz.zhijiandao.cn/gtznhujezt.html

ssh user@host 'uptime'
来源：http://hz.nanxinkj.top/gtonvyjurk.html

[R58] 下载文件
来源：http://hz.chenzaomai.com/gtdselxxwt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yangfankeji.com/gtripektiw.html

[R59] 发 POST JSON
来源：http://hz.316326.xyz/gtvvvxtpsq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.52xcode.cn/gttsfccpxc.html

[R60] 只看 HTTP 状态码
来源：http://hz.hywenlv.cn/gtweiqgcyp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yanxiufei.cn/gtbjhzkvxv.html

[R61] 磁盘占用
来源：http://hz.haohaochexian.top/gthivwmiao.html

df -h;  du -sh *
来源：http://hz.hnxiangtu.top/gtlxpcnrnz.html

[R62] 找最占空间的文件
来源：http://hz.pengpengdd.cyou/gtlpifmwny.html

du -ah . | sort -rh | head -10
来源：http://hz.fengsongda.top/gtcqnrvbue.html

[R63] 内存与进程
来源：http://hz.svipenyu.cn/gtddfqrlph.html

free -h;  ps aux | grep nginx
来源：http://hz.yuxming.cn/gtxtuvdwec.html

[R64] 结束进程
来源：http://hz.cashguo.top/gtcbmhldfg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xuetiantiany.cn/gtpyrijwfw.html

[R65] 查看端口占用
来源：http://hz.chenzaomai.com/gterpcrplq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jianghu66.top/gtvdbbflrl.html

[R66] 定时任务
来源：http://hz.birdmap.top/gtghnwzyox.html

crontab -e;  crontab -l
来源：http://hz.ydjk.org.cn/gtnzfvgjsy.html

[R67] 生成随机十六进制串
来源：http://hz.zhongyouzk.top/gtxyrwvccg.html

openssl rand -hex 16
来源：http://hz.zhixingplan.top/gtdtsqyepi.html

[R68] 计算文件校验值
来源：http://hz.jqgufenzy.top/gtkfalfwrb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhiwuduotai.top/gtjattntqt.html

[R69] 生成随机密码
来源：http://hz.hammf.cn/gtblirdnsh.html

head -c 16 /dev/urandom | base64
来源：http://hz.yuanzhike.top/gteaudqhdm.html

[R70] 时间戳与互转
来源：http://hz.sxryk.cn/gtwutujnpl.html

date +%s;  date -d @1700000000
来源：http://hz.chenzaomai.com/gtihjosflu.html

[R71] 日期格式化
来源：http://hz.andypj.xyz/gtxkjvzfyb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sxryk.cn/gtxmefowdw.html

[R72] 等待端口就绪
来源：http://hz.gaohongyu789.top/gtdrwtsbkf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.fengsongda.top/gtqwykicgj.html

[R73] 分割大日志
来源：http://hz.ehwqpu.com/gtprhmouyg.html

split -l 1000 big.log part_
来源：http://hz.yj20258888.top/gtjnddeetv.html

[R74] 批量重命名
来源：http://hz.guowangkeji.top/gtfpwxxwed.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zycfv.cn/gtenmoosfa.html

[R75] 导出环境变量
来源：http://hz.xziqi.cn/gtbkptisou.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.havefunace.top/gtdayarozh.html

[R76] 使用临时文件
来源：http://hz.wangdashe.top/gtsemwxgde.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.quarkkingdee.top/gtsvuabpgl.html

[R77] 读取用户输入
来源：http://hz.gaohongyu789.top/gtbrqmtpow.html

read -rp "请输入: " ans
来源：http://hz.iojbl.cn/gtzsnuiedl.html

[R78] 交互式菜单
来源：http://hz.xziqi.cn/gtcsrjktor.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nwbrower.top/gtlrkalgfr.html

[R79] 解析命令行选项
来源：http://hz.mhx1999.top/gtbsqmwfxn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinqigufen.top/gtfxavjycl.html

[R80] 查看脚本执行耗时
来源：http://hz.svipenyu.cn/gtkjtitiod.html

time ./run.sh
来源：http://hz.dianchejie.cn/gtiwclddll.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtswexukdo.html

S. C / C++ 专题
来源：http://hz.yangfankeji.com/gtlvmqlibn.html

================================================================================
来源：http://hz.cqqwz.cn/gtdcfkplsh.html

[S01] C：Hello World
来源：http://hz.chenzaomai.com/gtrugkkyjb.html

#include <stdio.h>
来源：http://hz.aizwys.cn/gtgsyyraxw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ydjk.org.cn/gtdifqmnpo.html

[S02] C：变量与格式化输出
来源：http://hz.jyoumei.cn/gtnqihwqlv.html

int a = 10; printf("%d\n", a);
来源：http://hz.hfpthk.cn/gtihfwlkce.html

[S03] C：读入整数
来源：http://hz.zdqjudy.top/gtbagjerys.html

int x; scanf("%d", &x);
来源：http://hz.xingfuxueyuan.xyz/gtlwhdcqvq.html

[S04] C：字符串复制
来源：http://hz.kuanghao11.cn/gtnfqntwmk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nwbrower.top/gtlbzluimn.html

[S05] C：字符串长度
来源：http://hz.zhixingplan.top/gtzrdkpetn.html

strlen(s)
来源：http://hz.zhijiandao.cn/gtvlivyvbc.html

[S06] C：字符串比较
来源：http://hz.yj20258.top/gtoldonxkz.html

strcmp(a, b) == 0
来源：http://hz.ppjwa.cn/gtyesaggrg.html

[S07] C：数组遍历求和
来源：http://hz.sxryk.cn/gtvqgtickp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.dianchejie.cn/gtmpayqfdl.html

[S08] C：动态内存分配与释放
来源：http://hz.xziqi.cn/gtzgmisnqd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhijiandao.cn/gtladygdsx.html

[S09] C：结构体定义与初始化
来源：http://hz.cheryme.top/gtcreszzlh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ivvv.top/gtblrdpyav.html

[S10] C：指针与解引用
来源：http://hz.guowangkeji.top/gtldmmxnyl.html

int *p = &a;  *p = 5;
来源：http://hz.tanke756.top/gttxqawkfx.html

[S11] C：逐行读文件
来源：http://hz.tian-w.cn/gtdwahculy.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hongshengwenyu.top/gtmvlllder.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sxryk.cn/gtrjnvniau.html

fclose(f);
来源：http://hz.yueranfly.top/gtfebomksq.html

[S12] C：写文件
来源：http://hz.jinqigfzy.top/gtfzrxyofm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhoulong.xyz/gtirxefvzg.html

[S13] C：宏定义
来源：http://hz.sufxvd.cn/gtpikhzaee.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.c1oappe.top/gtfrkungxu.html

[S14] C：枚举
来源：http://hz.sysykeji.top/gtraunslix.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.havefunace.top/gtripshcui.html

[S15] C：类型转换
来源：http://hz.redwolf501.top/gtgoxojnuq.html

(double) a / b
来源：http://hz.xuetiantiany.cn/gtswyslozv.html

[S16] C：位操作置位
来源：http://hz.dashuyun.cn/gtlzbpjths.html

x |= (1 << 3);
来源：http://hz.meibo888.top/gtmlrirydd.html

[S17] C：安全拼接字符串
来源：http://hz.zycfv.cn/gttgxahrta.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.pycfn.com/gtupwkhuaq.html

[S18] C：命令行参数
来源：http://hz.cheryme.top/gtucdusraf.html

int main(int argc, char **argv)
来源：http://hz.wangdashe.top/gteztbskza.html

[S19] C：快速排序
来源：http://hz.zycfv.cn/gtvqupveaj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jlsjyb.cn/gtbsyiblru.html

[S20] C：二分查找
来源：http://hz.jqgufenzy.top/gtquqnajqn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.c1oappe.top/gtjracudib.html

[S21] C：字符类别判断
来源：http://hz.quarkkingdee.top/gtnrqfohva.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.chenlongwang.top/gtnmxlfvim.html

[S22] C：字符串转数字
来源：http://hz.sysykeji.top/gtljlkuubu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xinyue.icu/gtmvndztoe.html

[S23] C：随机数
来源：http://hz.chenlongwang.top/gtmdokyxzr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xuetiantiany.cn/gtlectkmvu.html

[S24] C：获取本地时间
来源：http://hz.hnqzz.top/gtkpwkocfd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.vqdsnc.cn/gtgmjrmfuj.html

[S25] C：内存拷贝
来源：http://hz.hongshengwenyu.top/gtaoufrijs.html

memcpy(dst, src, n);
来源：http://hz.hnqzz.top/gtpogoirib.html

[S26] C：内存清零
来源：http://hz.zdqjudy.top/gthcwkcqqk.html

memset(a, 0, sizeof a);
来源：http://hz.shzxlz.cn/gtskqjwhtx.html

[S27] C：定义常量
来源：http://hz.jqgufenzy.top/gtozncecdc.html

const double PI = 3.14159;
来源：http://hz.quarkkingdee.top/gthhtvagme.html

[S28] C：静态变量
来源：http://hz.gzhubu.top/gtbcbjzdaq.html

static int counter = 0;
来源：http://hz.feifeiyinyue.top/gtkzwtskyg.html

[S29] C：变参函数
来源：http://hz.chenzaomai.com/gtvmtcykdt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.meibo888.top/gtwhefyxdw.html

[S30] C：头文件保护
来源：http://hz.ydzc1.top/gtxovfugjj.html

#ifndef X_H
来源：http://hz.shuidangran.top/gtocksfbds.html

#define X_H
来源：http://hz.chenjidiqi.icu/gtteandrjp.html

#endif
来源：http://hz.zhixingplan.top/gtppoppiwg.html

[S31] C++：Hello World
来源：http://hz.ywan-chungtsiang.top/gttyszgjfq.html

#include <iostream>
来源：http://hz.svipenyu.cn/gtzvoqeoaf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ivvv.top/gtpnrubgmf.html

[S32] C++：字符串
来源：http://hz.kuanghao11.cn/gtzakuomsw.html

std::string s = "hi";  s += "!";
来源：http://hz.sufxvd.cn/gtmijjkepn.html

[S33] C++：vector 增删
来源：http://hz.zdqjudy.top/gtnpmwpnay.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.pengpengdd.cyou/gtsfavihjc.html

[S34] C++：遍历 vector
来源：http://hz.smart0.xyz/gtlhnezgyr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cucudq.cn/gtyrwjisbt.html

[S35] C++：map
来源：http://hz.0kj1m.cn/gtkeuptjas.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.quarkkingdee.top/gtispplnhs.html

[S36] C++：unordered_map
来源：http://hz.9152youxi.cn/gtzunnvspr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gogol.net.cn/gttlvqorwr.html

[S37] C++：set
来源：http://hz.hnxiangtu.top/gtpqajmslu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenjidiqi.icu/gtgjkgrife.html

[S38] C++：排序
来源：http://hz.cqqwz.cn/gtfwdvedkx.html

std::sort(v.begin(), v.end());
来源：http://hz.gzhubu.top/gtrqrijzid.html

[S39] C++：自定义比较器排序
来源：http://hz.dashuyun.cn/gthdqobwjj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hfpthk.cn/gtjachsklr.html

[S40] C++：查找元素
来源：http://hz.yj202588.top/gtjwbxvvsn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jlsjyb.cn/gtgwkpkjqe.html

[S41] C++：类与构造函数
来源：http://hz.yj20258.top/gtmiidvcdc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.52xcode.cn/gtllykkfnl.html

[S42] C++：继承与虚函数
来源：http://hz.sysykeji.top/gtomcpshfr.html

class B : public Base { public: void f() override {} };
来源：http://hz.sweek.top/gtqmgquieh.html

[S43] C++：智能指针
来源：http://hz.cdnleiting.top/gtgezhpzma.html

auto p = std::make_unique<int>(5);
来源：http://hz.andypj.xyz/gtgaryvbim.html

[S44] C++：引用传参
来源：http://hz.sweek.top/gtbvjnywgr.html

void inc(int &x) { ++x; }
来源：http://hz.gogol.net.cn/gtuvpdqhxu.html

[S45] C++：lambda
来源：http://hz.jianghu66.top/gtqizlujjh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sysykeji.top/gtwwrinboa.html

[S46] C++：函数模板
来源：http://hz.zhengqikj.top/gtgacvxnof.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnxiangtu.top/gtelblazme.html

[S47] C++：结构化绑定遍历
来源：http://hz.shanyushiyangkeji.top/gtsvqjklwa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tian-w.cn/gtqkztgkgd.html

[S48] C++：逐行读文件
来源：http://hz.meibo888.top/gtxpeahkin.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sysykeji.top/gtdvtmhyxr.html

while (std::getline(in, line)) { }
来源：http://hz.shanyushiyangtech.top/gtjvedztlx.html

[S49] C++：写文件
来源：http://hz.xziqi.cn/gtnsahmckb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ywan-chungtsiang.top/gtibjrloeq.html

[S50] C++：格式化数字
来源：http://hz.jqgufenzy.top/gtelsqfgoj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhongyouzk.top/gtqvoocupz.html

[S51] C++：显式类型转换
来源：http://hz.guannengcc.top/gtzehwuchr.html

static_cast<double>(a) / b
来源：http://hz.sxryk.cn/gtppfyrnyr.html

[S52] C++：const 与 noexcept
来源：http://hz.tanke756.top/gtbysdgycw.html

int size() const noexcept { return n_; }
来源：http://hz.wangdashe.top/gtmqspqcvv.html

[S53] C++：移动语义
来源：http://hz.ydjk.org.cn/gtwgnisykb.html

std::vector<int> w = std::move(v);
来源：http://hz.tian-w.cn/gtquehhsag.html

[S54] C++：异常处理
来源：http://hz.sweek.top/gtnbfswmsi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jlsjyb.cn/gtgievffnn.html

[S55] C++：结构化绑定
来源：http://hz.yj202588.top/gtmnakykyb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.dianchejie.cn/gtejikeipc.html

[S56] C++：optional
来源：http://hz.sweek.top/gtkfkvwqhl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgufenzy.top/gtiuptvoca.html

[S57] C++：编译期常量
来源：http://hz.yj20258888.top/gtgohwkclb.html

constexpr int N = 10;
来源：http://hz.sxryk.cn/gtbkhpzfvw.html

[S58] C++：命名空间
来源：http://hz.wangdashe.top/gtdtelkrau.html

namespace ns { int f() { return 1; } }
来源：http://hz.hysaishi.cn/gtnuhceduh.html

[S59] C++：静态断言
来源：http://hz.smart0.xyz/gtcnpfmuda.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.feifeiyinyue.top/gthvujkydw.html

[S60] C++：遍历并删除元素
来源：http://hz.wangdashe.top/gtfofheqcn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.havefunace.top/gtvhjrnxuy.html

================================================================================
来源：http://hz.yj20258888.top/gtuhascdak.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cucudq.cn/gtwjlbqxgz.html

================================================================================
来源：http://hz.c1oappe.top/gtgcgkiesy.html

[T01] Kotlin：Hello World
来源：http://hz.birdmap.top/gtujwwifap.html

println("Hello")
来源：http://hz.shanyushiyangtech.top/gtpjfwjnbs.html

[T02] Kotlin：变量
来源：http://hz.xziqi.cn/gtegvjgdzl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.52xcode.cn/gtnxzwqxdl.html

[T03] Kotlin：字符串模板
来源：http://hz.zycfv.cn/gtiquathbq.html

"值: $b"
来源：http://hz.hfpthk.cn/gtxkzycwqd.html

[T04] Kotlin：空安全
来源：http://hz.sweek.top/gthqqbnlxr.html

val n: String? = null;  n?.length
来源：http://hz.yuxming.cn/gtdjpnupuo.html

[T05] Kotlin：when 表达式
来源：http://hz.xziqi.cn/gtvdfxeymb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.bjfxy.top/gtrdfkzwbb.html

[T06] Kotlin：集合映射
来源：http://hz.chenjidiqi.icu/gtnqpqdphb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yanxiufei.cn/gtvbvnkjtg.html

[T07] Kotlin：集合过滤
来源：http://hz.dashuyun.cn/gtjxjscexo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.fengsongda.top/gtrdsmkcgc.html

[T08] Kotlin：数据类
来源：http://hz.meibo888.top/gtztpcpfqm.html

data class User(val name: String, val age: Int)
来源：http://hz.zhoulong.xyz/gtzhpzbyfh.html

[T09] Kotlin：扩展函数
来源：http://hz.ywan-chungtsiang.top/gtkubledti.html

fun String.exclaim() = this + "!"
来源：http://hz.9152youxi.cn/gtwktdzvvw.html

[T10] Kotlin：默认参数
来源：http://hz.316326.xyz/gtvsfojosf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sweek.top/gtulsllcko.html

[T11] Kotlin：协程
来源：http://hz.hongshengwenyu.top/gtsarxmntj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.redwolf501.top/gttpqfaosh.html

[T12] Kotlin：解构声明
来源：http://hz.chenlongwang.top/gtwmbxvbmk.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenzaomai.com/gtxzoofvzu.html

[T13] Kotlin：只读 Map
来源：http://hz.andypj.xyz/gtwuljksbo.html

val m = mapOf("a" to 1)
来源：http://hz.zhiwuduotai.top/gtyhspzuox.html

[T14] Kotlin：循环
来源：http://hz.cqqwz.cn/gtbgdxbytj.html

for (i in 1..10) println(i)
来源：http://hz.jinqigfzy.top/gtagmudmct.html

[T15] Kotlin：接口
来源：http://hz.hysaishi.cn/gtkvrdbjlg.html

interface Shape { fun area(): Double }
来源：http://hz.chenlongwang.top/gtddlhnzbs.html

[T16] Swift：Hello World
来源：http://hz.hammf.cn/gtfewqwrut.html

print("Hello")
来源：http://hz.kuanghao11.cn/gtbpqudtuk.html

[T17] Swift：变量与常量
来源：http://hz.yongpay.top/gtutaerjke.html

var a = 1;  let b = 2
来源：http://hz.daxiang520.top/gtpsmsdaal.html

[T18] Swift：字符串插值
来源：http://hz.ppjwa.cn/gtpushxyak.html

"值: \(b)"
来源：http://hz.pengpengdd.cyou/gtkxrxfpro.html

[T19] Swift：可选绑定
来源：http://hz.0kj1m.cn/gtmdigfvpj.html

if let n = opt { print(n) }
来源：http://hz.ybcxt.top/gtsefkwxko.html

[T20] Swift：数组操作
来源：http://hz.xziqi.cn/gtkhpayogo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.aibaodan.cn/gtxdxvwigo.html

[T21] Swift：遍历
来源：http://hz.jinyuanbaomall.cn/gtuuhgviup.html

for x in a { print(x) }
来源：http://hz.guannengcc.top/gtpzqtjeeo.html

[T22] Swift：字典
来源：http://hz.daxiang520.top/gtabidkpvr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenjidiqi.icu/gtviiacvdi.html

[T23] Swift：函数
来源：http://hz.jinqigufen.top/gtxgxomsfy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ywan-chungtsiang.top/gtfoohrnsw.html

[T24] Swift：闭包
来源：http://hz.zdqjudy.top/gthndudotn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cqqwz.cn/gtwdknesyg.html

[T25] Swift：结构体
来源：http://hz.meibo888.top/gtnrqefxtp.html

struct P { var x: Int }
来源：http://hz.zhijiandao.cn/gtomwzxlmt.html

[T26] Swift：类与重写
来源：http://hz.316326.xyz/gtjdytisna.html

class A: Base { override func f() {} }
来源：http://hz.zhoulong.xyz/gtlceehgcy.html

[T27] Swift：错误处理
来源：http://hz.jinqigufen.top/gtxyxnoyza.html

do { try f() } catch { print(error) }
来源：http://hz.chenjidiqi.icu/gtdibntypa.html

[T28] Swift：枚举
来源：http://hz.sxryk.cn/gtysexlcpa.html

enum Color { case red, green }
来源：http://hz.andypj.xyz/gtikhedrgo.html

[T29] Swift：guard 提前返回
来源：http://hz.shangyingyoupin.top/gtmmlcticg.html

guard let x = opt else { return }
来源：http://hz.dashuyun.cn/gtwuvdgmpf.html

[T30] Swift：协议
来源：http://hz.zhiwuduotai.top/gtvmbbdzvi.html

protocol Shape { func area() -> Double }
来源：http://hz.yueranfly.top/gtnzovoisr.html

[T31] Lua：Hello World
来源：http://hz.hysaishi.cn/gtjvfxvjzh.html

print("Hello")
来源：http://hz.xuanzx.com/gteeeoyeqk.html

[T32] Lua：局部变量
来源：http://hz.jqgfzy.top/gtjxhzbjxv.html

local a = 1
来源：http://hz.chenjidiqi.icu/gtfhqrfyhl.html

[T33] Lua：表（数组）
来源：http://hz.zhongyouzk.top/gtlvxdaxcc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.quarkkingdee.top/gtzplusvcx.html

[T34] Lua：遍历表
来源：http://hz.yueranfly.top/gtpmeesxei.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.havefunace.top/gtievxaxff.html

[T35] Lua：字典表
来源：http://hz.yangfankeji.com/gtjkobfckc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xziqi.cn/gtxvhbnujk.html

[T36] Lua：函数
来源：http://hz.52xcode.cn/gtbhmllqvj.html

function add(a, b) return a + b end
来源：http://hz.zhiwuduotai.top/gtlumcisco.html

[T37] Lua：字符串拼接
来源：http://hz.hnxiangtu.top/gtahyaxwbq.html

"a" .. "b"
来源：http://hz.fengsongda.top/gtpeekvugx.html

[T38] Lua：条件
来源：http://hz.daria6918.cn/gtmewvhrsn.html

if x > 0 then print("正") end
来源：http://hz.quarkkingdee.top/gttrzmicms.html

[T39] Lua：模式匹配
来源：http://hz.aizwys.cn/gtyyuddqxu.html

string.find(s, "%d+")
来源：http://hz.gaohongyu789.top/gtbricevhr.html

[T40] Lua：元表
来源：http://hz.shanyushiyangkeji.top/gtmxgmzuth.html

setmetatable({}, { __index = base })
来源：http://hz.hysaishi.cn/gtihmaxrsd.html

[T41] Perl：Hello World
来源：http://hz.jqgufenzy.top/gtagjdpzxy.html

print "Hello\n";
来源：http://hz.vqdsnc.cn/gtxenfemwy.html

[T42] Perl：变量类型
来源：http://hz.sufxvd.cn/gtauevcncx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zdqjudy.top/gtqlnjznfk.html

[T43] Perl：字符串插值
来源：http://hz.xuanzx.com/gtlqdlsspx.html

"值: $a"
来源：http://hz.xinyue.icu/gtjmbtyyqd.html

[T44] Perl：条件
来源：http://hz.hywenlv.cn/gtdpfaxgyd.html

if ($a > 0) { print "正"; }
来源：http://hz.nwbrower.top/gtpuzjzabh.html

[T45] Perl：数组遍历
来源：http://hz.yuanzhike.top/gtpxgrguoc.html

for my $x (@arr) { print $x; }
来源：http://hz.jqgufenzy.top/gtkpmkmyir.html

[T46] Perl：哈希操作
来源：http://hz.yuxming.cn/gthuujfgez.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ydzc1.top/gtgcqacydu.html

[T47] Perl：正则捕获
来源：http://hz.nwbrower.top/gturodding.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.daria6918.cn/gtkfkfdpwp.html

[T48] Perl：正则替换
来源：http://hz.mhx1999.top/gtzfsktqtr.html

$s =~ s/old/new/g;
来源：http://hz.havefunace.top/gtkfdihtsn.html

[T49] Perl：函数
来源：http://hz.hysaishi.cn/gtemhwvirt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.chenzaomai.com/gteiwvhilb.html

[T50] Perl：逐行读文件
来源：http://hz.ybcxt.top/gtxmephuiq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cheryme.top/gtawrbfhhf.html


<!-- 参考信息 -->