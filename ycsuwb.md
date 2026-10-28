代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.52xcode.cn/gtpchlajsh.html

[R36] 并发执行多个任务
来源：http://hz.cqqwz.cn/gtkdrwbxfq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xingfuxueyuan.xyz/gtplsbdbzx.html

[R37] 把输出赋给变量
来源：http://hz.tanke756.top/gtaqeqsxog.html

files=$(ls -1)
来源：http://hz.jinyuanbaomall.cn/gtewvtozxm.html

[R38] 管道串联
来源：http://hz.andypj.xyz/gtyqgsszbm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ydzc1.top/gtbhckysek.html

[R39] 重定向标准输出与错误
来源：http://hz.ehwqpu.com/gtcedtdbno.html

cmd > out.log 2>&1
来源：http://hz.yangfankeji.com/gtfsenepmp.html

[R40] 追加写日志
来源：http://hz.fzhhl.top/gtttvzjkdt.html

echo "log" >> out.log
来源：http://hz.52xcode.cn/gtdghqgtvo.html

[R41] 丢弃输出
来源：http://hz.jianghu66.top/gtfweksdoh.html

cmd >/dev/null 2>&1
来源：http://hz.dianchejie.cn/gtacfvgydg.html

[R42] 输入重定向
来源：http://hz.cheryme.top/gtieuamunt.html

wc -l < a.txt
来源：http://hz.sxryk.cn/gtbjlceafs.html

[R43] 按名字查找文件
来源：http://hz.jianghu66.top/gtxwwfexfu.html

find . -name "*.log" -type f
来源：http://hz.jiagoushi.top/gtbltueljr.html

[R44] 按修改时间查找
来源：http://hz.fengsongda.top/gtoaptapsu.html

find . -mtime -7 -type f
来源：http://hz.ydzc1.top/gtfszelfyj.html

[R45] 批量删除
来源：http://hz.smart0.xyz/gtyrukiphl.html

find . -name "*.tmp" -delete
来源：http://hz.cdnleiting.top/gthsmhpecs.html

[R46] 递归替换文件内容
来源：http://hz.jinyuanbaomall.cn/gtnrwrqemz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258.top/gtumgdchwb.html

[R47] sed 单行替换
来源：http://hz.chenlongwang.top/gtifspvzrp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.daxiang520.top/gtnpmizxse.html

[R48] awk 取指定列
来源：http://hz.yuanzhike.top/gthmhqolkw.html

awk '{print $1, $3}' a.txt
来源：http://hz.nwbrower.top/gtrfjskjtu.html

[R49] awk 带条件
来源：http://hz.feifeiyinyue.top/gtyjqlcsgk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xuanzx.com/gtiagdrqeo.html

[R50] awk 求和
来源：http://hz.xziqi.cn/gthoojjovj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinqigufen.top/gtgdhqeiom.html

[R51] 排序去重取前几
来源：http://hz.jiagoushi.top/gtiboneeqw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhoulong.xyz/gtfaxtyjnx.html

[R52] 统计行数
来源：http://hz.yuxming.cn/gtxdsmobus.html

wc -l a.txt
来源：http://hz.52xcode.cn/gtnyddoebb.html

[R53] 查看文件头与实时尾
来源：http://hz.sufxvd.cn/gtkhrlkqho.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yongpay.top/gtlizlmoml.html

[R54] 比较两个文件
来源：http://hz.gotoacloud.top/gtchalmbez.html

diff a.txt b.txt
来源：http://hz.yuanzhike.top/gtcpwshunk.html

[R55] 压缩与解压
来源：http://hz.hysaishi.cn/gtglgmrrlq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenlongwang.top/gttrcbyzcw.html

[R56] 远程拷贝
来源：http://hz.dianchejie.cn/gthlqzlbmx.html

scp file user@host:/path/
来源：http://hz.tian-w.cn/gtxcahyqiy.html

[R57] 远程执行命令
来源：http://hz.gaohongyu789.top/gtorphqvzp.html

ssh user@host 'uptime'
来源：http://hz.yueranfly.top/gtmtoluyyl.html

[R58] 下载文件
来源：http://hz.vqdsnc.cn/gtmpenolth.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shanyushiyangtech.top/gtawibzkbv.html

[R59] 发 POST JSON
来源：http://hz.zhengqikj.top/gtzpjdvsqu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.guannengcc.top/gthipkubsi.html

