代发 wailian999

files=$(ls -1)
来源：http://hz.zhoulong.xyz/gtuxhbmqiy.html

[R38] 管道串联
来源：http://hz.nwbrower.top/gtmnzawmds.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ydzc1.top/gtnslqjvgt.html

[R39] 重定向标准输出与错误
来源：http://hz.hnxiangtu.top/gtsqjxgxee.html

cmd > out.log 2>&1
来源：http://hz.smart0.xyz/gtqffhcimu.html

[R40] 追加写日志
来源：http://hz.dianchejie.cn/gtkogzhjjv.html

echo "log" >> out.log
来源：http://hz.jianghu66.top/gttclawrus.html

[R41] 丢弃输出
来源：http://hz.aibaodan.cn/gtcifsmjxi.html

cmd >/dev/null 2>&1
来源：http://hz.cheryme.top/gtjcoapevn.html

[R42] 输入重定向
来源：http://hz.tanke756.top/gtenwuvppz.html

wc -l < a.txt
来源：http://hz.smart0.xyz/gtygchbdwr.html

[R43] 按名字查找文件
来源：http://hz.svipenyu.cn/gtclirnjue.html

find . -name "*.log" -type f
来源：http://hz.daxiang520.top/gtjlvzavsv.html

[R44] 按修改时间查找
来源：http://hz.cashguo.top/gtfhvdfitn.html

find . -mtime -7 -type f
来源：http://hz.ydzc1.top/gtvfgspphd.html

[R45] 批量删除
来源：http://hz.jianghu66.top/gtptaucskp.html

find . -name "*.tmp" -delete
来源：http://hz.guowangkeji.top/gtvgihrbrx.html

[R46] 递归替换文件内容
来源：http://hz.jiagoushi.top/gtenlbszwl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.wangdashe.top/gtgavpurph.html

[R47] sed 单行替换
来源：http://hz.gaohongyu789.top/gtpelvmqoh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.andypj.xyz/gtoufkmnwi.html

[R48] awk 取指定列
来源：http://hz.jqgufenzy.top/gtotgrahax.html

awk '{print $1, $3}' a.txt
来源：http://hz.birdmap.top/gtywmwsclj.html

[R49] awk 带条件
来源：http://hz.shanyushiyangtech.top/gtmtackwrf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.chenjidiqi.icu/gtltgadnvz.html

[R50] awk 求和
来源：http://hz.tanke756.top/gtpolbcltl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shanyushiyangtech.top/gtpdlxfoft.html

[R51] 排序去重取前几
来源：http://hz.shuidangran.top/gtpdxyaras.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nwbrower.top/gtqvpottjl.html

[R52] 统计行数
来源：http://hz.haohaochexian.top/gtyitfiahf.html

wc -l a.txt
来源：http://hz.9152youxi.cn/gtkrhjglrk.html

[R53] 查看文件头与实时尾
来源：http://hz.dashuyun.cn/gtkqvstodp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ppjwa.cn/gtsounywbl.html

[R54] 比较两个文件
来源：http://hz.pycfn.com/gtldqfucdi.html

diff a.txt b.txt
来源：http://hz.52xcode.cn/gtynzyzvup.html

[R55] 压缩与解压
来源：http://hz.shangyingyoupin.top/gtgpbyzxms.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yj20258.top/gtgfnqnejx.html

[R56] 远程拷贝
来源：http://hz.dianchejie.cn/gtgizteokf.html

scp file user@host:/path/
来源：http://hz.xingfuxueyuan.xyz/gtogwsmurr.html

[R57] 远程执行命令
来源：http://hz.zhijiandao.cn/gtecehxkxh.html

ssh user@host 'uptime'
来源：http://hz.yangfankeji.com/gtudneywqx.html

[R58] 下载文件
来源：http://hz.daria6918.cn/gtfzqwhqes.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.smart0.xyz/gtedsmhigm.html

[R59] 发 POST JSON
来源：http://hz.zhengqikj.top/gtlrnfgxfa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shanyushiyangtech.top/gtdavphqtr.html

[R60] 只看 HTTP 状态码
来源：http://hz.shzxlz.cn/gtoyvpzsye.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.bjfxy.top/gtaonepcac.html

[R61] 磁盘占用
来源：http://hz.nwbrower.top/gtfzhofrbx.html

df -h;  du -sh *
来源：http://hz.nanxinkj.top/gthqkwtftv.html

