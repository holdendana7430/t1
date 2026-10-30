代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gwazopytb.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gqcoczklx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gemacmbzb.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gfmldieix.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gkzgesfnq.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gujzmfrmj.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gnsambvsr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gcuqbkrjv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/ggoxufdvw.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/giprjcmrq.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gkbummufj.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gavywkbfp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gfdargisj.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gvaatcqud.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gtopvnsrp.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gbozptlgw.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/ghsgzmjqt.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gsfttrlte.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gjbobgcrm.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gbnwgdvse.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gqumiyzpt.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/goiqxktpn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gcijsvsci.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gykquifli.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gktjuiwza.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/glxwtgwoi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gimggsdns.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gjhjxmetc.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gmbcixfpn.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gzxwfzaas.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gktzyzssy.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gntythgjr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gmlngcmsz.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gkemmrboj.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gsttdmnft.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gxaqorljz.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gousobzwg.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gaarzvtkj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/ggcrxbltb.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gxjhokbkx.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gfhbdyogb.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gnwzewjfo.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/goixgaknr.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gevfsiitx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gbkujndml.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gpoalrnfc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gmbspkhjy.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gthjqjglq.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gjphlhowa.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/guknvpaqp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gerzxsrtc.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gkiykhqtn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gohxofvtr.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gqkovedtk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gzfzbqbxr.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gidzblwso.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gxdpxggmc.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gcgerzvii.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/glounrxcu.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gsiwhioec.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/glmxdzeob.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gagsymhpf.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/glhwwwmqk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnaxgidib.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gwzhvqrot.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gokbrtkda.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxsnoxyud.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gvjwvxasm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gxjorpnxf.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gwwqcebtz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gykfwdskj.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gnfnrkoqt.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gvesbuxyg.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gjcymveee.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gqmkfunxo.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gdjbwafsy.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gnudtqdgc.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/grlyijoyg.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gfugmrgal.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gyihxzesb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gksaoafgb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gnudkmqxu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gtiynzeuf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gxedwucug.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gtcwiynlu.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gghyzmihm.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gnnyjpunw.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gcuakrsww.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gnajrvjwo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gkzxsuykp.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gqwccejft.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gxwwjwpdf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/ghhoatiji.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gnacscsoo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gfheehngt.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gffvhpomm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gyrqnsdzf.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/ggidjytwo.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gamawuqgz.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gxquornxw.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gicceglwv.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gfopsvmvj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gkkykjaxd.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/grptdcxip.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gnbawtenb.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gbkvabjpe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gjrhsbavi.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/glngqsyzr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gnovkbznh.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gvfqnkigv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gszhotufg.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gpxxljggg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gsmaqbcja.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gvjbwgwvr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gehmytcfa.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gneuamlaz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gwrwtgfnq.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gokoqfrcu.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gyedokguy.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/goazjtzup.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gteumqydi.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gndarirlq.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gxiazuleg.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gcgwunvql.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gxtmayuhw.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/ghvwiiyab.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gmnmpgxlt.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gzxcaavoi.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gcojmodpf.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gyvllhkbj.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gydkagakc.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gbzmgvkqu.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/ggujivdqj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/guafkrbxl.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gergpxrbd.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gjtgpyfvk.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gmourkwwy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gzvfurojr.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/ghkjyenbx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/genbsocdv.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gipugkmji.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/grgvdhyha.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gxwdubpnp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gikwtiamb.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gkfgfmtgq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gikhnnpxn.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gmlaodxxt.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gutsvzrkd.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gdfljwwds.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gnkruyfye.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gkpnehjyq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gbpgrocol.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gyvshjjpt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gjdjuhvmh.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gelxunbtl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/geqkpijpi.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gynsileok.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gitvqbbqk.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gmqnnhdet.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gcudypqgg.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gknslrwlz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/ghnxveekn.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/grehawqgz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghiafjlcj.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gihzcaemb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/ghyszivbv.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gxqnppdin.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gvkywzqbf.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gbvfnbngc.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gthvbajxs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/ghcetszeh.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gdywjpdqc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/glpwsffkh.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gkmmsjitu.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gpfcccjzi.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gibvrdara.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gvkgvbthf.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/ghdnrynro.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gnkvwiinn.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gjefhnbvl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/givybiabz.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gtyrwgxlv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gqdiszrus.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gwxwevjko.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gfyfisdrp.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gbskfpssb.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gayhdjxqs.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gwjxjqjpb.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gankgodje.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gtbdafgvr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gnhlekxub.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/glmtuahwv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gfknvrtxe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyzrpmvpc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gbelspkcx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbwmielqr.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/glubjchtj.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gepxdrnpe.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gpmzurrxq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gqpsbcxqi.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gmhpeicrg.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gbgdtiojm.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gcvygsqyo.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gfsmjgjkz.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/guamigiwo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gdvwdjdsy.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gllqdjdyr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gmxxkvqtk.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/ggdocszbe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdrsutril.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gjhjuqkid.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gelgggyjm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gqdtifgpx.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/goqtsbknt.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gqxhqzwbq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gglnyjnxs.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gqefqlqjl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/ggvtadelw.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gyoxrjyzz.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gfxynqbbi.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gghbpdkxm.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/ghqwhwjkq.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/ggokjjzdy.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/giujvtbwq.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/glikfesyg.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gofsvwghj.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/geepsoklx.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/ggckqxzfz.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gwlegossp.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gjlsqvnyn.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ghpxeuemm.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gtpmmkbsu.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gekkmnuxy.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gklatifxe.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gkywtkdzk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/galojfyzx.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gaikrespg.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gayobioil.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gqxzyrpid.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gfloxqfpr.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gcnlkynim.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gsjwujjxi.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gwhggxfsh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gxqanajqc.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gllkcsqek.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gurmctjdd.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/glggyjwht.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gwajgfpok.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gyqictvwd.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gotajphmp.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gxnjvhcrp.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/guojgufwn.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gubeelick.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/ghlbcocrp.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gnttfojjd.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gekdmjsrs.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gtjfiyeno.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gqddppavy.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gleotaulh.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/grvcrykqx.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gsnihlwwg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gijnwogdk.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gfgzjusqb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gpijzzcxy.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gklqhvjnt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gknqvcphw.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gpvfucdsu.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gutjduvkp.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/grvucnejx.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/ggouyuacs.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gziqoiwsi.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gnbipzdhw.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gzzrscphv.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gncxgxbgd.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/guibqkyyg.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gguedrxgq.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gogimvxyu.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gtchkzvmn.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/glkfrwynk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gpzmtycdw.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gdjgizhkp.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gxlcuzgft.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gifeaqhrl.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gbtkvqozz.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/ghbulmdyi.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gzcyfwytx.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gmeelxybi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/grmthlgbv.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gkksjyjvk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/geugrnooj.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gwjluloou.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gfrmzgbhh.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/goifhinnh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gsvnwwpbo.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gsbcddcbq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gwnrtcqov.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gmsjjwrxa.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gdufkrhsw.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gjkqbgrit.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/guhpqembw.sHtML


<!-- 参考信息 -->