[R60] 只看 HTTP 状态码
来源：http://hz.dianchejie.cn/gtdoydwypz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yuxming.cn/gtqmkpkilp.html

[R61] 磁盘占用
来源：http://hz.mhx1999.top/gtsgrmztuq.html

df -h;  du -sh *
来源：http://hz.redwolf501.top/gtamcpqiii.html

[R62] 找最占空间的文件
来源：http://hz.zhengqikj.top/gtvdvkwmab.html

du -ah . | sort -rh | head -10
来源：http://hz.vqdsnc.cn/gttiphhvsy.html

[R63] 内存与进程
来源：http://hz.daxiang520.top/gtlzshatld.html

free -h;  ps aux | grep nginx
来源：http://hz.nanxinkj.top/gtuzcghfmr.html

[R64] 结束进程
来源：http://hz.yvedp.cn/gtmfharmda.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gzhubu.top/gtmsyjjmbq.html

[R65] 查看端口占用
来源：http://hz.yangfankeji.com/gtcafwaodj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.pycfn.com/gtiijzyeuy.html

[R66] 定时任务
来源：http://hz.yj20258888.top/gtuuuzwmfr.html

crontab -e;  crontab -l
来源：http://hz.nwbrower.top/gtgomttwdn.html

[R67] 生成随机十六进制串
来源：http://hz.pycfn.com/gtgrcwzxgp.html

openssl rand -hex 16
来源：http://hz.pengpengdd.cyou/gtrwvezbcq.html

[R68] 计算文件校验值
来源：http://hz.sysykeji.top/gtwclteaim.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ehwqpu.com/gtyualtkpz.html

[R69] 生成随机密码
来源：http://hz.daxiang520.top/gtmbrvxeyd.html

head -c 16 /dev/urandom | base64
来源：http://hz.sysykeji.top/gtavobndyl.html

[R70] 时间戳与互转
来源：http://hz.cdnleiting.top/gtxwbxxyvm.html

date +%s;  date -d @1700000000
来源：http://hz.yuanzhike.top/gtsijyjobb.html

[R71] 日期格式化
来源：http://hz.yj20258.top/gtaomwdlod.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.feifeiyinyue.top/gttufqdxzl.html

[R72] 等待端口就绪
来源：http://hz.xinyue.icu/gtiwunhywu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.kuanghao11.cn/gtcoriivmt.html

[R73] 分割大日志
来源：http://hz.pengpengdd.cyou/gtmtinnoxr.html

split -l 1000 big.log part_
来源：http://hz.shuidangran.top/gtrqdyqiap.html

[R74] 批量重命名
来源：http://hz.316326.xyz/gtuehaaxge.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.haohaochexian.top/gtxeqtusmu.html

[R75] 导出环境变量
来源：http://hz.xinyue.icu/gtazqrhhso.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gaohongyu789.top/gtxymvhakx.html

[R76] 使用临时文件
来源：http://hz.bjfxy.top/gtcwgfljje.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shuidangran.top/gtgdbwqtae.html

[R77] 读取用户输入
来源：http://hz.yangfankeji.com/gtsqwmfjpo.html

read -rp "请输入: " ans
来源：http://hz.guannengcc.top/gtzpfjpuiz.html

[R78] 交互式菜单
来源：http://hz.hysaishi.cn/gtbhsxdtnx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.snrcjt.cn/gtmarddxof.html

[R79] 解析命令行选项
来源：http://hz.iojbl.cn/gtuskxyolv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yuanzhike.top/gtpzfkmjws.html

[R80] 查看脚本执行耗时
来源：http://hz.shangyingyoupin.top/gtnqjublia.html

time ./run.sh
来源：http://hz.zhiwuduotai.top/gtgybgimgu.html

================================================================================
来源：http://hz.dashuyun.cn/gtzbtknmxx.html

S. C / C++ 专题
来源：http://hz.feifeiyinyue.top/gtlpyxqjnc.html

================================================================================
来源：http://hz.hnqzz.top/gtzrfazgyn.html

[S01] C：Hello World
来源：http://hz.cqqwz.cn/gtwuwwaakg.html

#include <stdio.h>
来源：http://hz.yongpay.top/gtshuedrqk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jianghu66.top/gtlsilxlch.html

[S02] C：变量与格式化输出
来源：http://hz.andypj.xyz/gtkqejrpfb.html

int a = 10; printf("%d\n", a);
来源：http://hz.zycfv.cn/gtwpuxvhjp.html

