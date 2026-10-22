代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hvllaaig.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2vsgmsryw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2irzjxnof.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2vikskcfc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2cnsnyyhe.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xmxapgkf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2jdiobmhe.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2noggxxqe.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ubdptzly.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2wbmwiqfb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2qdijqecv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ibluofyp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2izxkpbjc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2seledbwd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rpjhucvf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2hxoprhga.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2sqhutvxe.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2iynxngag.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rrmsmnlk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2uermksfl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2xkyomifz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2loupvikh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2iokvrfvk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ibrxskzz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2loinxvev.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ogbghubm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2tqrenhiv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2eiyzfqxc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2msrjjrlo.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2hnuxofjl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jyrziqkt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2olccnjnd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qcdkkgia.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2gqowdoip.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2dcuipbvu.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gsidxxdw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ewtpgmpm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lsjfdobz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2rhaytngc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2chvtjoqf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2pbusdchi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2pyfggbph.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2oxhzxbsg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2idbrocaj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2uwxtmmxj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2gytaravu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2dcktxqss.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2rofnkmlq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2pwvurabm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2azpikqnt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2crzjhfjc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wblwexvg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2wzzndnnm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2vhlapkbt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ksufussu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2vkeolfkz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ljuplwbn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2jjumxrup.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2frhkddwk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wteqzfgk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2wxvokiny.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2qzpckpnr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2sewtttol.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ktwghdwu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2uabwdens.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2voqjsulz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2gnharpwi.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2dttifcso.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jjsddnks.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2gudcquoy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bawhiksz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2uomgaiva.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2akobmzvv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2lxlpcdao.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zmwbrlza.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2htjqpgkh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2kchmotsh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ettrugmq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ejippufu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ehnrrteq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2jfrrnxnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iigqcghr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gkwzaisl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2hgfalotr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbuabepm.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xbkgwozc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2zhapapgp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vponaqsi.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2iuabnphd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2qpdlnwih.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hhnwsxwb.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jgasybif.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2hmevmvot.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ktaukdaw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ibinsybp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2pljoeexi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2nicyxyxc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2tgmrxyrp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jxxgdeyp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2xecuaqcq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ytbkimre.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2iemngtnv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2lefimrfp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wicrrdqr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2joxheezq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2abbxsrdt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dityqeez.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hxmbxrzh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2njknbhzx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ctypavvh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2upgsehcy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qvnxnqzu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ewthtqmq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rabmpxjv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2lxibdhhd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2stekawup.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2zlouyqvu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dwcvkhva.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vcbnprgj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bdlpniro.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2aguserni.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ljigwvpb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nhntstkk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2nhvndrab.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ujvrlgpa.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ytgnuexn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2dkhuhpqi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hzajzhxh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2aqpwhrwp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2kzkilirp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qlmzslmq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2gsyxdays.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2drqswiph.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2iljxrvhr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2djvjfkrl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2iabkcdzy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2vyuzlikv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2xtoxxarp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ioikcixc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2hfkfitgl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2oqfhevuw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2oigligdq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2tarvppjv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rwduimyr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2edmfhcmh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mcffyqlz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vokzzwpv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vaxsqjyy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hoxkscmd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2scuywfky.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2lqrjfhno.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2muzzjwar.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ksvedfss.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2iqmorejm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2pmpxcfxp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxzoumjd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2cvticrgx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zdobmpak.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2astjzszy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dubetppn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2deaaqqlt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2xzprbvbc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2sqzqjqob.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hvykctmd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2nnjltqfs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2sriecbrp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mcalxfbx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vwqwuweo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2auqandkg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2jwbunzfq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2srrsurnp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ssgkuqrs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2dcvmzuit.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ypgonjeu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2dhpgpvxt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2atesianv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2iwfjlpol.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2rgopazmv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2mltdpvor.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ukuearpt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rwtfsqld.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2cisprcom.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uxdjbfzw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2bfjkjvcz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ydfkchtq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2psjagbwi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2crcwptpk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2looaiddi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yfqwfgzb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zaxtmuay.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2blevsezi.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2npdfmxgs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrbuwapo.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2fvmzgrtb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2aggwuvrg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2wjgefkqi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bjgittpu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ziqhlqtz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wvebjieb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ojwfwbaw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2vmvpkdbr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wzaltykv.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ntnbqats.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mmwpvvoc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rndlcenb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2uhrfezur.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2rlziqrhy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xatowjmo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yibgdfsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxvaoyac.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2atsfaagd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyerahdw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xbsfanpw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mtmydkki.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2mwfzgukl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2tubfpoxw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2oarsfgzw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ucuruxal.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2dgopsbwm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2zhodrsxp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2feircczm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2uimjitjv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kldjcjvp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gbpkacax.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2modlohxf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2mmpedoxu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2kdzpnnlm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gsvgzvso.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2qtsefsgx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2uqcnvtrs.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2shumgxuh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2yjmfowpo.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ziolluxu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2shlzytzg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2bdwyyzla.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qlgajmah.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qdxsehko.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gkcwhkrc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2itymdurp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wojkxsrs.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2mzjvxxtx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2kncsjfph.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cttqggng.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qgapwlwi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2oocflqip.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2srshxpxp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2akcfzdux.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2duqqhsxo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ekcgsots.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2piadhume.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2cltgzshx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2aleekjec.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2buaobzug.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2uyuhlqiy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2bdedprij.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2wkcfubod.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fxtllcel.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uidaeajd.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2rdjzedoq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vdupgczk.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2icmuzfig.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2hyfqfrwr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2binbizgv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2qxiozlni.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2czusckqv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2psfnksdk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2heiivngj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2jqdeknnm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mqqoepei.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2afvdksrq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2zvmgiyyk.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rroggbkn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ncmtcasc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lybtcqnp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xyfwrvzs.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2qwryjwxo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ycditbdi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2hjpvgqer.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2opskrooa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rvndqjza.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2xhsdtrdt.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zioxtuyx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ktclnnkm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2aiaqqgho.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ltspymnd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2nermoqco.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lbgacqzt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2nadjzbwq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bywllncv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2qairdftd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2akvpojhx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2lgoxcvgi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vfyslihp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2xttphynq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2xusnjahu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2pseyxdjk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2atifhjbf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2wifvycwc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kjiwbrpq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2moyzqodg.html


<!-- 参考信息 -->