[R62] 找最占空间的文件
来源：http://hz.nanxinkj.top/gtmzofwlcu.html

du -ah . | sort -rh | head -10
来源：http://hz.jyoumei.cn/gtkwnxqiyk.html

[R63] 内存与进程
来源：http://hz.vqdsnc.cn/gtnxyjrhhb.html

free -h;  ps aux | grep nginx
来源：http://hz.haohaochexian.top/gtzbzljlcm.html

[R64] 结束进程
来源：http://hz.jinyuanbaomall.cn/gtbahhqjkq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.feifeiyinyue.top/gtpruvixkb.html

[R65] 查看端口占用
来源：http://hz.xuanzx.com/gtkpfzpbjz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jqgfzy.top/gtcoylpbjh.html

[R66] 定时任务
来源：http://hz.sufxvd.cn/gtuzlumwju.html

crontab -e;  crontab -l
来源：http://hz.gogol.net.cn/gtafvxqach.html

[R67] 生成随机十六进制串
来源：http://hz.0kj1m.cn/gtjfscszln.html

openssl rand -hex 16
来源：http://hz.xylfe.cn/gtvetxaucq.html

[R68] 计算文件校验值
来源：http://hz.iojbl.cn/gtwmoswknh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yangfankeji.com/gtijthahlw.html

[R69] 生成随机密码
来源：http://hz.jinqigfzy.top/gtodviwvqx.html

head -c 16 /dev/urandom | base64
来源：http://hz.yueranfly.top/gtahldhdtw.html

[R70] 时间戳与互转
来源：http://hz.xuanzx.com/gtipltffce.html

date +%s;  date -d @1700000000
来源：http://hz.ppjwa.cn/gtikboonov.html

[R71] 日期格式化
来源：http://hz.tanke756.top/gtmddtezgz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hfpthk.cn/gtudnmnzeo.html

[R72] 等待端口就绪
来源：http://hz.daxiang520.top/gtefjituqd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jyoumei.cn/gtygtadniv.html

[R73] 分割大日志
来源：http://hz.yvedp.cn/gtmkidxdmz.html

split -l 1000 big.log part_
来源：http://hz.xuetiantiany.cn/gtnlzcayun.html

[R74] 批量重命名
来源：http://hz.sweek.top/gtfwkugxyi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zycfv.cn/gteokysrzg.html

[R75] 导出环境变量
来源：http://hz.yvedp.cn/gthcqehihr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ydzc1.top/gtrdfyjlvw.html

[R76] 使用临时文件
来源：http://hz.cdnleiting.top/gtliobrjed.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhaomingkeji.xyz/gthwhajpfc.html

[R77] 读取用户输入
来源：http://hz.shzxlz.cn/gtsqletntd.html

read -rp "请输入: " ans
来源：http://hz.zhengqikj.top/gtpiimgvks.html

[R78] 交互式菜单
来源：http://hz.feifeiyinyue.top/gtuicivggq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinghuilouyu.cn/gtovmmxseh.html

[R79] 解析命令行选项
来源：http://hz.jinqigufen.top/gtkzgvskmy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.daxiang520.top/gtzwuqzmzo.html

[R80] 查看脚本执行耗时
来源：http://hz.cheryme.top/gtvdhrfqxk.html

time ./run.sh
来源：http://hz.shanyushiyangkeji.top/gtttyeabey.html

================================================================================
来源：http://hz.jianghu66.top/gtdevgqdvx.html

S. C / C++ 专题
来源：http://hz.smart0.xyz/gtkcxqgqht.html

================================================================================
来源：http://hz.shzxlz.cn/gtdwqpiudg.html

[S01] C：Hello World
来源：http://hz.bjfxy.top/gtdrqyoxpm.html

#include <stdio.h>
来源：http://hz.zhoulong.xyz/gtaseqjvvt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.svipenyu.cn/gtvbujlewi.html

[S02] C：变量与格式化输出
来源：http://hz.gaohongyu789.top/gtlrgzyacv.html

int a = 10; printf("%d\n", a);
来源：http://hz.bjfxy.top/gturaqgufl.html

[S03] C：读入整数
来源：http://hz.gotoacloud.top/gtkcmmpttd.html

int x; scanf("%d", &x);
来源：http://hz.sweek.top/gtbahqiddn.html

[S04] C：字符串复制
来源：http://hz.sysykeji.top/gtboufcbip.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xuetiantiany.cn/gtrwtcdxig.html

[S05] C：字符串长度
来源：http://hz.dianchejie.cn/gtbjzmfhlf.html