[S03] C：读入整数
来源：http://hz.tanke756.top/gtdovwgbhj.html

int x; scanf("%d", &x);
来源：http://hz.jinyuanbaomall.cn/gtydivikla.html

[S04] C：字符串复制
来源：http://hz.havefunace.top/gtvkqtngyx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.daria6918.cn/gtrbfedauj.html

[S05] C：字符串长度
来源：http://hz.yj20258888.top/gtqjlugtqq.html

strlen(s)
来源：http://hz.quarkkingdee.top/gtjkcrzzls.html

[S06] C：字符串比较
来源：http://hz.pengpengdd.cyou/gtbdljcpnx.html

strcmp(a, b) == 0
来源：http://hz.sxryk.cn/gtgupqoemf.html

[S07] C：数组遍历求和
来源：http://hz.yanxiufei.cn/gtzkfpdhka.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xuanzx.com/gtqxcikifx.html

[S08] C：动态内存分配与释放
来源：http://hz.feifeiyinyue.top/gtysyjlbdn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hongshengwenyu.top/gtzwehigvz.html

[S09] C：结构体定义与初始化
来源：http://hz.sweek.top/gtluexqkhm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj20258.top/gtlrtwsvsk.html

[S10] C：指针与解引用
来源：http://hz.zycfv.cn/gtclpriccq.html

int *p = &a;  *p = 5;
来源：http://hz.chenjidiqi.icu/gtmeggtoog.html

[S11] C：逐行读文件
来源：http://hz.cdnleiting.top/gtvihaajlc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.bjfxy.top/gtginzsywo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.daxiang520.top/gtzosmjrwv.html

fclose(f);
来源：http://hz.havefunace.top/gtprjqdjci.html

[S12] C：写文件
来源：http://hz.havefunace.top/gtukchpiex.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xingfuxueyuan.xyz/gtmywgdhta.html

[S13] C：宏定义
来源：http://hz.fzhhl.top/gtdivwmeur.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhiwuduotai.top/gtyokaqfmz.html

[S14] C：枚举
来源：http://hz.hywenlv.cn/gtufkfiepe.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.andypj.xyz/gtjjdiolgk.html

[S15] C：类型转换
来源：http://hz.sxryk.cn/gtliilgqec.html

(double) a / b
来源：http://hz.nanxinkj.top/gtpmevzmoh.html

[S16] C：位操作置位
来源：http://hz.aizwys.cn/gtwkwiakog.html

x |= (1 << 3);
来源：http://hz.zhongyouzk.top/gtrgoomfth.html

[S17] C：安全拼接字符串
来源：http://hz.wangshuangyany.cn/gtsrdkocpl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.pengpengdd.cyou/gtpamyalsf.html

[S18] C：命令行参数
来源：http://hz.fzhhl.top/gtxorbsvmu.html

int main(int argc, char **argv)
来源：http://hz.cdnleiting.top/gtpfgxbrfb.html

[S19] C：快速排序
来源：http://hz.jinqigfzy.top/gtkihcaydj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.c1oappe.top/gtjplmfhiw.html

[S20] C：二分查找
来源：http://hz.cucudq.cn/gtjsvekpfn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xuetiantiany.cn/gtovsglbsd.html

[S21] C：字符类别判断
来源：http://hz.bjfxy.top/gtwohcvdvz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.wangdashe.top/gtixvsjinr.html

[S22] C：字符串转数字
来源：http://hz.svipenyu.cn/gtsgqrpood.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.316326.xyz/gtajdiujpz.html

[S23] C：随机数
来源：http://hz.aizwys.cn/gtleiqgegg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.birdmap.top/gtbhxzqfum.html

[S24] C：获取本地时间
来源：http://hz.gotoacloud.top/gtarkvabva.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.fengsongda.top/gtkebsxysr.html

[S25] C：内存拷贝
来源：http://hz.feifeiyinyue.top/gteodujdrv.html

memcpy(dst, src, n);
来源：http://hz.kuanghao11.cn/gtiarxangz.html

[S26] C：内存清零
来源：http://hz.tianlin.xyz/gtktmytemj.html

memset(a, 0, sizeof a);
来源：http://hz.yueranfly.top/gtyxbmlthh.html

[S27] C：定义常量
来源：http://hz.gogol.net.cn/gtythvzmsc.html

const double PI = 3.14159;
来源：http://hz.snrcjt.cn/gthdabkchp.html

