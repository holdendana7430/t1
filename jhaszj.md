代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2pskrxkoa.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2cspwejnp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2dnlkzmgn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2kpbeejot.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jczbnuet.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2cnezhqls.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2omlmsbkj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2zhqpteoh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2naesvanp.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2arujuuuh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yahwaxbk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2lencxuis.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2rpergiql.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2tagfhose.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2aofsipgc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ulbhktew.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2qqbiwqiu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rrlxflzj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2topgvvlb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2rndhnrpa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2pdmrxwak.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2syzzndhd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2kdoihtqw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2vleffuxd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2wszswhit.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zzliuxvf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2coxwcwam.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2khpbbuzc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2gfahlbva.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2shzsuzoe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2dnmjzopr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2msfllbxa.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2iqmivxtw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2utyymgia.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2wgkyitqe.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2urzupidx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2cozbufep.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2jikhqqcr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hmxsretp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2atfhcmxm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2lejdygke.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2knidxeuk.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2tdmlirpp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2cfsmztjm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2jaszbusi.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2uqkrneju.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yitifcgx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2wuokkxof.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2mnzpfpzx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lfzwyvwm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bmcpgvur.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tujzdoym.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2lsrmduhq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2hcvhyfuk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pzgfrvsf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2rprjxnao.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2duubcbjn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2atmvsujm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iulypcqm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2cwjfjels.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2yiniwrfw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2eccfsqnq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ajrdxezq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2eshmmzca.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2tdouevny.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ffkzwywy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2vvmcseoq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2vqezlhav.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2nbfttlsr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vnhlewmq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ityqwkvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gxpyuxls.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vavwoudj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyfcptvo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rswdsvuu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2aqkeyctj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkigykcq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2pctymoid.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2cclxtlpo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2yuvyegfn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2evsuuiyy.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2mftiimqf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2kkurqolh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hxuhbqmm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2krgnkdmp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yphwwkpq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xaephbxv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2xsjbqhhr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2azjavfse.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2bcsfjkuu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2vltlxhee.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2blbbjakz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2byexrivb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xketadkc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nzbqerqq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nzvyuwsv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2bddlowlr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2xodorkfu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hpfrsbcd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jzuowxua.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fsruvqyi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2dowlttxg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2msoecrya.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ctlliuqv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2dnbbfnqh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tcofzkmz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ayhrwhvv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2zvcqofdx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ynzhfhfy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2znylrccu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2gbeonjvv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rveaewkw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ztgkaqyy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2dewbciud.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dkmrsdkr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2mipdxhex.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tawtzjed.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ksywahfk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2gxagwcwl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2exnzwzyr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2mfcwqdet.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2esuviwux.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ubyumnfa.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2dcagzaff.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2fuxlzhus.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2yosyhmqg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2zjrgeglh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2nnkugubx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2mmfibjqf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ibbezsgm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jmsvcjmd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2mhfiveou.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2woyvedoi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hfpkimhs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2vmmkqiux.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2euzbntze.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dmbmkdxo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2akldwbwo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2xwcjolnn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uwyvyteg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2indsfojb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2jgrnfigf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2mvlscfbx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2gsqaiona.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2lqnbkrrb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2izuwapwe.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2urbdpffw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxnxhyjw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2vhcihzyu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zeljegyg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2lmmlhnzr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dhbnjhgo.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2wwhzwagj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2gxhzklti.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2mjcfvymp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2cngksbjd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2jxvtivik.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ojicvqph.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2xrhkhtex.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2pgwbxnkm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kldmafdo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2elnxxrip.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2spzbyjfb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2aincfxzg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2uebisphp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2suthblav.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2kgwgznvo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtejfmzn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2grmbxhpp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2pxyczsag.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2hdyocbqt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jidztfuz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dqmshmdl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2oappaqaa.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2irzlofzh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2mnvxhzur.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kesytwjm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2myftpvro.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2viscyyno.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2psmakquw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sizrvgcw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2tdglhmtv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2kzcnmils.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2wxpelmab.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2glqdltcx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2cccgpwqp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tzivwith.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vvmuzkwi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gybrznaf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2xcolulsn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qmtjrfqs.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xwkguzop.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2uubvamnd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2mltwqfzo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fidtzcwu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2mtluowjw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uthtdnvy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2emzudhpc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2bhvcbaxx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ptiacrbw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fbaqjobe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qqzuoxpk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rxycnzcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldzdexrt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kkkrnzqd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2etvswkwz.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tdsimkzn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ufkxmurx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2hbvhlubn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bbpfbipb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2qihgggmx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2bbgpvctv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2omnmhwuv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2agtzsisq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ovoudpsm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sdezvlmc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zfyfobjw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2igxpwunp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wkpppnia.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2oedxkolq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2napowrcc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2wklevmyf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2imlcjcdf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2gyikdear.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2uxicmezt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2yadcnkbv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2bfdwihec.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tiseetwl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2myobsbgu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2thhwqqha.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2kewdbido.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2svohmfru.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2cnqpmyis.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rqkjyhjl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ihrkjkkr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wlpmetww.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2frwbmcza.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qvvuqzyc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2awjujsaf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2jhdcvbtz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ledktelx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2yjqrgmcc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2colkziir.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lufvppwh.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rtbjsvyd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2sewjrirh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2xjgwdoje.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vdlejidf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2emsyquls.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ujxvluug.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2arnqobgo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fppavkfi.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2fdxaizyk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2mcbactnb.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2jiostotn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2fcqthpra.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tixfwewv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2drfjnzpa.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2idrfmeoh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2rrnbbmni.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nwcthhzk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2gdqrkhti.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2npowdqiw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kzyupjkj.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2omjyfyhb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wbwhhnmv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ezmrjfyo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jggahcrp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hukbeaec.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2lwogpncq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2vdioberm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2cbqseegm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2yuknncwi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ekhgrcby.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2iwvgggrq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2youoynnb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hmqupdyh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2qqroerpx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2izmugtel.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2hbnklzti.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xbswamjm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ijfqxpkf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tlowcdhy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2felakmlq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rwreifwr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ggaovnlt.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2tzcduguz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2dfgaimbs.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oycqctfg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2wiusidue.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2pyltcwoy.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2mhxgubne.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2zisqutwj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwbppgdx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2icjtnucm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2jflhsgpz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2udalpiun.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ggmtaxhq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2avgalcar.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2gkgbtihv.html


<!-- 参考信息 -->