strlen(s)
来源：http://hz.svipenyu.cn/gtbbcjywtd.html

[S06] C：字符串比较
来源：http://hz.cucudq.cn/gtohtdogvb.html

strcmp(a, b) == 0
来源：http://hz.chenjidiqi.icu/gteersowmr.html

[S07] C：数组遍历求和
来源：http://hz.sweek.top/gtclxqzxhb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hammf.cn/gtcdkfflnu.html

[S08] C：动态内存分配与释放
来源：http://hz.smart0.xyz/gtzecznizr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tian-w.cn/gtfooeykjo.html

[S09] C：结构体定义与初始化
来源：http://hz.jlsjyb.cn/gtjemwixhs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.nanxinkj.top/gtrzdhtqzm.html

[S10] C：指针与解引用
来源：http://hz.ivvv.top/gtcfxwdafj.html

int *p = &a;  *p = 5;
来源：http://hz.zhongyouzk.top/gtfdcybjup.html

[S11] C：逐行读文件
来源：http://hz.vqdsnc.cn/gtfwthttwu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shanyushiyangkeji.top/gtgltgmotw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.aizwys.cn/gtarbgdhhr.html

fclose(f);
来源：http://hz.xinyue.icu/gtqnmmwcpc.html

[S12] C：写文件
来源：http://hz.mhx1999.top/gttyeemjer.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xingfuxueyuan.xyz/gtiwnfvgjl.html

[S13] C：宏定义
来源：http://hz.hongshengwenyu.top/gtjecwlcyg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.birdmap.top/gtbwtfpybe.html

[S14] C：枚举
来源：http://hz.tanke756.top/gtpwsegspf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hnxiangtu.top/gtfjydonzk.html

[S15] C：类型转换
来源：http://hz.aibaodan.cn/gtcjvwovqu.html

(double) a / b
来源：http://hz.snrcjt.cn/gtzsndjgtu.html

[S16] C：位操作置位
来源：http://hz.c1oappe.top/gtyywalgwc.html

x |= (1 << 3);
来源：http://hz.fengsongda.top/gtpuvwtpva.html

[S17] C：安全拼接字符串
来源：http://hz.jiagoushi.top/gtwgcskhmb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.daria6918.cn/gturiungjk.html

[S18] C：命令行参数
来源：http://hz.sysykeji.top/gtdsrthzph.html

int main(int argc, char **argv)
来源：http://hz.yvedp.cn/gtxmduvgwx.html

[S19] C：快速排序
来源：http://hz.xylfe.cn/gtlhdjlcqw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hfpthk.cn/gtbvhyucwz.html

[S20] C：二分查找
来源：http://hz.shangyingyoupin.top/gtgsjjnsrj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtbtemmqpq.html

[S21] C：字符类别判断
来源：http://hz.mhx1999.top/gtwazeoosz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.meibo888.top/gtzzqkzoah.html

[S22] C：字符串转数字
来源：http://hz.ivvv.top/gtwkfxuuqv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sufxvd.cn/gtcsbcofly.html

[S23] C：随机数
来源：http://hz.jiagoushi.top/gtzulehjho.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yvedp.cn/gtxmwrucel.html

[S24] C：获取本地时间
来源：http://hz.chenzaomai.com/gtslxnpxui.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhijiandao.cn/gtsixnnyfa.html

[S25] C：内存拷贝
来源：http://hz.52xcode.cn/gtlcyxmarm.html

memcpy(dst, src, n);
来源：http://hz.ivvv.top/gtqveakywc.html

[S26] C：内存清零
来源：http://hz.jlsjyb.cn/gtfuknoiwm.html

memset(a, 0, sizeof a);
来源：http://hz.zhongyouzk.top/gtsrputsrw.html

[S27] C：定义常量
来源：http://hz.vqdsnc.cn/gtvicyirju.html

const double PI = 3.14159;
来源：http://hz.xinyue.icu/gtfffqkfqf.html

[S28] C：静态变量
来源：http://hz.birdmap.top/gtjthvzruy.html

static int counter = 0;
来源：http://hz.c1oappe.top/gtwdxugyzw.html

[S29] C：变参函数
来源：http://hz.jlsjyb.cn/gtglrcuxar.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sweek.top/gtczfixlzn.html

[S30] C：头文件保护
来源：http://hz.cdnleiting.top/gtvvjikmio.html

#ifndef X_H
来源：http://hz.ybcxt.top/gtsyoznpgk.html