[S28] C：静态变量
来源：http://hz.zhaomingkeji.xyz/gtltffseru.html

static int counter = 0;
来源：http://hz.chenjidiqi.icu/gtfhjetmtz.html

[S29] C：变参函数
来源：http://hz.shuidangran.top/gtqnlwfzkd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.andypj.xyz/gtgwqewwdf.html

[S30] C：头文件保护
来源：http://hz.jqgfzy.top/gtbgmlibrh.html

#ifndef X_H
来源：http://hz.jianghu66.top/gtdbsoywxi.html

#define X_H
来源：http://hz.zhongyouzk.top/gtlnlvckvb.html

#endif
来源：http://hz.yj20258.top/gtxcbqpdia.html

[S31] C++：Hello World
来源：http://hz.daxiang520.top/gtxtsvyngh.html

#include <iostream>
来源：http://hz.svipenyu.cn/gtrqxmbrsb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yangfankeji.com/gtlapmglfy.html

[S32] C++：字符串
来源：http://hz.zhijiandao.cn/gtzaahzbjl.html

std::string s = "hi";  s += "!";
来源：http://hz.guannengcc.top/gtzuxcgigk.html

[S33] C++：vector 增删
来源：http://hz.bjfxy.top/gtujivlnqz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ywan-chungtsiang.top/gtcnfqeczc.html

[S34] C++：遍历 vector
来源：http://hz.xuanzx.com/gtfnqptaqz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fzhhl.top/gtenijbhin.html

[S35] C++：map
来源：http://hz.dashuyun.cn/gtxhrfhysh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dianchejie.cn/gtsjuadfqm.html

[S36] C++：unordered_map
来源：http://hz.ivvv.top/gtnzwnmmyz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cqqwz.cn/gtosjasyac.html

[S37] C++：set
来源：http://hz.yj20258888.top/gteqvzxdcv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuetiantiany.cn/gtokpnctfx.html

[S38] C++：排序
来源：http://hz.pengpengdd.cyou/gtcacnhnju.html

std::sort(v.begin(), v.end());
来源：http://hz.zhengqikj.top/gtnlqvnmqo.html

[S39] C++：自定义比较器排序
来源：http://hz.cashguo.top/gtamktolqq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhijiandao.cn/gtiiuywaeg.html

[S40] C++：查找元素
来源：http://hz.guannengcc.top/gtoxskhtts.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.c1oappe.top/gtlsbuafxy.html

[S41] C++：类与构造函数
来源：http://hz.zhengqikj.top/gtqkdxyilh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xingfuxueyuan.xyz/gtkszptizt.html

[S42] C++：继承与虚函数
来源：http://hz.yj20258888.top/gtpkwuaujw.html

class B : public Base { public: void f() override {} };
来源：http://hz.sxryk.cn/gtzhbybezf.html

[S43] C++：智能指针
来源：http://hz.dashuyun.cn/gtetnlsvam.html

auto p = std::make_unique<int>(5);
来源：http://hz.fzhhl.top/gtpocproqg.html

[S44] C++：引用传参
来源：http://hz.jqgufenzy.top/gtbspzihej.html

void inc(int &x) { ++x; }
来源：http://hz.pycfn.com/gtzrwigypp.html

[S45] C++：lambda
来源：http://hz.yuxming.cn/gtcuudcmgh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.tian-w.cn/gtametozoy.html

[S46] C++：函数模板
来源：http://hz.jqgufenzy.top/gtwttjpylq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yvedp.cn/gtkdfsysgk.html

[S47] C++：结构化绑定遍历
来源：http://hz.meibo888.top/gthxsvbhqt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinqigfzy.top/gtkqtggmok.html

[S48] C++：逐行读文件
来源：http://hz.pengpengdd.cyou/gtiihsufqg.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.wangshuangyany.cn/gtlqesbsof.html

while (std::getline(in, line)) { }
来源：http://hz.xylfe.cn/gtpetihrip.html

[S49] C++：写文件
来源：http://hz.chenjidiqi.icu/gtbcwmjdmc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydzc1.top/gtxxkxziel.html

[S50] C++：格式化数字
来源：http://hz.ehwqpu.com/gtqwtevuec.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yonumen.top/gtwujqdham.html

[S51] C++：显式类型转换
来源：http://hz.guannengcc.top/gtntxbrwry.html

static_cast<double>(a) / b
来源：http://hz.sufxvd.cn/gtzdtxtpza.html

