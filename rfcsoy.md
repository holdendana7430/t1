代发 wailian999

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2uwzoqltm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2zriovvus.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2unirbqcc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2dlyvdylb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2tjrvxeeo.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fehhbarg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2evlmxxik.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2muqzrtre.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jptwduzy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2gicvmqsc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hqcboygh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2rhotkxar.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2yjsnqwyj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2rsvyopds.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pwobuqnl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2pofxxaaq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2rsagvitg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2eohvhacd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2goczbglp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2gtjedtfg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2vpfyfzdu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nvuitfwk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sghnqnqx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ijpcrghu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2axpcsmzq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2duzwdtgc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2olvhitib.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2evawqujc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2xlunalqp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2nnnkfnhn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2njmoipqh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zntopprs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ggtmgbpj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cmgydcud.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2duntdtgy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ofuofycz.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2sfnoohqk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2zrlalpgg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2siwewiwj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ewcvkqcy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jpcvjivc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2vkfvbvkd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2eqlgunmv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2coemmovl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2sfckrvjm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bsjlpypc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qtmgpvdi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wapeieno.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2hftflowp.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2uqzwznnk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2aoukbwgz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2rihiiear.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2uyarmvmd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vnrcoqdh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2dmkrscjr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dbncylvu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2dblcsnkn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2pqxwxrzj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2caczzdmx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ixgoptqq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ivbzlimw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2qyoqquws.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sqxcqcdo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pvtwjtfa.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2bcycjwte.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2uhrswckq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mzyegomr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2vzvjttnn.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2adoegtns.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2koriimae.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2inwiqtgl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2xauimgto.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2lyzrmxqm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2hftaitlr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2zkrnitik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jekeksaz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2otrgbxdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbuhahsd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ipuzdtsg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2lhogylqz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2wolfcxce.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2llibjawq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rtecemrv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2muhqlehz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2lonshzmn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ngtrxpqs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nxtjvdwa.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rdanzlvk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2xzikjsyq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gpdrhtbh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2qgadbumf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2pzanwhhg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2jymsdlpw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xstgefpo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2qomqtqvx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ncvlczri.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2pegvnklx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2fkhsqduj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2fqnvcggo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dempjebd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ymwdhesu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ddxikxxr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tftcxudf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yqpquaon.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jcgeaugw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ptcwajrx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2cqgfatwy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aleowahv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2tdskrsgr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2rbtigivy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2xdojrgrr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2lnrookkk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2xexqmfrd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zsvknrof.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2mwkpzfiz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cdobouyo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2gofmtmys.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2trxelehk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hqxkejoi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2zjigfqlw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ekitotmz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qamjtydx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2vdeawapm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2utedmbnw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tyufnvye.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2mhkzlmap.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2lvykndda.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2tajlbyqh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2sfdnusxk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2rxiagjxy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2sjryjkud.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2islxvwqs.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wqieekrd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2dyvinsah.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cwtblkph.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2vcsinzpq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2hbyzqwsl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2obiyuquj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fweagdtk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ooeyvxno.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wbbgyngs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ichqbnoh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2zeeizwmp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jwqoekvg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2wzynlvdq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2hfckaddj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2putcycmt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ovjkrlfi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2yeueqioi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ykognekt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2vobtmqzo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2iljybsfq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ncabblfm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jhkiqbdv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2umjcfluh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dxbavnzj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2buyysbqz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2eqigwtle.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2aoxzkpyk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ffslcodh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2jkfaosvt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2gfruzgfk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2nvtxwlit.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2txlmocuc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qxtehqxm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kpcvxdzl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2uepnnhgw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rhnthixp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2lmliabed.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vsidtwfi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2hcbrrkre.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ajmhxmtv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2zbeqpscw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xtoubgpi.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2yotrgssx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykeinidu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ylxrcaed.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2mxtpicfk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2izaffojy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wleyuxfe.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2tfajsbiu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2bsldghad.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2chcicvyl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2llswxxqf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bryhivet.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2aeyzvphl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2pcwresji.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2zkdrovci.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkyknohy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2kvnnbikc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2jwlnjbty.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2bpxsmale.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2fdtyzwhk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fzamtfhg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tciflgrv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2zujeucuu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2dbkxejnj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2wwgxkeia.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2hczhidjf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2mlnebarj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xxzhmslm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2bzxlydjp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2vabqauvu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2xwnlvvph.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ikszhrzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwcckqyq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jrsjyyct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2teooewyj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bshajmak.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2axsspqqh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lgkoerwj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2xdmgrjqs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2dyeysjhi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ffqbvipa.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2muebageq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2sfrjzlhk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ewxbqgcz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2vurhrmre.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ldhpupgp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hiciqvit.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vcrtjvve.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2qvijmxsa.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ghpjynzi.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hznihltb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2rrhnltwa.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2rdnmnyfy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wthrwtse.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2wuvueeyi.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ihnkglyb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2nqfltcwn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2juiaclmm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ofafddhf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kmdpefgp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oiwniuih.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2agtnfmos.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rjygnmxi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ipyxzswi.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ggxvlayo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ekqjpyor.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jyynlldv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ffgrijhr.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kxvinskq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dpoywjdp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2oezlbptm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2vcduauug.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2xgeyqdym.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2auxidelo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2vcraqpvf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2qaerxysx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2wqmxkped.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vloopuvg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uazqwqct.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2hhtgqgmx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mhefljkr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bsfuvbty.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mrkoluzi.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2tmwguefr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2jlvgwdwj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2byyqztke.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2pbkhadgy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fvoazbok.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2uizqojtu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2wciclqpy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2rqfaeumh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ylxdodgf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fyolyxjr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yfpldyzm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2oyctcsdd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qkywswpr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2aeqkglya.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sqzutthf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2mtqksqev.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ckzwiazi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2tfbmdbxm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2mvuouzlx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2cgnfeytm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2wsgljgke.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2yacdyyae.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2pbaaztao.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2devpbdss.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fglhnghx.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2cjzdzwpz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ponxcorw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2qofegtla.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pnomkkio.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ncocihsx.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2kfonkdig.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2jglupmzd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2keyaimfu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2qvkftwbg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ywlqftip.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2pwhdlxrf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tfxsnmrs.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2rhyvmdln.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2appfikbc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbqvufgq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xdijmgok.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrqzkgdd.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2eawcvefz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2wkqetwjd.html


<!-- 参考信息 -->