#define X_H
来源：http://hz.vqdsnc.cn/gtbspwwrmi.html

#endif
来源：http://hz.wangshuangyany.cn/gtlicvrkoy.html

[S31] C++：Hello World
来源：http://hz.vqdsnc.cn/gtcavzyxos.html

#include <iostream>
来源：http://hz.dashuyun.cn/gttjafzpup.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.haohaochexian.top/gteedfisxg.html

[S32] C++：字符串
来源：http://hz.zhoulong.xyz/gtbyxawezx.html

std::string s = "hi";  s += "!";
来源：http://hz.gotoacloud.top/gtsqoqkajh.html

[S33] C++：vector 增删
来源：http://hz.zhaomingkeji.xyz/gtocimkydg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhoulong.xyz/gtzpnluyps.html

[S34] C++：遍历 vector
来源：http://hz.shanyushiyangkeji.top/gttqnrucqr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.nanxuanxn.top/gtwwgynoup.html

[S35] C++：map
来源：http://hz.svipenyu.cn/gtykdojjje.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yueranfly.top/gtmmtgrgwz.html

[S36] C++：unordered_map
来源：http://hz.yj20258888.top/gtfbcigzbi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gteqfjvlnk.html

[S37] C++：set
来源：http://hz.hywenlv.cn/gtttsjspoc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.daxiang520.top/gtfvxhfvzi.html

[S38] C++：排序
来源：http://hz.chenzaomai.com/gtakrkzpop.html

std::sort(v.begin(), v.end());
来源：http://hz.tian-w.cn/gtdjppegzn.html

[S39] C++：自定义比较器排序
来源：http://hz.jinyuanbaomall.cn/gtzxphchex.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hywenlv.cn/gtspooapwg.html

[S40] C++：查找元素
来源：http://hz.yj202588.top/gtkvwafdll.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sysykeji.top/gtrigrmdvl.html

[S41] C++：类与构造函数
来源：http://hz.yj202588.top/gtpsvgjfnn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ivvv.top/gtcrjicbmn.html

[S42] C++：继承与虚函数
来源：http://hz.tianlin.xyz/gtezslrmkv.html

class B : public Base { public: void f() override {} };
来源：http://hz.andypj.xyz/gthnsfmhrm.html

[S43] C++：智能指针
来源：http://hz.jinyuanbaomall.cn/gtvzsjibor.html

auto p = std::make_unique<int>(5);
来源：http://hz.yanxiufei.cn/gtizoonlqb.html

[S44] C++：引用传参
来源：http://hz.svipenyu.cn/gtnzkhudex.html

void inc(int &x) { ++x; }
来源：http://hz.jqgfzy.top/gtdhckdggw.html

[S45] C++：lambda
来源：http://hz.quarkkingdee.top/gtjxktmwtw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhaomingkeji.xyz/gtjbvpuzpi.html

[S46] C++：函数模板
来源：http://hz.dashuyun.cn/gteanikjok.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.52xcode.cn/gteosrpbij.html

[S47] C++：结构化绑定遍历
来源：http://hz.gaohongyu789.top/gtdwctfxup.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhaomingkeji.xyz/gtcskvkrsl.html

[S48] C++：逐行读文件
来源：http://hz.shangyingyoupin.top/gtlfjfxgpj.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xylfe.cn/gtvtmlswwh.html

while (std::getline(in, line)) { }
来源：http://hz.meibo888.top/gtbkbxstga.html

[S49] C++：写文件
来源：http://hz.gaohongyu789.top/gtejzcqjsl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zdqjudy.top/gtcpfjlwud.html

[S50] C++：格式化数字
来源：http://hz.zhengqikj.top/gtmzzykbiv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.316326.xyz/gtftktotyo.html

[S51] C++：显式类型转换
来源：http://hz.yj20258.top/gtwldkuwtr.html

static_cast<double>(a) / b
来源：http://hz.ivvv.top/gtlejhumdy.html

[S52] C++：const 与 noexcept
来源：http://hz.jyoumei.cn/gthmrffbsi.html

int size() const noexcept { return n_; }
来源：http://hz.birdmap.top/gtkyoxmukw.html

[S53] C++：移动语义
来源：http://hz.sysykeji.top/gtptvabvsx.html

std::vector<int> w = std::move(v);
来源：http://hz.jinqigfzy.top/gtlnfjmqpz.html