[S52] C++：const 与 noexcept
来源：http://hz.hnxiangtu.top/gtumhbbsbk.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258.top/gtejiozjkh.html

[S53] C++：移动语义
来源：http://hz.pycfn.com/gthpqevemp.html

std::vector<int> w = std::move(v);
来源：http://hz.feifeiyinyue.top/gtehuzrdjo.html

[S54] C++：异常处理
来源：http://hz.havefunace.top/gtsgdmniqf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhaomingkeji.xyz/gtpztwvlrr.html

[S55] C++：结构化绑定
来源：http://hz.xuanzx.com/gteeghnxud.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hnqzz.top/gttdstyuwd.html

[S56] C++：optional
来源：http://hz.zycfv.cn/gtzyaaqrww.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.c1oappe.top/gtznxcfacl.html

[S57] C++：编译期常量
来源：http://hz.guowangkeji.top/gtmlguqsug.html

constexpr int N = 10;
来源：http://hz.yueranfly.top/gtidjjrtuz.html

[S58] C++：命名空间
来源：http://hz.sxryk.cn/gtycajxtwj.html

namespace ns { int f() { return 1; } }
来源：http://hz.gzhubu.top/gtrsthkawp.html

[S59] C++：静态断言
来源：http://hz.sysykeji.top/gtnzxsarip.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.daxiang520.top/gtdeefbnkf.html

[S60] C++：遍历并删除元素
来源：http://hz.iojbl.cn/gthbrnmkqc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.dashuyun.cn/gtfavmcujq.html

================================================================================
来源：http://hz.cheryme.top/gtifnamyoa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pycfn.com/gtowljotsn.html

================================================================================
来源：http://hz.sufxvd.cn/gtxqvmbvqi.html

[T01] Kotlin：Hello World
来源：http://hz.yangfankeji.com/gteoaiedge.html

println("Hello")
来源：http://hz.zhongyouzk.top/gtnwaneezw.html

[T02] Kotlin：变量
来源：http://hz.nanxuanxn.top/gtvmktploh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yangfankeji.com/gtixuzuwoh.html

[T03] Kotlin：字符串模板
来源：http://hz.shangyingyoupin.top/gtmjqjrhtp.html

"值: $b"
来源：http://hz.tian-w.cn/gtomwzowuw.html

[T04] Kotlin：空安全
来源：http://hz.cdnleiting.top/gteurvcstv.html

val n: String? = null;  n?.length
来源：http://hz.mhx1999.top/gtykawcgfi.html

[T05] Kotlin：when 表达式
来源：http://hz.jyoumei.cn/gthcwbmvct.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenlongwang.top/gtpfheytiq.html

[T06] Kotlin：集合映射
来源：http://hz.zhongyouzk.top/gtlmqufyfd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nanxuanxn.top/gtsojvzlbm.html

[T07] Kotlin：集合过滤
来源：http://hz.ydjk.org.cn/gtwpriiziw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gogol.net.cn/gtbekffguq.html

[T08] Kotlin：数据类
来源：http://hz.nanxuanxn.top/gtwsmkrkdd.html

data class User(val name: String, val age: Int)
来源：http://hz.jianghu66.top/gtianntxsk.html

[T09] Kotlin：扩展函数
来源：http://hz.haohaochexian.top/gtcbtnggyu.html

fun String.exclaim() = this + "!"
来源：http://hz.ywan-chungtsiang.top/gtfijvnvlv.html

[T10] Kotlin：默认参数
来源：http://hz.haohaochexian.top/gttgqlrqdf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gaohongyu789.top/gthgmjzrjd.html

[T11] Kotlin：协程
来源：http://hz.hnqzz.top/gtvutolhzh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.wangdashe.top/gthwnhhira.html

[T12] Kotlin：解构声明
来源：http://hz.yanxiufei.cn/gtsnxtdlig.html

val (a, b) = Pair(1, 2)
来源：http://hz.sufxvd.cn/gtqatttfij.html

[T13] Kotlin：只读 Map
来源：http://hz.andypj.xyz/gthvykepxa.html

val m = mapOf("a" to 1)
来源：http://hz.chenlongwang.top/gtgaqkwjsy.html

[T14] Kotlin：循环
来源：http://hz.cucudq.cn/gtbkmbcllf.html

for (i in 1..10) println(i)
来源：http://hz.smart0.xyz/gtvjhyjwic.html

[T15] Kotlin：接口
来源：http://hz.fengsongda.top/gtlgqtkpyd.html