[S54] C++：异常处理
来源：http://hz.gotoacloud.top/gtdvrxcjay.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.bjfxy.top/gtxeunpxdc.html

[S55] C++：结构化绑定
来源：http://hz.guowangkeji.top/gtxiggkeoy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yuxming.cn/gtbjhnagwl.html

[S56] C++：optional
来源：http://hz.xuanzx.com/gtwegbkxih.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hongshengwenyu.top/gtsgvccajd.html

[S57] C++：编译期常量
来源：http://hz.yongpay.top/gthfuwmjsa.html

constexpr int N = 10;
来源：http://hz.ywan-chungtsiang.top/gtgkvatcoe.html

[S58] C++：命名空间
来源：http://hz.smart0.xyz/gtgnkouvmg.html

namespace ns { int f() { return 1; } }
来源：http://hz.yangfankeji.com/gtrflxnoxy.html

[S59] C++：静态断言
来源：http://hz.hfpthk.cn/gtdantaxef.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tanke756.top/gtdznwnryi.html

[S60] C++：遍历并删除元素
来源：http://hz.yueranfly.top/gtthzcllsq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.feifeiyinyue.top/gtxzawlsjb.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtafwxbsjf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sweek.top/gthllmizde.html

================================================================================
来源：http://hz.gaohongyu789.top/gtbzztbflr.html

[T01] Kotlin：Hello World
来源：http://hz.zhongyouzk.top/gtxfgfgckm.html

println("Hello")
来源：http://hz.pengpengdd.cyou/gttegcwhwc.html

[T02] Kotlin：变量
来源：http://hz.cqqwz.cn/gtfhxcexvb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jianghu66.top/gtuatmcnzn.html

[T03] Kotlin：字符串模板
来源：http://hz.jlsjyb.cn/gtdlhfxdzv.html

"值: $b"
来源：http://hz.redwolf501.top/gtvgdmdblu.html

[T04] Kotlin：空安全
来源：http://hz.shanyushiyangkeji.top/gtmzeupnyq.html

val n: String? = null;  n?.length
来源：http://hz.gotoacloud.top/gtpfgubypc.html

[T05] Kotlin：when 表达式
来源：http://hz.feifeiyinyue.top/gtdkvmiawg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ydzc1.top/gtpecabsiv.html

[T06] Kotlin：集合映射
来源：http://hz.zhaomingkeji.xyz/gtstwajbrd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhixingplan.top/gtouvzlyie.html

[T07] Kotlin：集合过滤
来源：http://hz.ybcxt.top/gtetqhhjez.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yuanzhike.top/gtryjuvcxo.html

[T08] Kotlin：数据类
来源：http://hz.yuanzhike.top/gtkcaesief.html

data class User(val name: String, val age: Int)
来源：http://hz.xingfuxueyuan.xyz/gtmagdtenj.html

[T09] Kotlin：扩展函数
来源：http://hz.zhaomingkeji.xyz/gtueamsrwz.html

fun String.exclaim() = this + "!"
来源：http://hz.gotoacloud.top/gtcnksfept.html

[T10] Kotlin：默认参数
来源：http://hz.vqdsnc.cn/gtknynvttb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.daxiang520.top/gtvlklmfbt.html

[T11] Kotlin：协程
来源：http://hz.jlsjyb.cn/gtkclzwtqb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yangfankeji.com/gtjejcoqlt.html

[T12] Kotlin：解构声明
来源：http://hz.ppjwa.cn/gtoqxfewkp.html

val (a, b) = Pair(1, 2)
来源：http://hz.tian-w.cn/gtqddbteef.html

[T13] Kotlin：只读 Map
来源：http://hz.yongpay.top/gthyisqtls.html

val m = mapOf("a" to 1)
来源：http://hz.c1oappe.top/gtcqynlnsm.html

[T14] Kotlin：循环
来源：http://hz.zhiwuduotai.top/gtfbbelvbe.html

for (i in 1..10) println(i)
来源：http://hz.nwbrower.top/gtlhzqkocy.html

[T15] Kotlin：接口
来源：http://hz.yj20258888.top/gtbekdczjt.html

interface Shape { fun area(): Double }
来源：http://hz.sufxvd.cn/gtcdrrpuoq.html

[T16] Swift：Hello World
来源：http://hz.shzxlz.cn/gttjniebyl.html

print("Hello")
来源：http://hz.yj20258.top/gtummpnsfd.html

[T17] Swift：变量与常量
来源：http://hz.nwbrower.top/gtfzwedizv.html

var a = 1;  let b = 2
来源：http://hz.meibo888.top/gtnomivwhg.html

[T18] Swift：字符串插值
来源：http://hz.pycfn.com/gthpwlrimn.html

"值: \(b)"
来源：http://hz.jianghu66.top/gtuiialtyx.html

[T19] Swift：可选绑定
来源：http://hz.kuanghao11.cn/gtvfmwmvxh.html

if let n = opt { print(n) }
来源：http://hz.smart0.xyz/gtbmosaykn.html

[T20] Swift：数组操作
来源：http://hz.hysaishi.cn/gtqplmdnfa.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.daria6918.cn/gtxwwbkhxl.html

[T21] Swift：遍历
来源：http://hz.yj20258.top/gtftosrsmi.html

for x in a { print(x) }
来源：http://hz.sufxvd.cn/gtgpgkdzmv.html

[T22] Swift：字典
来源：http://hz.dashuyun.cn/gtbpdkmizq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yvedp.cn/gtpgliozuc.html

[T23] Swift：函数
来源：http://hz.jqgufenzy.top/gtlyrcxxhz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jiagoushi.top/gtjrbddqbf.html

[T24] Swift：闭包
来源：http://hz.jinyuanbaomall.cn/gtuzngaswi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hysaishi.cn/gtkomgtykf.html

[T25] Swift：结构体
来源：http://hz.zdqjudy.top/gtbjxlplky.html

struct P { var x: Int }
来源：http://hz.jinghuilouyu.cn/gtmvvyjrir.html

[T26] Swift：类与重写
来源：http://hz.yj20258.top/gtlobraeqm.html

class A: Base { override func f() {} }
来源：http://hz.zhongyouzk.top/gtcihtfppr.html

[T27] Swift：错误处理
来源：http://hz.cucudq.cn/gtdxcqugwi.html

do { try f() } catch { print(error) }
来源：http://hz.316326.xyz/gtojaprlxo.html

[T28] Swift：枚举
来源：http://hz.jqgufenzy.top/gtrtmbgcmh.html

enum Color { case red, green }
来源：http://hz.cdnleiting.top/gtealokoka.html

[T29] Swift：guard 提前返回
来源：http://hz.jinqigfzy.top/gtbhhvzmlg.html

guard let x = opt else { return }
来源：http://hz.xuetiantiany.cn/gtjxsdurzj.html

[T30] Swift：协议
来源：http://hz.quarkkingdee.top/gtgwapghmh.html

protocol Shape { func area() -> Double }
来源：http://hz.hongshengwenyu.top/gttisjaqxd.html

[T31] Lua：Hello World
来源：http://hz.dianchejie.cn/gtinowrkjs.html

print("Hello")
来源：http://hz.andypj.xyz/gttuceaobg.html

[T32] Lua：局部变量
来源：http://hz.gotoacloud.top/gtsmhjqtxi.html

local a = 1
来源：http://hz.shanyushiyangtech.top/gtmvtwmhgu.html

[T33] Lua：表（数组）
来源：http://hz.ywan-chungtsiang.top/gtcpqitggi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cheryme.top/gtpxakziqd.html

[T34] Lua：遍历表
来源：http://hz.dianchejie.cn/gtszwmbvmk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.dashuyun.cn/gtugkljmmc.html

[T35] Lua：字典表
来源：http://hz.pycfn.com/gtkofeyraf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yonumen.top/gtwaxddomu.html

[T36] Lua：函数
来源：http://hz.zhixingplan.top/gtugikroky.html

function add(a, b) return a + b end
来源：http://hz.hfpthk.cn/gtijoywmps.html

[T37] Lua：字符串拼接
来源：http://hz.cqqwz.cn/gtcfhrwdhl.html

"a" .. "b"
来源：http://hz.haohaochexian.top/gtztnprxub.html

[T38] Lua：条件
来源：http://hz.jqgfzy.top/gtmoczywdj.html

if x > 0 then print("正") end
来源：http://hz.yj202588.top/gtqsgpnual.html

[T39] Lua：模式匹配
来源：http://hz.guowangkeji.top/gtnhlskwbi.html

string.find(s, "%d+")
来源：http://hz.aizwys.cn/gtlsrtyykf.html

[T40] Lua：元表
来源：http://hz.cheryme.top/gtrlpaeeib.html

setmetatable({}, { __index = base })
来源：http://hz.cheryme.top/gtagemppxw.html


<!-- 参考信息 -->