interface Shape { fun area(): Double }
来源：http://hz.wangdashe.top/gtmbovjiut.html

[T16] Swift：Hello World
来源：http://hz.yvedp.cn/gtybclmcmx.html

print("Hello")
来源：http://hz.haohaochexian.top/gtttruebsx.html

[T17] Swift：变量与常量
来源：http://hz.shzxlz.cn/gtgvmkjwzc.html

var a = 1;  let b = 2
来源：http://hz.nanxuanxn.top/gtttoiuykh.html

[T18] Swift：字符串插值
来源：http://hz.zhengqikj.top/gtljsmyrwm.html

"值: \(b)"
来源：http://hz.yj20258888.top/gtunidrbcv.html

[T19] Swift：可选绑定
来源：http://hz.guannengcc.top/gthemtrkcs.html

if let n = opt { print(n) }
来源：http://hz.shzxlz.cn/gtscbwqclb.html

[T20] Swift：数组操作
来源：http://hz.iojbl.cn/gtmfptmuix.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.bjfxy.top/gtfrtxvjjo.html

[T21] Swift：遍历
来源：http://hz.hysaishi.cn/gtzxuukybw.html

for x in a { print(x) }
来源：http://hz.snrcjt.cn/gtggxcuoub.html

[T22] Swift：字典
来源：http://hz.birdmap.top/gtpgeblgud.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenzaomai.com/gtvpnvgthi.html

[T23] Swift：函数
来源：http://hz.vqdsnc.cn/gtqytrhffb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hnqzz.top/gtdyexscdo.html

[T24] Swift：闭包
来源：http://hz.ppjwa.cn/gtdbqcbnal.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yuxming.cn/gtilfbwlgs.html

[T25] Swift：结构体
来源：http://hz.zdqjudy.top/gtnxjipeoh.html

struct P { var x: Int }
来源：http://hz.cheryme.top/gtsmawlwjw.html

[T26] Swift：类与重写
来源：http://hz.aizwys.cn/gtwdyacjvx.html

class A: Base { override func f() {} }
来源：http://hz.wangshuangyany.cn/gtzfyjkcvj.html

[T27] Swift：错误处理
来源：http://hz.hnqzz.top/gtlvqvwbrt.html

do { try f() } catch { print(error) }
来源：http://hz.yangfankeji.com/gtvsvqmxyf.html

[T28] Swift：枚举
来源：http://hz.yongpay.top/gtaacnvqkr.html

enum Color { case red, green }
来源：http://hz.jqgfzy.top/gtoqxscqvm.html

[T29] Swift：guard 提前返回
来源：http://hz.jinghuilouyu.cn/gtrhbjotbf.html

guard let x = opt else { return }
来源：http://hz.yongpay.top/gtfnbiokjl.html

[T30] Swift：协议
来源：http://hz.hammf.cn/gtevjyzcad.html

protocol Shape { func area() -> Double }
来源：http://hz.xuanzx.com/gtvagzvful.html

[T31] Lua：Hello World
来源：http://hz.gzhubu.top/gtkqoiximd.html

print("Hello")
来源：http://hz.wangshuangyany.cn/gtngnxvely.html

[T32] Lua：局部变量
来源：http://hz.yj20258888.top/gtwrmzbxkd.html

local a = 1
来源：http://hz.gotoacloud.top/gtxodmecwa.html

[T33] Lua：表（数组）
来源：http://hz.xuanzx.com/gtahrgftmd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jinqigufen.top/gtmfklsaqf.html

[T34] Lua：遍历表
来源：http://hz.yonumen.top/gtbaurufnw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhiwuduotai.top/gtbgpmnwuf.html

[T35] Lua：字典表
来源：http://hz.gaohongyu789.top/gtgdumalrk.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xinyue.icu/gtzqnhugfe.html

[T36] Lua：函数
来源：http://hz.zycfv.cn/gtqipwdyor.html

function add(a, b) return a + b end
来源：http://hz.pycfn.com/gthefofigu.html

[T37] Lua：字符串拼接
来源：http://hz.xziqi.cn/gtloiynpsg.html

"a" .. "b"
来源：http://hz.xinyue.icu/gtnwqxzrtw.html

[T38] Lua：条件
来源：http://hz.ppjwa.cn/gtmmdxjrlt.html

if x > 0 then print("正") end
来源：http://hz.havefunace.top/gtceilzafh.html


<!-- 参考信息 -->